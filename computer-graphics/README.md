# Computer Graphics (NYU, Fall 2021)

Six assignments for Computer Graphics, NYU Fall 2021, written in C++ with [Eigen](https://eigen.tuxfamily.org/).

Course materials: https://github.com/danielepanozzo/cg

## Contents

Each assignment folder holds the assignment spec (`README.md`) and, for most assignments, my write-up with result images (`REPORT.md`).

| Folder | Topic |
| --- | --- |
| [`Assignment_1`](Assignment_1/) | 2D geometry: convex hull (Graham scan) and point-in-polygon test |
| [`Assignment_2`](Assignment_2/) | First ray tracer: orthographic / perspective projection, spheres and parallelograms, diffuse / specular shading |
| [`Assignment_3`](Assignment_3/) | Ray tracing effects: shadows, reflection, refraction, depth of field, animation |
| [`Assignment_4`](Assignment_4/) | Ray tracing triangle meshes, accelerated with an AABB tree (BVH) |
| [`Assignment_5`](Assignment_5/) | Software rasterization: wireframe, flat and per-vertex shading, object transformations, camera |
| [`Assignment_6`](Assignment_6/) | Interactive 2D triangle editor with SDL2 (insert, translate, rotate, scale, color, zoom); key bindings in `keybinds.txt` |

> **Note:** Assignment 4 contains only the report, data and result images. Its source code was not committed to the original repository.

## Build

Each assignment uses CMake:

```sh
cd Assignment_3
mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make
```
