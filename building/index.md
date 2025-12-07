---
title: Toucanix Official Building Guide
layout: default
---

<link rel="stylesheet" href="/assets/css/theme.css">

> **Note:** All tools are intended for Ubuntu 20.04.x LTS.  
> Windows users **must** use WSL with Ubuntu 20.04.

---

## Windows Users (WSL)

### Step 1 — Install Ubuntu 20.04 LTS

1. Open the Microsoft Store  
2. Search for **Ubuntu 20.04 LTS**  
3. Install it and complete first-time setup (username/password)

### Step 2 — Install build tools

Inside your WSL terminal:

```sh
cd /path/to/Toucanix
make install_required
```

### Step 3 — Build & Run

Inside your WSL terminal:

```sh
make
```

---

## Linux Users (Native Linux)
### Step 1 — Install build tools

Inside your terminal:

```sh
cd /path/to/Toucanix
make install_required
```

### Step 2 — Build & Run
```sh
make
```

---

## Universal Commands
### Clean
```sh
make clean
```

### Build
```sh
make build
```

### Run
```sh
make run
```

### Install Required Tools
```sh
make install_required
```

### Allow All Shell Scripts
```sh
make chmod_all
```

### Reset OVMFbin
This is to fix that silly bug where QEMU decides to not boot.

```sh
make reset_ovmf_bin
```

### Build & Reset OVMFbin & Run (shortcut)
```sh
make
```

### Clean & Build & Reset OVMFbin & Run (shortcut)
```sh
make ultra
```
