---
title: "CHECKING PC CAPABILITY FOR LOCAL AI"
category: "General"
date: "2026-09-22"
---

## 📌 Problem Overview
Check your PC's RAM, CPU, GPU/VRAM, and storage to determine whether it can run AI models locally.

## ✅ Solution & Prevention
────────────────────────────────────────────
⭐ WHAT TO LOOK FOR
────────────────────────────────────────────

RAM:
16 GB+ → Good
8 GB → Limited
4 GB → Not recommended

GPU/VRAM:
8 GB+ dedicated VRAM → Good for many local AI models
4 GB → Limited
Integrated GPU → Can run some small models, but limited

Storage:
20–50 GB+ free → Recommended for models and tools

## 💻 Code Example
```bash
1. systeminfo
   → Provides:
   - Operating system information
   - CPU/processor information
   - Total physical RAM
   - System details

2. wmic path win32_VideoController get name,AdapterRAM
   → Provides:
   - GPU name
   - GPU memory (VRAM)

3. wmic logicaldisk get caption,freespace,size
   → Provides:
   - Available storage
   - Total storage

────────────────────────────────────────────
🍎 macOS
────────────────────────────────────────────

1. system_profiler SPHardwareDataType
   → Provides:
   - Mac model
   - CPU/chip (e.g., Apple M1/M2/M3)
   - RAM/unified memory

2. system_profiler SPDisplaysDataType
   → Provides:
   - GPU/graphics processor
   - Graphics memory information

3. df -h
   → Provides:
   - Available storage
   - Used storage
   - Total storage
```
