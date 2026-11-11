# termkes

A custom Termux APT repository hosting pre-built packages (`bash`, `apt`, and more) across `aarch64`, `arm`, `i686`, and `x86_64` architectures.

## How to Add This Repository to Termux

You can add this repository to your Termux setup by following these steps:

1. **Install required packages** (if not already installed):
```bash
pkg update && pkg install apt gnupg
```

2. **Add the repository source list**:
Create a custom source entry in your sources list directory:
```bash
echo "deb https://yoshiro2017.github.io/termkes/ stable main" > $PREFIX/etc/apt/sources.list.d/termkes.list
```

4. **Update and install packages**:
```bash
pkg update
pkg install bash
```

## Repository Layout
All packages, package indices (`Packages`, `Packages.gz`), and metadata (`Release`) are hosted directly in the root directory of the <code>main</code> branch for streamlined deployment.
