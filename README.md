**English** | [日本語](README.jp.md)

# RocketToolbox 🚀🛠️🧰
A Julia toolbox of standard utilities for aerospace calculation and analysis

_In development since 2026 Jan 22_

> ### ⚠️ Project status
>
> **Author.** RocketToolbox was written by **Joel T Harter** as its sole author, during his
> employment at Interstellar Technologies.
>
> **This repository is not actively maintained.** The author left Interstellar Technologies
> on **13 August 2026**. No maintainer has taken over here, and Interstellar Technologies
> has no current plans to continue development in this repository — issues and pull requests
> opened against it should not be expected to get a response.
>
> **Active development continues in the author's own fork:
> [github.com/JoelHarter/RocketToolbox](https://github.com/JoelHarter/RocketToolbox)**, which
> he intends to keep maintaining. Use that one if you want the living version; use this one if
> you specifically need the state of the code as of the author's departure.

## Overview

### 📐 Constants Library
* Unit conversions
* Physical constants
* Earth and Astronomical parameters

### 🌏 Functions for transforming between coordinate frames
* Geodetic (Geo)
* Earth-Centered Earth-Fixed (ECEF)
* Earth-Centered Inertial (ECI)

### 🔄 Quaternions and Rotations
* Quaternion object definition
* Constructors for 2D, 3D principal axis, and 3D general rotation matrices

### 👽 And much more!

## Setup

### Install Packages
Julia:
```
using Pkg
Pkg.add("StaticArrays")
```

### Use in your code
Julia:
```julia
# include.jl is the single entry point — include it once to load everything.
include("[path to repo]/include.jl")
```

All functions, types, and constants are loaded into the current scope.
No module qualifiers needed: use `Earth.μ`, `Quat(...)`, `rotmat(...)`, etc. directly.