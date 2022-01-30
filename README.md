# File Utils

Simple file helper functions for C.


## Quick Start

Copy file_utils.h into your project and include it like this:

``` c++
#define FILE_UTILS_IMPLEMENTATION
#include "file_utils.h"
```
 
This is a stb style header only library. For more information about stb style
headers libraries see [stb_howto.txt](https://github.com/nothings/stb/blob/master/docs/stb_howto.txt)


## Functions

| Function         | Args             | Return Type | Description |
|------------------|------------------|-------------|-----------------------------------------|
| file_count_lines | const char *path | size_t      | Returns total number of lines in a file |
| file_as_str      | const char *path | char *      | Returns file contents as a string       |
| file_as_str_arr  | const char *path | char **     | Returns file contents as array of strings. Array count is file lines + 1. The last element is NULL to allow iteration without needing to store the line count |
