# 💻 CEA Offline

## 🧭 Overview
**CEA Offline** is a standalone Windows application built using **C#**, **SQL Server**, and **Visual Studio**. It was developed to serve as an offline backup presentation tool for director meetings at AHMSA. When network connectivity fails or is unavailable, this application allows seamless access to purchase approval sessions by loading data and media from local storage.

The system mirrors the user experience of **CEA Web**, ensuring continuity during executive committee reviews.

## 💡 Idea & Concept
CEA Offline was created to guarantee uninterrupted Monday procurement committee meetings by:
- Exporting session data and images from CEA
- Allowing system admins to manually prepare offline assets
- Presenting sessions in a PowerPoint-style, branded format

## ✨ Features & Functionality
- 🗂 Load Local Session:
  - Excel sheet with session metadata
  - Folder of PNG images with vendor comparison tables
- 🖥 Presentation Mode:
  - Full-screen, clean interface optimized for projection
  - Step-by-step slide view per case (title, description, image)
- 🧭 Session Selector:
  - Lists sessions available in `C:\CEA\[SessionDate]`
- 🔄 Navigation:
  - Next/Previous case slide buttons
- 💾 Offline Execution:
  - No network or database access required
- 🎯 Identical UI to CEA Web for consistency

## ⚙️ Tech Stack
| Category                | Tools & Frameworks |
|-------------------------|--------------------|
| **Frontend**            | ![WinForms](https://img.shields.io/badge/WinForms-512BD4?logo=.net&logoColor=white&style=for-the-badge) |
| **Backend**             | ![C#](https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white&style=for-the-badge) |
| **Platform**            | ![Windows App](https://img.shields.io/badge/Windows%20App-0078D4?logo=windows&logoColor=white&style=for-the-badge) |
| **Framework**           | ![.NET Framework](https://img.shields.io/badge/.NET%20Framework-512BD4?logo=.net&logoColor=white&style=for-the-badge) |
| **IDE**                 | ![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?logo=visualstudio&logoColor=white&style=for-the-badge) |
| **Database**            | ![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?logo=microsoft-sql-server&logoColor=white&style=for-the-badge) |
| **Cloud & Hosting** | ![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D4?logo=windows&logoColor=white&style=for-the-badge) ![IIS](https://img.shields.io/badge/IIS-0078D7?logo=microsoft&logoColor=white&style=for-the-badge) |
| **Security & Identity** | ![Custom Auth](https://img.shields.io/badge/Custom%20Auth-000000?style=for-the-badge&logo=key&logoColor=white) |

## 🏗 Architecture & Design
- Reads `.xlsx` and `.png` files exported by CEA system
- Each case rendered using pre-designed layouts
- No login or role-based access needed (read-only tool)

## 🚀 Installation & Setup
- **Setup Path:** `C:\CEA\[SessionName]`
- **Contents Required:** Excel + image files
- **User:** Executed by system admin on dedicated Windows machine

> **Note:** System Admin must export session before Monday meeting.

## 🧑‍💻 My Role & Contributions
- 💼 Designed and implemented the full offline workflow
- 📦 Integrated session parser and offline media loader
- 🎯 Ensured full visual parity with CEA Web
- 🧪 QA testing and user simulation for emergency scenarios

## 🧗 Challenges & Learnings
- Ensured app runs without SQL or internet
- Built dynamic renderer based on local content
- Created fallback mechanism for session errors
- Matched corporate branding under limited constraints

## 📈 Future Enhancements
- One-click export bundle from CEA Admin
- Cloud download sync when internet resumes
- Annotated slide mode for meeting presenters

## 🪪 License
⚠️ **Internal Use Only**  
Originally under MIT License; changed to **CC BY-NC-ND 4.0** as of April 22, 2025.

## 🔗 Related Projects
- **[CEA](https://github.com/HermiloOrtega/CEA)**
- **[CEA Web](https://github.com/HermiloOrtega/CEA-Web)**
- **[CEA Offline](https://github.com/HermiloOrtega/CEA-Offline)**
