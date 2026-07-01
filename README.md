# Hi there, I'm Irvan Prastyo 👋

<p align="left">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F59E0B&width=450&lines=Game+Server+Developer;C%2B%2B+Server+Plugin+Engineer;Laravel+Fullstack+Developer;Flutter+Mobile+App+Builder;ARK+Ecosystem+Architect" alt="Typing SVG" />
  </a>
</p>

![Profile Views](https://komarev.com/ghpvc/?username=vertex-pan&color=orange&style=flat-square)

I specialize in building end-to-end ecosystems for high-traffic game servers, with a deep focus on **ARK: Survival Evolved (ASE)** and **ARK: Survival Ascended (ASA)**. My work spans low-level game engine hooking in C++, high-performance companion mobile apps (Flutter), robust web administration portals (Laravel), automation bots (Node.js), and asset extraction pipelines (Python).

---

### 🌐 Live Ecosystem Status
[![Website](https://img.shields.io/badge/Website-lokagamers.com-orange?style=for-the-badge&logo=laravel)](https://lokagamers.com/)
[![Android App](https://img.shields.io/badge/Android_App-In_Development-blue?style=for-the-badge&logo=android)](#)

---

### 🏛️ System Architecture

Here is the complete data flow, integration pipeline, and hardware administration map of the game server ecosystem:

```mermaid
graph TD
    classDef default fill:#1e1e24,stroke:#444,stroke-width:2px,color:#fff;
    classDef highlight fill:#f59e0b,stroke:#d97706,stroke-width:2px,color:#000;
    classDef storage fill:#2563eb,stroke:#1d4ed8,stroke-width:2px,color:#fff;

    subgraph Infrastructure [Server Nodes Layout]
        MainNode[Main Server: Intel Xeon]
        TestNode[Tester Server: AMD EPYC]
        SupportNode[Support Server: Intel Xeon VM]
    end

    subgraph Game_Cluster [ARK Game Server Node]
        ASM[ARK Server Manager - ASM] -->|Administers & Deploys| GameServer[ARK Game Process]
        GameServer <-->|Low-Level Hooks| Plugins[C++ Plugins: CrossChat, LokaCloud, Notifier, PVPZone]
    end

    subgraph Data_Extraction [Asset Extraction Pipeline]
        Assets[(ARK Game Files .uasset)] -->|Reads Assets| Purlovia[Purlovia Python Extractor]
        Purlovia -->|Generates JSON & Rates Config| Configs[Static Configs & rates.ini]
    end

    subgraph Database [Database Layer]
        MySQL[(MySQL Databases)]
    end

    subgraph Web_Services [Web Backend & Management]
        Laravel[Loka Laravel Dashboard]
        Gateways[PayPal & Sociabuzz APIs] -->|Automated Webhooks| Laravel
    end

    subgraph Clients [User Interfaces]
        Flutter[Flutter Mobile Client]
        Discord[Discord Bot]
    end

    %% Communications
    Configs -->|Served by Web / Whitelisted URL| Laravel
    GameServer -->|Downloads rates.ini| Configs
    Plugins <-->|Live SQL Stacking & Player Data| MySQL
    Laravel <-->|Eloquent ORM & Web State DB| MySQL
    Laravel -->|RCON Command Delivery| GameServer
    Flutter <-->|REST API & WebView Session Bridge| Laravel
    Discord <-->|RCON Status Polling & Chat Broadcast| GameServer

    %% Styling
    class Laravel,Flutter,Plugins highlight;
    class MySQL,Assets storage;
```

---

### 🛠️ Languages & Technologies

<table>
  <tr>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/cpp/cpp.png" width="48" height="48" alt="C++" />
      <br>C++
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/php/php.png" width="48" height="48" alt="PHP" />
      <br>PHP
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/dart/dart.png" width="48" height="48" alt="Dart" />
      <br>Dart
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" width="48" height="48" alt="JavaScript" />
      <br>JavaScript
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" width="48" height="48" alt="Python" />
      <br>Python
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/windows/windows.png" width="48" height="48" alt="Windows Batch" />
      <br>Batch / Cmd
    </td>
  </tr>
  <tr>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/laravel/laravel.png" width="48" height="48" alt="Laravel" />
      <br>Laravel
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/flutter/flutter.png" width="48" height="48" alt="Flutter" />
      <br>Flutter
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/nodejs/nodejs.png" width="48" height="48" alt="Node.js" />
      <br>Node.js
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/mysql/mysql.png" width="48" height="48" alt="MySQL" />
      <br>MySQL
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/tailwind/tailwind.png" width="48" height="48" alt="Tailwind CSS" />
      <br>Tailwind / DaisyUI
    </td>
    <td align="center" width="110">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/git/git.png" width="48" height="48" alt="Git" />
      <br>Git
    </td>
  </tr>
</table>

*   **Core Languages:** C++, PHP, Dart, JavaScript (Node.js), Python, SQL, Windows Batch Scripting (`.bat` / `.cmd`)
*   **Web Frameworks & Libraries:** Laravel (MVC), Tailwind CSS v4, DaisyUI, Leaflet.js (Interactive Maps), Blade Templating, Vite
*   **Mobile Technologies:** Flutter SDK, Android SDK, WebView (with Session/Cookie Injector)
*   **Protocols & APIs:** RCON Protocol (Game Server Remote Execution), Steam OpenID / Web API, PayPal Checkout SDK, Sociabuzz Payment Gateway Webhooks
*   **Game Engine Integration:** Ark Server API (C++ Hooking), Unreal Engine Asset Extractor (uasset serialization & schema parsing)
*   **Dev Tools & Environments:** Visual Studio (MSBuild), VS Code, npm, Composer, Git/GitHub, Ark Server Manager (ASM)

---

### 📂 Highlighted Projects

#### 🎮 [Loka Laravel Dashboard](https://github.com/vertex-pan/loka-laravel-dashboard) (Web Ecosystem Portal)
*A high-end player web portal and automated billing system for game server clusters.*
*   **Tech Stack:** PHP (Laravel), Tailwind CSS & DaisyUI, Vite, JavaScript, MySQL, Steam OpenID
*   **Key Features:**
    *   **Secure Steam Integration:** Direct authentication using Steam ID 64 with automatic database profiling linked to live game characters.
    *   **Automated Payment Gateways:** Dual checkout integration featuring **Sociabuzz** (for local Indonesian payment channels: QRIS, GoPay, OVO, DANA, Virtual Accounts) and **PayPal** (for international credit cards). Features automated webhook processing with SQL locking to manage timed VIP tier stacking.
    *   **Item Store & Cloud Delivery:** Custom-built shop `/shop` querying live databases. Purchases automatically generate RCON item delivery queues (extracting blueprint paths, parameters, and count) dispatched directly to active servers.
    *   **Server Monitoring:** Live Leaflet.js interactive maps, real-time online player counters, and server status cards caching query ports asynchronously.
    *   **Admin Impersonation:** Secure Signed URL-based bypass login allowing server admins to audit dashboard interactions from any player's perspective.

#### 📱 [LokaGamers Mobile Client](https://github.com/vertex-pan/LokaGamers) (Cross-Platform Mobile App)
*A dedicated mobile application companion for players to manage their characters and track servers.*
*   **Tech Stack:** Dart, Flutter SDK, WebViewCookieManager, Shared Preferences
*   **Key Features:**
    *   **WebView Cookie Bridge:** Native login screen saving session cookies locally. It uses `WebViewCookieManager` to inject active sessions into embedded WebViews (Live Map & Leaderboards) to bypass web re-authentication.
    *   **In-App Game Utilities:** Native screens for autocomplete Wild Dino Finder (with daily query quotas), live multi-server Tribe Log viewer with keyword filtering, and Server Status cards.
    *   **Remote RCON Execution:** Interactive commands allowing players to trigger actions like instant "Kill Me" to unstuck characters from their mobile device.
    *   **Mobile Item Shop:** Full native UI catalog for store items, purchase checkout, and cloud inventory management to send stored items instantly to in-game characters.

#### 🧩 C++ Server Plugins (Ark Server API Hooking)
*Low-level, high-performance C++ DLLs hooking into the server executable to inject custom logic.*
*   **LokaCrossChat:** Hooks into server chat events to synchronize chat messages across multiple game servers in the cluster in real time.
*   **LokaCloud:** Custom server database synchronizer storing player inventory data safely into external MySQL servers.
*   **Notifier-Loka-System:** Detects in-game world events (e.g., Space Biome changes, Dino spawn events, Extinction cycles) and uses webhooks to broadcast them to external networks.
*   **LokaPVPZone & LokaRoyaleZone:** Dynamic arena zone management adjusting actor damage multipliers and boundary logic.

#### 🤖 ARK-Loka-BOT (Discord Automation)
*A custom Node.js bot for Discord automation and server monitoring.*
*   **Tech Stack:** JavaScript, Node.js, Discord.js, RCON Client
*   **Key Features:**
    *   Real-time server stats reporting, role synchronization based on VIP purchases, and automated RCON command executors for moderators.

---

### 🖥️ Infrastructure & Cluster Specs

Since I manage high-traffic game clusters (including automation, backups, and live player data sync), here is the technical infrastructure stack and dedicated server nodes I administer:

| Server Node | Operating System | CPU Processor | Installed RAM | Hardware / Motherboard |
| --- | --- | --- | --- | --- |
| **Main Production** | Windows Server 2022 Std | Intel Xeon E-2388G @ 3.20GHz (8C/16T) | 64.0 GB | ASRockRack E3C252D4U-2T/OVH |
| **Tester & Dev** | Windows Server 2022 Std | AMD EPYC 4344P @ 3.80GHz (8C/16T) | 64.0 GB | ASRockRack B650D4U |
| **Support & Utility** | Windows 10 Pro | Intel Xeon E5-2698 v4 @ 2.20GHz (8 Cores) | 32.0 GB | VMware Virtual Machine |

#### 🛠️ Technology Stack
*   **Cluster Management:** ARK Server Manager (ASM)
*   **Low-Level Hooking:** ARK Server API (DLL Plugin System)
*   **Database Architecture:** MySQL (Dual-connection setups for live state & web state)
*   **Command Delivery:** Native RCON Protocol Remote Execution

---

### 📲 Connect with LokaGamers
[![Website](https://img.shields.io/badge/Website-lokagamers.com-blue?style=for-the-badge&logo=google-chrome&logoColor=white)](https://lokagamers.com/)
[![Discord](https://img.shields.io/badge/Discord-Join_Hub-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/lokagamers)
[![Facebook](https://img.shields.io/badge/Facebook-lokagamers-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](http://facebook.com/lokagamers)
[![Instagram](https://img.shields.io/badge/Instagram-lokagamers-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](http://instagram.com/lokagamers)
[![X](https://img.shields.io/badge/X-lokagamers-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/lokagamers)
[![YouTube](https://img.shields.io/badge/YouTube-@lokagamersofficial-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@lokagamersofficial)
[![TikTok](https://img.shields.io/badge/TikTok-@lokagamers-000000?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@lokagamers)

---

### 📈 GitHub Stats

<p align="left">
  <img src="https://github-stats-extended.vercel.app/api?username=vertex-pan&show_icons=true&theme=material-palenight" height="195" alt="GitHub Stats" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=vertex-pan&layout=compact&theme=material-palenight&langs_count=6" height="195" alt="Top Languages" />
</p>

<p align="left">
  <img src="https://streak-stats.demolab.com/?user=vertex-pan&theme=material-palenight" height="195" alt="GitHub Streak Stats" />
</p>

---

*“Bridging the gap between low-level game engines and modern web/mobile experiences.”*  
📬 Feel free to connect with me if you're interested in server backend integrations, C++ game plugins, or custom gaming companion apps!
