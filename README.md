Rasterizer and Shader Toy Fun
==================================

**University of Pennsylvania, CIS 560: Introduction to Computer Graphics**

* Bowen Deng
  * [LinkedIn](www.linkedin.com/in/bowen-deng-7dbw13)

## Abstract

![](img/shader/represent.jpeg)

This project includes two parts of work. One is a C++ based rasterizer, which is capable for rendering 3D objects with multiple reflection models. Another one works with OpenGL, and utilizes different vertex and fragment shaders to achieve interesting visual effects.

## Rasterizer

### Basic Functionality

For a 3D object loaded from OBJ files, firstly it will be projected to the screen through the model-view-projection transformation. Then the rasterizer performs triangulation on its faces, and scans line by line to determine where such triangles start and end at each line. The color of a pixel is computed by barycentric interpolation.

![](img/rasterizer/res.bmp)

### Reflection Model

Several kinds of refection models are embedded.

- **Line Rendering**

![](img/rasterizer/line2.bmp)

- **Blinn-Phong Model**

![](img/rasterizer/phong.bmp)

- **Lit Sphere Model**

![](img/rasterizer/sph.bmp)

- **Toon Model**

![](img/rasterizer/toon.bmp)

------------------------------------------------------------------------------------------

## Shader

### Interactive Camera

A polar spherical camera is applied to provide interactive controls.

![](img/shader/camera.gif)

### Surface Shaders

Some interesting shading achieved with vertex shaders.

- **Blinn-Phong Reflection Shader**

![](img/shader/phong.png)

- **Matcap Reflection Shader**

![](img/shader/matcap.png)

- **Iridescent Shader**

![](img/shader/color.png)

- **Deformation shader**

![](img/shader/deform.gif)

### Post-Process Shaders

Cool effects made with fragment shaders.

- **Greyscale and vignette Shader**

![](img/shader/grey.png)

- **Gaussian Blur Shader**

![](img/shader/gaussian.png)

- **Sobel Filter Shader**

![](img/shader/sobel.png)

- **Bloom Shader**

![](img/shader/bloom.png)

- **Worley Noise-Based Shader**

![](img/shader/worley.png)

### Shader Combination

Of course, the surface shaders and post-process shaders can be combined to create more crazy results!

![](img/shader/combine.gif)
