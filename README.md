Skeletal animation using C++ and OpenGL.

## Fork notes

This is a fork from <https://github.com/MathNuts/SkeletalAnimation> and a few changes were applied:

- Backports OpenGL code from `4.6` to `4.1` to enable support for **macOS**
  - Removes layouts from shader code since these are not yet available in 4.1
  - Dynamically retrieves uniform and attribute locations

Shadows, unfortunately, are still broken as of now.

## Why?

I created this project in order to explore several aspects of OpenGL and 3D animation. This includes but is not limitied to: lighting, shadow maps, texturing, model loading, animations and skeletal representations.

## Building and running

To run the code, enter the build directory and run CMake.

```console
cd ./build
cmake ..
```

The build directory will then be populated by a VS Project or a make file that can be used to run the project.

This has been tested and works on my Windows and Linux machine.

## Movement

The model can be moved by using the WASD keys along with the spacebar to jump.

## Video preview

https://user-images.githubusercontent.com/60390557/164997059-28e2f81a-2872-4af1-b552-d4e89537e770.mp4

## About the 3D model

The model, textures and animations are all made by [Mixamo](https://www.mixamo.com/#/).
