<p align="right">
  🌐 <a href="README.md"><img src="https://img.shields.io/badge/EN-6e7781?style=flat-square" alt="EN"></a> <img src="https://img.shields.io/badge/TR-0f7a63?style=flat-square" alt="TR (current)">
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Ayberk Cerit — Yerel çalışan yapay zekâ geliştiren Yazılım Mühendisliği öğrencisi" src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://ayberkcerit.github.io/Portfolio_Web/"><img src="https://img.shields.io/badge/Portfolio-0f7a63?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/ayberk-cerit-4707a12a4/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:a2407231005@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://ayberkcerit.github.io/Portfolio_Web/cv.pdf"><img src="https://img.shields.io/badge/CV-24292f?style=for-the-badge&logo=readdotcv&logoColor=white" alt="CV"></a>
</p>

## Hakkımda

Gümüşhane Üniversitesi'nde **Yazılım Mühendisliği** 3. sınıf öğrencisiyim ve hedefim **yapay zekâ / makine öğrenmesi mühendisliği**.
Beni en çok *verinin bulunduğu yerde* çalışan yapay zekâ heyecanlandırıyor: bilgisayarında, küçük bir cihazda, bir İHA'da. Başkasının bulutunda değil.

- 🔭 **Geliştiriyorum:** [PLA](https://github.com/AyberkCerit/personal_life_assistant), yerel bir dil modeliyle çalışan çevrimdışı kişisel asistan (Rust · Tauri · llama.cpp)
- 🏛️ **2026 yazı:** **Bilim A.Ş.**'de (Konya Büyükşehir Belediyesi teknoloji birimi) yazılım geliştirme stajyeri; Laravel + Docker üzerinde saha denetim ve görev yönetim sistemi geliştirdim
- 🌱 **Öğreniyorum:** otonom İHA'lar için pekiştirmeli öğrenme, görüntü işleme, işletim sistemleri
- 🤝 **Açığım:** yapay zekâ / ML stajlarına ve cihaz üzerinde çalışan yapay zekâ sohbetlerine

## Öne çıkan proje: PLA, bilgisayarından çıkmayan kişisel asistan

Notlar, görevler, hatırlatıcılar ve sağlık ölçümleri tek bir masaüstü uygulamasında, **tamamen çevrimdışı**.
Yapay zekâ yandan eklenmiş bir sohbet botu değil. Arka planda çalışıyor: yazdıklarını okuyup sessizce görev, hatırlatıcı ve ölçüme çeviriyor. Sorduğunda kendi notlarından cevap veriyor.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/pla-pipeline-dark.svg">
  <img alt="PLA akışı: Markdown not → değişen bloklar → Gemma 4 ile cihaz üzerinde çıkarım → Rust'ta doğrulama → görevler, hatırlatıcılar, ölçümler" src="assets/pla-pipeline-light.svg" width="100%">
</picture>

<table>
  <tr>
    <td width="27%" valign="top">🧪 <b>Model ölçümle seçildi</b></td>
    <td>Dört küçük açık modeli Türkçe ve İngilizce notlarla denedim. Gemma 4 E2B kazandı; Q3_K_M niceleme ve düşük bellek ayarlarıyla <b>~1,85 GB RAM</b> kullanıyor, ayrı test setinde <b>%91 alan doğruluğu / %94 kesinlik</b> alıyor.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🔒 <b>Tasarım gereği yerel</b></td>
    <td><code>llama-server</code>, <code>127.0.0.1</code> adresine bağlı yerel bir yan süreç olarak çalışır ve uygulamayla birlikte kapanır; hesap yok, bulut çağrısı yok. Notlar düz <code>.md</code> dosyası olarak kalır, kasa Obsidian'da da açılır.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🧠 <b>Bellek ve soru-cevap</b></td>
    <td>EmbeddingGemma-300M ile anlamsal arama, araç çağıran bir asistan paneli (not arama, görev ekleme, …), günlük özetler ve haftalık rapor.</td>
  </tr>
  <tr>
    <td width="27%" valign="top">🛠️ <b>Mühendislikle yapıldı</b></td>
    <td>Önce şartname: ISO 29148 tarzı SRS'te 267 EARS gereksinimi. Rust çekirdek (<code>pla-core</code>) + Tauri 2 / Svelte 5 arayüz, FTS5'li SQLite, ~490 otomatik test, Windows kurulum dosyası.</td>
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

## Diğer projeler

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/smart-field-audit-system">Smart Field Audit System</a></h3>
      <p>Belediye saha ekipleri için denetim ve görev yönetimi; stajım sırasında geliştirdim. Yönetici / müdür / saha rolleri, haritalı denetim noktaları, fotoğraflı kanıt, tam etkinlik günlüğü, Excel / PDF / QR raporları.</p>
      <p><code>Laravel 12</code> <code>Docker</code> <code>MySQL</code> <code>Redis</code> <code>MinIO</code> <code>Leaflet</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/cogni-ticket">CogniTicket</a></h3>
      <p>Her talebi sıralı bir arka plan işinde bir LLM'in (Groq üzerinden Llama 3) önceliklendirip analiz ettiği destek talebi sistemi. Çatısız, düz JavaScript ile SPA benzeri arayüz.</p>
      <p><code>Laravel 12</code> <code>Groq API</code> <code>Queues</code> <code>Tailwind</code> <code>MySQL</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/AyberkCerit/cms-app_back-end_database">CMS &amp; Blog Platform</a></h3>
      <p>Rol tabanlı erişimli içerik yönetimi; eager loading ile N+1 sorguları giderildi, sık sorgulanan sütunlar indekslendi, menüler önbelleğe alındı, içerik Türkçe / İngilizce.</p>
      <p><code>Laravel 13</code> <code>PHP 8.4</code> <code>Spatie Permission</code> <code>MySQL</code> <code>Vite</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://ayberkcerit.github.io/Portfolio_Web/">Portfolio</a></h3>
      <p>Kişisel sitem: yeteneklerimi, projelerimi ve CV'mi gösteren, iki dilli, duyarlı tek sayfa; GitHub Pages'te yayında.</p>
      <p><code>HTML</code> <code>CSS</code> <code>JavaScript</code></p>
    </td>
  </tr>
</table>

## Araç kutusu

**Diller**<br>
<img src="https://skillicons.dev/icons?i=py,cpp,php&perline=12" alt="Python, C++, PHP, " height="44">

**Masaüstü ve web**<br>
<img src="https://skillicons.dev/icons?i=laravel,html,css&perline=12" alt="Laravel, HTML, CSS" height="44">

**Veri, altyapı ve araçlar**<br>
<img src="https://skillicons.dev/icons?i=sqlite,mysql,redis,docker,git,github,vscode&perline=12" alt="SQLite, MySQL, Redis, Docker, Git, GitHub, VS Code" height="44">

**AI / ML**<br>
<img src="https://img.shields.io/badge/llama.cpp-1f2328?style=for-the-badge" alt="llama.cpp">
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama">
<img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Hugging Face">
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">

🎓 [freeCodeCamp Python sertifikası](https://www.freecodecamp.org/certification/fcc-8f89b51a-2986-4298-b835-168ac71e984c/python-v9)

<p align="center"><sub>Yerel öncelikli, ölçülmüş, belgelenmiş. Uğradığın için teşekkürler.</sub></p>
