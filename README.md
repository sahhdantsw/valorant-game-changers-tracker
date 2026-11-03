<div align="center">

# ♡ VALORANT · Game Changers

### A little desktop companion to keep up with upcoming matches. ✧

<img src="https://img.shields.io/badge/Windows-desktop-F7B7C8?style=flat-square&labelColor=F7B7C8&logo=windows&logoColor=6B4F5F" alt="Windows">
<img src="https://img.shields.io/badge/Python-3.10%2B-F4A6C1?style=flat-square&labelColor=F4A6C1&logo=python&logoColor=6B4F5F" alt="Python">
<img src="https://img.shields.io/badge/built%20with-Flet-E8A4B8?style=flat-square&labelColor=E8A4B8&logoColor=6B4F5F" alt="Built with Flet">

<br>

<img src="https://img.shields.io/badge/✿%20made%20with%20care%20by%20ME-✿-F7B7C8?style=flat-square&labelColor=F7B7C8" alt="Made with care by ME">

<br><br>

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=F7B7C8" width="80%" alt="pink divider">

</div>

## about

**VALORANT · Game Changers** is a small desktop app for keeping track of Game Changers competition schedules. Pick a competition and the teams you want to follow; upcoming matches are shown in your selected time zone, and optional email reminders can let you know before they start.

> **Language:** The app's interface is in **Brazilian Portuguese (Português do Brasil)**. This README is in English.

## features

- Follow teams from the Brazilian and international scenes.
- See upcoming matches and team logos.
- View match times in your selected time zone.
- Get optional email reminders with a configurable lead time.
- Keep the app minimized in the Windows notification area and launch it at startup.
- Save your preferences locally on your computer.

## installation · Windows

1. Download or clone this repository, then extract the files if needed.
2. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if it is not already installed.
3. Run `instalar.bat`.

The installer prepares the environment, builds the app, and adds it to Windows startup. After installation, the app starts minimized; look for its icon in the notification area next to the clock.

To remove the app, run `desinstalar.bat`.

## email reminders

Email reminders are optional. The app uses SMTP to send a message before a match, and you can set the reminder lead time in the app.

1. Copy `.env.example` to `.env` in the project folder.
2. Fill in your SMTP server details:

```dotenv
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@example.com
SMTP_PASSWORD=your-app-password
EMAIL_FROM=your-email@example.com
SMTP_USE_SSL=false
