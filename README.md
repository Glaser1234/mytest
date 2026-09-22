# mytest

## Introduction
This is my first test in robomaster.It's about an easiest C++ program.

The ideal output is "Hello,RoboMaster!".

## Environment
- Ubuntu 22.04.5 LTS
- cmake version 3.22.1
- g++ 11.4.0

```bash
#Install Command:
$ sudo apt update
$ sudo apt upgrade -y       %update and upgrade packages in Linux(Ubuntu)
$ sudo apt install -y build-essential cmake git  
```

```bash
#Check your version:
$ lsb_release -a
$ cmake --version
$ g++ --version
$ git --version
```
## Directory Structure
```
hello_cmake/
├── CMakeLists.txt
├── README.md
├── .gitignore
├── Images/
│   └── result1.png
└── src/
    └── main.cpp
```
CMakeLists.txt 描述构建系统规则

Images/result1.png 终端截图

src/ 放置源代码文件main.cpp

build/ 保存缓存，目标文件和程序

## Build System
```bash 
# 编写CMakeLists.txt
cmake_minimum_required(VERSION 3.16)
project(mytest LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_executable(hello src/main.cpp)
```
```bash
#生成build目录，-j并行编译
$ cmake -S . -B build
 cmake --build build -j
```

## Running Result
![result1](Images/result1.png)


```bash
#building success:
-- Building files have been written to: /home/robot/文档/mytest/build 
```
```bash
[100%] Built target hello
```
### **output of C++ program:**
`Hello RoboMaster!`

## Author&Date
```
姓名：林国伟
学号：2255116042
日期：2026年9月22日
```
