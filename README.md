<p align="right">
  🌐 <img src="https://img.shields.io/badge/EN-0f7a63?style=flat-square" alt="EN (current)"> <a href="README.tr.md"><img src="https://img.shields.io/badge/TR-6e7781?style=flat-square" alt="TR"></a>
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Ayberk Cerit — Software Engineering student building local-first AI" src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://ayberkcerit.github.io/Portfolio_Web/"><img src="https://img.shields.io/badge/Portfolio-0f7a63?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/ayberk-cerit-4707a12a4/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:a2407231005@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://ayberkcerit.github.io/Portfolio_Web/cv.pdf"><img src="https://img.shields.io/badge/CV-24292f?style=for-the-badge&logo=readdotcv&logoColor=white" alt="CV"></a>
</p>

## About me

I'm a third-year **Software Engineering** student at Gümüşhane University in Türkiye, working toward **AI/ML engineering**.
What pulls me in is AI that runs *where the data lives*: on your laptop, on a small device, on a drone. Not in someone else's cloud.

- 🔭 **Building** [PLA](https://github.com/AyberkCerit/personal_life_assistant), an offline personal assistant powered by a local LLM (Rust · Tauri · llama.cpp)
- 🏛️ **Summer 2026:** software development intern at **Bilim A.Ş.**, the technology unit of Konya Metropolitan Municipality, where I built a field audit and task platform on Laravel + Docker
- 🌱 **Learning:** reinforcement learning for autonomous UAVs, image processing, operating systems
- 🤝 **Open to** AI/ML internships and conversations about on-device AI

## Featured: PLA, a personal assistant that never leaves your machine

Notes, tasks, reminders and health metrics in one desktop app, **fully offline**.
The AI is not a chatbot bolted onto the side. It works in the background: it reads what you write and quietly turns it into tasks, reminders and metrics. When you ask, it answers from your own notes.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/pla-pipeline-dark.svg">
  <img alt="PLA pipeline: Markdown note → changed blocks → Gemma 4 on-device extraction → validation in Rust → tasks, reminders, metrics" src="assets/pla-pipeline-light.svg" width="100%">
</picture>

<table>
  <tr>
    <td width="27%" valign="top">🧪 <b>Model chosen by measurement</b></td>
    <td>Benchmarked four small open models on Turkish and English notes. Gemma 4 E2B won; quantized to Q3_K_M with low-memory settings it uses <b>~1.85 GB RAM</b> and scores <b>91% field accuracy / 94% precision</b> on a held-out set.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🔒 <b>Local by design</b></td>
    <td><code>llama-server</code> runs as a local sidecar bound to <code>127.0.0.1</code> and stops with the app; no account, no cloud calls. Notes stay plain <code>.md</code> files, so the vault also opens in Obsidian.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🧠 <b>Memory and Q&A</b></td>
    <td>Semantic search with EmbeddingGemma-300M, an assistant panel that calls tools (search notes, add a task, …), daily summaries and a weekly report.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🛠️ <b>Engineered, not vibe-coded</b></td>
    <td>Spec first: 267 EARS requirements in an ISO 29148-style SRS. Rust core (<code>pla-core</code>) + Tauri 2 / Svelte 5 UI, SQLite with FTS5, ~490 automated tests, Windows installer.</td>
  </tr>
</table>

<p>
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/Tauri_2-24C8D8?style=flat-square&logo=tauri&logoColor=white" alt="Tauri">
  <img src="https://img.shields.io/badge/Svelte_5-FF3E00?style=flat-square&logo=svelte&logoColor=white" alt="Svelte">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/llama.cpp-1f2328?style=flat-square" alt="llama.cpp">
  <img src="https://img.shields.io/badge/Gemma_4-4285F4?style=flat-square&logo=google&logoColor=white" alt="Gemma 4">
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/Python-eval_harness-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
</p>

## More projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/smart-field-audit-system">Smart Field Audit System</a></h3>
      <p>Field audit and task management for municipal field teams, built during my internship. Admin / manager / field roles, map-based audit points, photo evidence, a full activity log, Excel / PDF / QR reports.</p>
      <p><code>Laravel 12</code> <code>Docker</code> <code>MySQL</code> <code>Redis</code> <code>MinIO</code> <code>Leaflet</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/cogni-ticket">CogniTicket</a></h3>
      <p>Support ticket system where an LLM (Llama 3 via Groq) prioritizes and analyzes each ticket in a queued background job. SPA-like interface in plain JavaScript with no frontend framework.</p>
      <p><code>Laravel 12</code> <code>Groq API</code> <code>Queues</code> <code>Tailwind</code> <code>MySQL</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/cms-app_back-end_database">CMS &amp; Blog Platform</a></h3>
      <p>Content management with role-based access, N+1 queries removed with eager loading, indexed hot columns, cached navigation and Turkish / English content.</p>
      <p><code>Laravel 13</code> <code>PHP 8.4</code> <code>Spatie Permission</code> <code>MySQL</code> <code>Vite</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://ayberkcerit.github.io/Portfolio_Web/">Portfolio</a></h3>
      <p>My personal site: a bilingual, responsive single page with my skills, projects and CV, hosted on GitHub Pages.</p>
      <p><code>HTML</code> <code>CSS</code> <code>JavaScript</code></p>
    </td>
  </tr>
</table>

## Toolbox

**Languages**<br>
<img src="https://skillicons.dev/icons?i=py,cpp,php&perline=12" alt="Python, C++, PHP, " height="44">

**Desktop and web**<br>
<img src="https://skillicons.dev/icons?i=laravel,html,css&perline=12" alt="Laravel, HTML, CSS" height="44">

**Data, infrastructure and tools**<br>
<img src="https://skillicons.dev/icons?i=sqlite,mysql,redis,docker,git,github,vscode&perline=12" alt="SQLite, MySQL, Redis, Docker, Git, GitHub, VS Code" height="44">

**AI / ML**<br>
<img src="https://img.shields.io/badge/llama.cpp-1f2328?style=for-the-badge" alt="llama.cpp">
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama">
<img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Hugging Face">
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">

🎓 [freeCodeCamp Python certification](https://www.freecodecamp.org/certification/fcc-8f89b51a-2986-4298-b835-168ac71e984c/python-v9)

<p align="center"><sub>Local-first, measured, documented. Thanks for stopping by.</sub></p>
