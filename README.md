<p align="center">
    <img src="https://seeso.io/img/logo_shape.bdd77355.svg"
        height="130">
    <img src="https://seeso.io/img/logo_text.6064523e.svg"
        height="130">
</p>
<div align="center">
    <h1>SeeSo MacOS Sample(C++)</h1>
    <a href="https://github.com/visualcamp/seeso-sample-macos/releases" alt="release">
        <img src="https://img.shields.io/badge/version-4.0.0_beta-blue" />
    </a>
</div>



## Sample Demo Requirements
* [SeeSo MacOS SDK][seeso-manage]
* Must be issued a license key in [SeeSo Console][seeso-manage]
* C++ 14 or higher
* [CMake](https://cmake.org/download/) 3.5 or higher
* [OpenCV](https://opencv.org/releases/) 


## Build
1. Sign in to [seeso.io][seeso-io] and download a SeeSo MacOS SDK from [SeeSo console page][seeso-manage]
2. Copy the `seeso` folder to this project.
3. Get a license key from [SeeSo console page][seeso-manage] and copy your key to `main.cpp`.

   ```cpp
   // authenticate
   const char* license_key = "PUT YOUR LICENSE KEY HERE"; // paste your key here
   ```
4. MacOS install OpenCV library.([HomeBrew opencv info](https://formulae.brew.sh/formula/opencv))
    ```cli
    brew install opencv
    ```

5. Build the project with CMake
    * You can load a CMake project with IDEs, such as CLion or Visual Studio
    * Or you can build with command line  
    ```
    cmake -B build -DCMAKE_BUILD_TYPE=Release
    cmake --build build --config Release
    ```
    * vcpkg is not supported yet. If you want to build with Visual Studio project instead of CMake,
      you have to manually implement the source codes and third party libraries.
      
If you have any problems, feel free to [contact us](https://seeso.io/Contact-Us) 

[seeso-io]: https://seeso.io
[seeso-manage]: https://manage.seeso.io/
