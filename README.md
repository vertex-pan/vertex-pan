# Hi there, I'm Irvan Prastyo 👋
### Game Server Developer & Fullstack Game Ecosystem Architect 🚀

I specialize in building end-to-end ecosystems for game servers, with a deep focus on **ARK: Survival Evolved (ASE)** and **ARK: Survival Ascended (ASA)**. I develop high-performance C++ server plugins, robust Laravel web dashboards, cross-platform mobile apps (Flutter), and interactive Discord bots to connect players, server managers, and in-game states.

---

### 🛠️ Languages & Technologies

<table>
  <tr>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/cpp/cpp.png" width="48" height="48" alt="C++" />
      <br>C++
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/php/php.png" width="48" height="48" alt="PHP" />
      <br>PHP
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/dart/dart.png" width="48" height="48" alt="Dart" />
      <br>Dart
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" width="48" height="48" alt="JavaScript" />
      <br>JavaScript
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" width="48" height="48" alt="Python" />
      <br>Python
    </td>
  </tr>
  <tr>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/laravel/laravel.png" width="48" height="48" alt="Laravel" />
      <br>Laravel
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/flutter/flutter.png" width="48" height="48" alt="Flutter" />
      <br>Flutter
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/nodejs/nodejs.png" width="48" height="48" alt="Node.js" />
      <br>Node.js
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/mysql/mysql.png" width="48" height="48" alt="MySQL" />
      <br>MySQL
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/git/git.png" width="48" height="48" alt="Git" />
      <br>Git
    </td>
  </tr>
</table>

* **Languages:** C++, PHP, Dart, JavaScript (Node.js), Python, SQL
* **Web Frameworks:** Laravel (MVC), Tailwind CSS, DaisyUI, Vite, Blade templating
* **Mobile Technologies:** Flutter SDK, Android SDK, iOS SDK, WebView session-bridge integrations
* **Specialized APIs & Integrations:** Steam API/OpenID, PayPal SDK, Sociabuzz Payment Gateway Webhook, RCON Protocol
* **Tools & Server Management:** Ark Server API (C++ hooking), Ark Server Manager (ASM), Git, Visual Studio

---

### 📂 Highlighted Projects

#### 🎮 [Loka Laravel Dashboard](https://github.com/vertex-pan/loka-laravel-dashboard) (Web Ecosystem Portal)
*A premium Web UI dashboard and payment integration platform for game servers.*
* **Tech Stack:** PHP (Laravel), Tailwind CSS & DaisyUI, Vite, JavaScript, MySQL, Steam OpenID
* **Key Features:**
  * **Secure Steam Integration:** Login using Steam ID 64 with automatic user registration linked to active in-game profiles.
  * **Dual Gateway Payment System:** Integrated with **Sociabuzz** (for local Indonesian payment options like QRIS, GoPay, OVO, DANA) and **PayPal** (for international credit card payments). Automated webhook handler securely updates timed VIP membership permissions via SQL transaction locks.
  * **Game & Store Integrations:** Fully custom-built item shop (`/shop`) communicating directly with database servers via AJAX. Items purchased trigger dynamic in-game item delivery via RCON commands and backend task runner queues.
  * **Interactive Tools & Real-Time Stats:** Interactive live maps (Leaflet), online player count trackers, and server status cards pulling dynamic data directly from local servers.
  * **Advanced Admin Impersonation:** Secure Signed URL-based bypass login for administrators to troubleshoot and experience the portal from a player's perspective.

#### 📱 [LokaGamers Mobile Client](https://github.com/vertex-pan/LokaGamers) (Cross-Platform Mobile App)
*A high-performance companion app for players, built with Flutter.*
* **Tech Stack:** Dart, Flutter SDK, WebViewCookieManager, Shared Preferences
* **Key Features:**
  * **Native Authentication & Auto-Login:** Stores session cookies locally and uses an active session injection system to log players into embedded WebViews (e.g., Live Map and Leaderboards) without re-authenticating.
  * **Game Utilities (Loka Tools):** Native screens for Wild Dino Finder (featuring search limits and autocomplete fields), live Tribe Log viewer with multi-server keyword filter, and Server Status checker.
  * **Remote Commands:** RCON-integrated client controls allowing users to trigger live game commands (e.g., instant "Kill Me" command when stuck).
  * **In-App Shop:** Clean, Material Design 3-inspired native catalog for purchasing store items, managing cloud inventories, and sending items instantly to the game cluster.

#### 🧩 C++ Server Plugins (Ark Server API Hooking)
*Low-level, high-performance plugin systems written in native C++ to hook into game engines.*
* **LokaCrossChat:** A robust C++ plugin that hooks into the game chat commands and coordinates cross-server communications, allowing cluster-wide chat sync in real time.
* **LokaCloud:** A custom cloud inventory and storage utility synchronizing player inventories with external databases securely.
* **Notifier-Loka-System:** Event detection plugin that monitors server-side occurrences (like genesis space biomes, specific spawn events, and extinction cycles) and coordinates with external APIs to broadcast alerts.
* **LokaPVPZone / LokaRoyaleZone:** C++ systems managing custom gameplay zones, dynamically adjusting game damage parameters, and automating arena event boundaries.

#### 🤖 ARK-Loka-BOT (Discord Automation)
*A custom Node.js bot for Discord automation and server monitoring.*
* **Tech Stack:** JavaScript, Node.js, Discord.js, RCON client
* **Key Features:**
  * Real-time server status polling and broadcast to specific Discord status channels.
  * Integration with RCON to run server checks, manage channel structures, and display server rates.

---

### 📈 GitHub Stats

<p align="left">
  <img src="https://github-stats-extended.vercel.app/api?username=vertex-pan&show_icons=true&theme=material-palenight" alt="GitHub Stats" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=vertex-pan&layout=compact&theme=material-palenight&langs_count=6" alt="Top Languages" />
</p>

---

*“Bridging the gap between low-level game engines and modern web/mobile experiences.”*  
📬 Feel free to connect with me if you're interested in server backend integrations, C++ game plugins, or custom gaming companion apps!
