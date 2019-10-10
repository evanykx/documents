1. system environment
```
path: OPENCV_HOME\build\bin;OPENCV_HOME\build\x64\vc15\bin;
```

2. Debug | x64 > Property
    1. VC++ Directories > Include Directories
    ```
    + OPENCV_HOME\build\include\opencv2
    ```
    or copy this directory to 
    ```
    C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.23.28105\include
    ```
    2. VC++ Directories > Library Directories
    ```
    + OPENCV_HOME\build\x64\vc15\lib\opencv_world411.lib
    + OPENCV_HOME\build\x64\vc15\lib\opencv_world411d.lib
    ```
    or copy these files to 
    ```
    C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.23.28105\lib\x64
    ```
    3. Linker > Input > Additional Dependencies(select one)
    ```
    + opencv_world411d.lib / opencv_world411.lib
    ```
    