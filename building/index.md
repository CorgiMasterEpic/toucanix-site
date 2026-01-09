---
title: Toucanix Official Building Guide
layout: default
---

> **Note:** All tools are intended for Ubuntu 20.04.x LTS.  
> Windows users **should** use WSL with Ubuntu 20.04.x for errorless installs
> Linux users **should** also use ubuntu 20.04.x for errorless installs

---

### Step 1 — Install Ubuntu 20.04 LTS (Linux users skip to step 2)

1. Open the Microsoft Store  
2. Search for **Ubuntu 20.04 LTS**  
3. Install it and complete first-time setup (username/password)

### Step 2 — Install build tools

Inside your terminal:

```sh
cd /path/to/Toucanix
./Build/Scripts/install_dependencies.sh
```

### Step 3 — Build & Run

Inside your terminal:

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
