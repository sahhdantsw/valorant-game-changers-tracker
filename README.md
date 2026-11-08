<h1 align="center">VALORANT · Game Changers</h1>

<h3 align="center">A desktop companion to keep up with upcoming matches</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-555555?style=for-the-badge&logo=windows&logoColor=white" alt="Windows">
  <img src="https://img.shields.io/badge/Python-3.10%2B-555555?style=for-the-badge&logo=python&logoColor=white" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/Built%20with-Flet-555555?style=for-the-badge&logo=flutter&logoColor=white" alt="Built with Flet">
  <img src="https://img.shields.io/badge/Language-Portugu%C3%AAs%20(BR)-555555?style=for-the-badge" alt="Brazilian Portuguese">
</p>

---

## About

**VALORANT · Game Changers** is a small desktop app for keeping track of Game Changers competition schedules. Pick a competition and the teams you want to follow; upcoming matches are shown in your selected time zone, and optional email reminders can let you know before they start.

- 🌐 **Language:** the app's interface is in **Brazilian Portuguese (Português do Brasil)**. This README is in English

---

## Features

- 👥 Follow teams from the Brazilian and international scenes
- 📅 See upcoming matches and team logos
- 🕒 View match times in your selected time zone
- 📧 Get optional email reminders with a configurable lead time
- 🔔 Keep the app minimized in the Windows notification area and launch it at startup
- 💾 Save your preferences locally on your computer

---

## Installation (Windows)

1. Download or clone this repository, then extract the files if needed
2. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if it is not already installed
3. Run `instalar.bat`

The installer prepares the environment, builds the app, and adds it to Windows startup. After installation, the app starts minimized; look for its icon in the notification area next to the clock.

To remove the app, run `desinstalar.bat`.

---

## Email reminders

Email reminders are optional. The app uses SMTP to send a message before a match, and you can set the reminder lead time in the app.

1. Copy `.env.example` to `.env` in the project folder
2. Fill in your SMTP server details:

```dotenv
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@example.com
SMTP_PASSWORD=your-app-password
EMAIL_FROM=your-email@example.com
SMTP_USE_SSL=false
```
