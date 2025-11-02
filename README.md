# LIMO — ROS Packages

[![License](https://img.shields.io/badge/License-BSD--3--Clause-blue.svg)](LICENSE)
[![ROS](https://img.shields.io/badge/ROS-Noetic-blue)](http://wiki.ros.org/noetic)
[![Build](https://img.shields.io/badge/Build-catkin-green)](#build-from-source-code)

This repository contains ROS packages for **LIMO**.

<p align="center">
  <img src="docs/images/limo_models.png" alt="LIMO models preview" width="680">
</p>

---

## Packages

- **limo_base**: ROS wrapper for LIMO  
- **limo_bringup**: launch & configuration files to start ROS nodes  
- **limo_description**: URDF model for LIMO

---

## Build from source code

Clone the repository and build with `catkin_make`:

```bash
# 1) workspace 준비
mkdir -p ~/catkin_ws/src && cd ~/catkin_ws/src

# 2) 레포 클론
git clone https://github.com/USERNAME/REPO_NAME.git

# 3) 빌드
cd ..
catkin_make

# 4) 환경설정
source devel/setup.bash
