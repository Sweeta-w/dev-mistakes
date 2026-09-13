---
title: "Difference between pip and !pip in Jupyter / Colab"
category: "Python"
date: "2026-09-13"
---

## 📌 Problem Overview
pip: System terminal command used to install Python packages.

!pip: Jupyter/Colab shell escape command to run pip from inside a notebook cell.

## ✅ Solution & Prevention
%pip install: Best practice command in notebooks that guarantees installation directly into your active Python kernel.

## 💻 Code Example
```python
# ❌ Can install package in base environment instead of active kernel
!pip install numpy

# ✅ Recommended: Safely installs into current active Jupyter kernel
%pip install numpy
```
