<div align="center">

<img src="https://raw.githubusercontent.com/RoxelJohnBangi-an/RoxelJohnBangi-an/main/github-metrics.svg" alt="GitHub metrics for RoxelJohnBangi-an" width="100%"/>

</div>

---

## 🐾 Spotlight: DailyFur

**A veterinary mobile app for pet owners (BSIT Capstone).**

- 📅 Vet appointments with notification badges
- 💬 Real-time chat with clinics
- 📍 Nearby clinics via geo-mapping
- 🩺 Teleconsultation with veterinarians
- 🚨 Emergency pet service coordination
- ⭐ Clinic ratings and in-app pet store

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Android](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=androidstudio&logoColor=white)
[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=for-the-badge&logo=github)](https://github.com/RoxelJohnBangi-an/DailyFur-MobileApp)

---

## 🚀 Featured Projects

| Project | What it does | Stack |
|---|---|---|
| 🐶 [**DailyFur**](https://github.com/RoxelJohnBangi-an/DailyFur-MobileApp) | Veterinary consultation mobile app | Kotlin · Firebase |
| 🛒 [**shophub**](https://github.com/RoxelJohnBangi-an/shophub) | E-commerce system | Laravel · MySQL |
| 📒 [**SlamBook**](https://github.com/RoxelJohnBangi-an) | Digital slam book Android app | Kotlin |
| 🌐 **Portfolio** | Personal developer site | HTML · CSS · JS |

---

## 🎯 Currently

- 🔨 Building and polishing **DailyFur**
- 📚 Learning **Machine Learning fundamentals**
- 🌱 Exploring **clean architecture for Android**
- 🤝 Looking for **collaborations and internships**

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github)](https://github.com/RoxelJohnBangi-an)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:roxeljohnbangian@gmail.com)

<br/>

*⭐ Building apps that help pets live healthier lives. 🐾*

</div>

# Save as: .github/workflows/metrics.yml
# (inside your profile repo: RoxelJohnBangi-an/RoxelJohnBangi-an)

name: Metrics
on:
  schedule: [{ cron: "0 */12 * * *" }]
  workflow_dispatch:
  push: { branches: ["main", "master"] }

jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Create a personal access token and save it as a repo secret named METRICS_TOKEN
          token: ${{ secrets.METRICS_TOKEN }}
          user: RoxelJohnBangi-an
          filename: github-metrics.svg

          # Same look as the screenshot: dark, 3-column "classic" layout
          template: classic
          config_display: columns
          config_timezone: Asia/Manila
          base: header, activity, community, repositories, metadata
          base_indepth: yes

          # Left/middle column
          plugin_lines: yes
          plugin_habits: yes
          plugin_habits_from: 200
          plugin_habits_days: 14
          plugin_habits_charts: yes
          plugin_topics: yes
          plugin_topics_mode: icons
          plugin_topics_sort: stars
          plugin_topics_limit: 30

          # Right column
          plugin_isocalendar: yes
          plugin_isocalendar_duration: half-year
          plugin_languages: yes
          plugin_languages_sections: most-used
          plugin_languages_limit: 8
          plugin_languages_colors: github

          # --- Optional blocks from the screenshot (uncomment to enable) ---

          # PageSpeed scores (needs a live site URL, e.g. your portfolio)
          # plugin_pagespeed: yes
          # plugin_pagespeed_url: https://YOUR-PORTFOLIO-URL

          # "Suggested tracks" (Apple Music playlist)
          # plugin_music: yes
          # plugin_music_provider: apple
          # plugin_music_playlist: https://music.apple.com/YOUR-PLAYLIST-URL
          # plugin_music_mode: playlist
          # plugin_music_limit: 2

          # Project board progress
          # plugin_projects: yes
          # plugin_projects_repositories: RoxelJohnBangi-an/DailyFur-MobileApp/1
