请务必使用这条命令进行编译`pwsh.exe -c './env.ps1 cmake --build --preset conan-release --parallel'`

conan install . --build=missing --output-folder=build

cmake --preset conan-default

cmake --build --preset conan-release --parallel