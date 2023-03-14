# Modern CPP 
## By Ignacio Vizzo and Cyrill Stachniss

### Use Modules and libraries

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
