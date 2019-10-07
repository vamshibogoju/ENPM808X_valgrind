# Valgrind

## Overview

This is a C++ excercise which uses valgrind tools to check bugs


## Standard install via command-line
```
git clone https://github.com/vamshibogoju/ENPM808X_valgrind
cd <path to repository>
mkdir build
cd build
cmake ..
make
```	

## Valgrind Commands 

Check for bugs:
 valgrind --leak-check=full ./app/shell-app 

Save to a textfile:
 valgrind --log-file=filename --leak-check=full ./app/shell-app 


## KCachegrind 

Commands: 
valgrind --tool=callgrind ./app/shell-app

-callgrind.out file is created 
-run this file to get memory profile

