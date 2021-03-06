# NanoSTL, a small subset of C++ STL.

NanoSTL is good for using STL-like feature in your C++ application and C++-like JIT compiler.

## Status

Eearly testing stage. Not ready for the production use.

## Supported features

Be careful! Not all C++ STL functions are supported for each module.

* vector
* string
* algorithm
* limits
* map

## Supported architectures

* 64bit and 32bit machine.

## Supported compilers

Even though NanoSTL can be compilable with old and various C++ compilers, at least following compilers works well.

* gcc 4.8.x+
* clang 3.4+

## Types

* char : 8bit
* short : 16bit
* int : 32bit
* long long : 64bit
* float : 32bit IEEE754 floating point.
* double : 64bit IEEE754 floating point.

## Differences compared to (full featured) C++ STL

* RTTI and exception is not supported.
* Returns `NULL` when memory allocation failed(no `bad_alloc`)

## TODO

* [ ] CUDA NVRTC support
* [ ] isnan/isinf/isfinite support
* [ ] Unit tests
* [ ] Multithread support
* [ ] Backport of some C++11 features(e.g. `unordered_map`)

## Developer note

### Debugging 

Use `NANOSTL_DEBUG` define for debugging.

## Licenss

MIT license

### Third party licenses

* microtest.h : MIT license.
