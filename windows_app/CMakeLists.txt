cmake_minimum_required(VERSION 3.10)
project(WindowsApp)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 指定使用 MinGW 工具链
set(CMAKE_C_COMPILER x86_64-w64-mingw32-gcc)
set(CMAKE_CXX_COMPILER x86_64-w64-mingw32-g++)
set(CMAKE_RC_COMPILER x86_64-w64-mingw32-windres)

# Windows 可执行文件后缀名
set(CMAKE_EXECUTABLE_SUFFIX ".exe")

# 添加可执行文件
add_executable(WindowsApp main.cpp)

# 如果有静态库需要链接，可以在这里添加
# target_link_libraries(WindowsApp PRIVATE your_library)
