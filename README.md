# PaiMap

A high-performance interactive mapping application built in C++ using 
OpenStreetMap data. Achieved O(1) spatial queries across 100K+ Toronto 
intersections with all functions executing under 150ms.

> [!WARNING]
> Source code is kept private per course policy (UofT ECE297). This repository contains documentation and visuals only.
>
> 
## Screenshots
<img width="1684" height="1004" alt="image" src="https://github.com/user-attachments/assets/fca899b5-83ed-4dbb-a911-1e334a88ceb0" />

### Map View with POI Filtering
<img width="1681" height="1012" alt="image" src="https://github.com/user-attachments/assets/041b15f3-4708-4f53-b6f4-0d8abc5e6b93" />

### Map View with all Collapsed Menus
<img width="1681" height="1007" alt="image" src="https://github.com/user-attachments/assets/935f6e54-cfeb-4b96-ad00-d4db36306a39" />

### Route Finding 
<img width="1686" height="1008" alt="image" src="https://github.com/user-attachments/assets/264d8aac-1ce4-4cf5-8d97-cd0d9b14addc" />

### Chatbot (Gemini API)
<img width="388" height="287" alt="image" src="https://github.com/user-attachments/assets/6a747cd2-0ef3-4342-874a-81156fdb7fea" />


### Performance Profiling (perf flame graph)
<img width="1370" height="588" alt="image" src="https://github.com/user-attachments/assets/300f0c08-7b38-4f3d-9748-bec1693080ae" />

## Performance Highlights
- Query time: **500ms → 0.2ms** (90%+ reduction via perf profiling)
- **O(1)** intersection lookups using a 160×160 geo-grid index
- Smooth **60fps** zoom and pan across 10+ cities
- **Zero memory leaks** verified across all map datasets
- All required functions execute in **under 150ms**

## Tech Stack
- **Language:** C++, STL
- **Graphics:** EZGL / GTK3 / Cairo
- **Data:** OpenStreetMap APIs
- **Profiling:** perf, Valgrind, Chrono library
- **Version Control:** Git (3-person team)

## Features
- 160×160 geo-grid spatial index for O(1) intersection lookups
- Partial-name search with click-to-highlight intersections
- POI filtering by category (food, medical, transit, etc.)
- Light/dark mode toggle
- Multi-city support
- Integrated "Paimon" travel guide assistant with local recommendations
- Route visualization between any two intersections

## What I Built
- Designed and implemented the geo-grid spatial indexing system
- Led profiling effort using perf flame graphs — identified and 
  eliminated bottlenecks reducing query time by 90%+
- Led the 4-person team using Git with branch management
- Built the partial-name search and click-highlight UI features

## Team
4-person team project — UofT ECE297 (Software Design and Communication)
