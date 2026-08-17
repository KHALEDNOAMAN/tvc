# Build & Setup Guide

## Prerequisites
- C++ compiler (GCC 11+ or Clang 14+)
- CMake 3.20+
- Git

## Quick Build
```bash
git clone https://github.com/mamadou-wane/tvc.git
cd tvc
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
make -j$(nproc)
```

## Project Structure
```
tvc/
├── src/           # Source files
├── include/       # Header files
├── tests/         # Unit tests
├── docs/          # Documentation
├── CMakeLists.txt # Build configuration
└── README.md
```

## Running Tests
```bash
cd build
ctest --output-on-failure
```

## Contributing
1. Fork the repository
2. Create feature branch: `git checkout -b feature/my-feature`
3. Commit changes: `git commit -am 'Add feature'`
4. Push: `git push origin feature/my-feature`
5. Open Pull Request

## Debugging
```bash
cmake .. -DCMAKE_BUILD_TYPE=Debug
make
gdb ./tvc_app
```
