# README #

* Set the parameters before dispatching the shader (see source code)
* Supports noise map sizes which are multiple of 8 (due to gpu thread layout, google for "wavefront") in height and width -> chunks of 8x8=64
* For other sizes the threadcount needs to be modified, [here](https://learn.microsoft.com/en-us/windows/win32/direct3dhlsl/sm5-attributes-numthreads) is an explanation

### What is this repository for? ###

* contains a ready to use compute shader to generate perlin noise on the gpu