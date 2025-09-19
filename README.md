
# starter-cpp

Starter project for modern C++ development using Bazel and CMake, with optional Python bindings, automated linting, documentation, and CI/CD integration.

[![Build Status](https://github.com/your-org/starter-cpp/actions/workflows/ci.yml/badge.svg)](https://github.com/your-org/starter-cpp/actions/workflows/ci.yml)
[![Lint Status](https://github.com/your-org/starter-cpp/actions/workflows/lint.yml/badge.svg)](https://github.com/your-org/starter-cpp/actions/workflows/lint.yml)
[![Docs Status](https://github.com/your-org/starter-cpp/actions/workflows/docs.yml/badge.svg)](https://github.com/your-org/starter-cpp/actions/workflows/docs.yml)
[![License](https://img.shields.io/github/license/your-org/starter-cpp)](LICENSE)

---

## Features

- Modern C++17/20 codebase
- Dual build system support: Bazel and CMake
- Python bindings with `pybind11`
- Automated linting with `clang-format`, `clang-tidy`, and `pre-commit`
- Unit testing with Google Test
- Documentation via Doxygen
- GitHub Actions CI/CD
- Python wheel builds for packaging
- Security audits with OSSF Scorecard and Dependabot

---

## Project Structure

```

starter-cpp/
├── src/              # C++ source files
├── include/          # Public headers
├── test/             # Unit tests
├── bindings/         # Python bindings (pybind11)
├── docs/             # Documentation (Markdown + Doxygen)
├── cmake/            # CMake modules
├── bazel/            # Bazel dependencies
├── tools/            # Helper scripts or Bazel tools
├── .github/          # GitHub Actions workflows and issue templates

````

---

## Getting Started

### Requirements

- C++17 or later
- Bazel ≥ 6.x
- CMake ≥ 3.20
- Python ≥ 3.8
- Optional: `clang-format`, `clang-tidy`, `pre-commit`

### Build with Bazel

```bash
bazel build //...
bazel test //...
````

### Build with CMake

```bash
mkdir -p build && cd build
cmake ..
cmake --build .
ctest
```

---

## Python Bindings

To build and install the Python module:

```bash
pip install .
```

To verify:

```bash
python -c "import project; print(project.hello())"
```

---

## Documentation

To generate local Doxygen docs:

```bash
doxygen Doxyfile
```

Documentation is also generated in CI and available in the `docs/` directory.

---

## Pre-commit Hooks

```bash
pip install pre-commit
pre-commit install
pre-commit run --all-files
```

---

## Security

This project uses:

* [OSSF Scorecard](https://github.com/ossf/scorecard)
* [Dependabot](https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically)

---

## Contributing

We welcome contributions!

* [CONTRIBUTING.md](CONTRIBUTING.md)
* [CODE\_OF\_CONDUCT.md](CODE_OF_CONDUCT.md) *(if available)*

---

## License

Licensed under the [MIT License](LICENSE).

---

## Acknowledgments

Thanks to all [contributors](CONTRIBUTORS) and [authors](AUTHORS).


