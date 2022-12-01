To build, you need conan, ninja, cmake and a c++ compiler.

```bash
python -m pip install cmake ninja conan
git clone https://github.com/EricAtORS/CMakeBugReport
cd CMakeBugReport
conan install . -if output/conan
cmake -S . --preset=default
cmake --build build/default
```

If you enable conan (the default),  the output goes to ${CMAKE_BINARY_DIR}/bin.
If you disable conan by commenting out the lines 