# Dr. Leaf - Plant Disease Detection Model

[![Platform: Windows / WSL](https://img.shields.io/badge/platform-Windows%20%2F%20WSL-blue)](https://learn.microsoft.com/en-us/windows/wsl/)
[![Tooling: Visual Studio](https://img.shields.io/badge/Tooling-Visual%20Studio-purple.svg?logo=visual-studio)](https://visualstudio.microsoft.com)
[![Engine: Unreal Engine 4.27](https://img.shields.io/badge/Engine-Unreal%20Engine%204.27-black.svg?logo=unreal-engine)](https://www.unrealengine.com/)

A foundational software engineering project focused on configuring, debugging, and optimizing the local compilation pipelines and development environments for the **Dr. Leaf** ecosystem. This repository documents the source-build environment configurations, automated build orchestration, and deep IDE workflows required to handle heavy graphic engine assets alongside deep learning architectures.

---

## 🚀 Key Engineering Focus Areas

* **Pipeline Automation:** Executed and tested automated batch processing configurations using `.bat` orchestration routines (`GenerateProjectFiles.bat`) to dynamically map system headers and clean up dependency trees.
* **Environment Architecture:** Configured native **Visual Studio** workspaces to reliably index and manage heavy project state files, custom compiler flags, and build targets matching **Unreal Engine 4.27** specifications.
* **Cross-Platform Bridge:** Structured local paths and environment variables to seamlessly bridge Windows-based developer tools with Linux-centric machine learning frameworks via WSL (Windows Subsystem for Linux).

---

## 🛠️ Tech Stack & Tooling

* **IDE / Compiler:** Visual Studio, MSBuild
* **Engine Architecture:** Unreal Engine 4.27 (Source-build pipeline)
* **Scripting & Automation:** Windows Batch (`.bat`), Command Line Interface
* **Compatibility Layer:** WSL (Windows Subsystem for Linux)

---

## 💡 Technical Challenges Overcome

### 🔧 IDE Solution Generation & Synchronization Faults
* **Problem:** The automation runner failed during execution, causing compilation blockages where Visual Studio could not display the target `.sln` icon or bind to newly initialized source assets.
* **Solution:** Diagnosed the registry and variable path discrepancies, repaired the broken compiler-to-IDE handshakes, and manually forced a clean re-generation of the project metadata. This fully restored solution file visibility, indexing, and stable compilation trees.

---

## ⚙️ Quick Start & Setup

### Prerequisites
* Windows 10/11 with WSL installed
* Visual Studio (with C++ game development workloads)
* Unreal Engine 4.27 Source

### Environment Initialization
1. Clone the repository to your local workspace.
2. Double-click and execute the orchestration batch file:
   ```bash
   GenerateProjectFiles.bat
