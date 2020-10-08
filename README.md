# Lasticot

Multiplayer snake

## Project Architecture

```
|-- /.github
   |-- /workflows
     |-- cmake.yml
|-- /cmake
|-- /doc
|-- /main
  |-- Client.cpp
|-- /src
  |-- /include
    |-- Worm.h
  |-- CMakeLists.txt
  |-- Worm.cpp
|-- /test
  |-- CMakeLists.txt
|-- .gitignore
|-- .clangformat
|-- CMakeLists.txt
|-- README.md
```

## Compilation

### Linux (ubuntu) and Windows 10 (64 bits)

```
cmake -E make_directory build 
cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
cmake --build . --config Release
```

To run tests
```ctest -C Release```
