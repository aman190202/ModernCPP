# Modern CPP 
## By Ignacio Vizzo and Cyrill Stachniss

### Method 1
#### Use Modules and libraries

1. Compile Modules

```
c++ -std=c++17 -c tools.cpp -o tools.o
```

2. Organize modules into libraries :

``` 
ar rcs libtools.a tools.o <other_modules>
```

3. Link Libraries when building code :

```
c++ -std=c++17 main.cpp -L . -ltools -o main
```

4. Run the code : 

```
./main
```
### Method 2

#### Using CMake

1. Make a **CMakeLists.txt** in your project folder.
2. Check out <a href="first_library/CMakeLists.txt">this</a>
3. 

```
mkdir build
cd build
ls
cmake . .
make
```