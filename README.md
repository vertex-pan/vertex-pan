# Hi there, I'm Irvan Prastyo 👋

<p align="left">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F59E0B&width=450&lines=Game+Server+Developer;C%2B%2B+Server+Plugin+Engineer;Laravel+Fullstack+Developer;Flutter+Mobile+App+Builder;ARK+Ecosystem+Architect" alt="Typing SVG" />
  </a>
</p>

I specialize in building end-to-end ecosystems for high-traffic game servers, with a deep focus on **ARK: Survival Evolved (ASE)** and **ARK: Survival Ascended (ASA)**. My work spans low-level game engine hooking in C++, high-performance companion mobile apps (Flutter), robust web administration portals (Laravel), automation bots (Node.js), and asset extraction pipelines (Python).

---

### 🌐 Live Ecosystem Status
[![Web Portal](https://img.shields.io/badge/Live_Dashboard-Visit_Web-orange?style=for-the-badge&logo=laravel)](http://ark.lokagamers.com)
[![Android App](https://img.shields.io/badge/Android_App-In_Development-blue?style=for-the-badge&logo=android)](#)

---

### 🏛️ System Architecture

Here is how the components of the game server ecosystem communicate and synchronize data:

```mermaid
graph TD
    classDef default fill:#1e1e24,stroke:#333,stroke-width:2px,color:#fff;
    classDef highlight fill:#f59e0b,stroke:#d97706,stroke-width:2px,color:#000;
    
    subgraph Game Server [ARK Server Cluster]
        A[Game Server Process] <-->|Ark Server API Hooking| B[C++ Plugins: LokaCrossChat, LokaCloud, Notifier]
    end
    
    subgraph Database [Database Layer]
        C[(MySQL: Game & Web DB)]
    end
    
    subgraph Web [Web Backend & Portal]
        D[Loka Laravel Dashboard]
    end
    
    subgraph Clients [User Interfaces]
        E[Flutter Mobile Client]
        F[Discord Bot]
    end
    
    subgraph Gateways [Payment Systems]
        G[PayPal & Sociabuzz API]
    end

    B <-->|Live SQL Sync| C
    D <-->|Eloquent ORM & Transaksi| C
    D -->|RCON Commands| A
    E <-->|REST APIs / Cookie Session Bridge| D
    F <-->|RCON status & Chat Broadcast| A
    G -->|Automated Webhooks| D

    class D,E,B highlight;
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

### 📈 GitHub Stats

<p align="left">
  <img src="https://github-stats-extended.vercel.app/api?username=vertex-pan&show_icons=true&theme=material-palenight" alt="GitHub Stats" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=vertex-pan&layout=compact&theme=material-palenight&langs_count=6" alt="Top Languages" />
</p>

---

*“Bridging the gap between low-level game engines and modern web/mobile experiences.”*  
📬 Feel free to connect with me if you're interested in server backend integrations, C++ game plugins, or custom gaming companion apps!
