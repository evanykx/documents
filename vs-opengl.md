1. download 
```
https://www.transmissionzero.co.uk/files/software/development/GLUT/freeglut-MSVC.zip
```

2. Debug | x64 > Property
    1.  VC++ Directories > Include Directories
    ```
    + FREEGLUT_HOME\include\GL
    ```
    Or copy header files to 
    ```
    FREEGLUT_HOME\include\GL > 
    C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.23.28105\include
    ```
    2. VC++ Directories > Library Directories
    ```
    + FREEGLUT_HOME\lib\x64\freegult.lib
    ```
    Or copy these library files to 
    ```
    FREEGLUT_HOME\lib\x64\freegult.lib >
    C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.23.28105\lib\x64
    ```
    3. Linker > Input > Additional Dependencies(select one)
    ```
    + freegult.lib
    ```
    