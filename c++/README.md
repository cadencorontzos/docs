# C++

### Basic Syntax

Functions and command line arguments and reading files
```c++
#include <iostream>
#include <fstream>
#include <chrono>
#include <filesystem>

namespace fs = std::filesystem;

// Here's a comment

/*

Here is a block comment

*/
int main(int argc, char* argv[]){

    if (argc != 2){
        std::cerr<<"Please include the name of the file you would like to compress\n";
        return 1;
    }

    std::ifstream input (argv[1], std::ios::binary);
    if (!input.is_open()){
        std::cout << "Unable to open " << argv[1] << ".\n";
        return 1;
    }

}
```
