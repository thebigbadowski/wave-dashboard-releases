# Wave Dashboard

Wave Dashboard is a Windows desktop app for live Rocket League session stats. It connects to Rocket [League's Stats API](https://www.rocketleague.com/en/developer/stats-api), shows a real-time match dashboard, and helps track what is happening during a play session without needing a browser tab open.

This repository hosts the public installer and release files only. It does not contain the app source code.

## Download

[Download Wave Dashboard for Windows](https://github.com/thebigbadowski/wave-dashboard-releases/releases/latest/download/Wave-Dashboard-Setup.exe)

Run the installer, then open Wave Dashboard from the Start Menu, desktop shortcut, or pinned taskbar icon.

## Features

- Live Rocket League dashboard powered by the local Stats API.
- Session win/loss/streak tracking by playlist and mode.
- Team views with live player stats for goals, shots, assists, saves, touches, bumps, demos, own goals, average hit speed, and fastest hit speed.
- Large live ball-speed speedometer with peak-speed and average-speed visuals.
- One click pop out RL Tracker profile windows.
- Mode controls for playlist, game mode, and team size.
- Visual stat-change highlights during live play.
- A large visual demo notification
  -Green if other team dies
  -Red if your team dies
  -Yellow if both are destroyed
- Built-in bug report and feature request buttons.

## Rocket League Setup

Wave Dashboard needs Rocket League's local Stats API enabled before it can receive live match data.

Edit Rocket League's `DefaultStatsAPI.ini` before launching the game:
This file can be found at <Install Dir>\TAGame\Config\DefaultStatsAPI.ini
Do NOT change the port number but adjust this send rate to any number 1-120. That is how many times a second RL will send information to Wave.
It works fine on 10

```ini
PacketSendRate=10
Port=49123
```

Then start Rocket League, open Wave Dashboard, and turn the server on from the app.

## Updates

Wave Dashboard checks for updates when the app opens. If a newer version is available, the app shows an update notice and lets you choose whether to download it.

If you skip an update and install a later one, the app can show the release notes for the versions you missed.

## Notes

Wave Dashboard is currently a pre-1.0 alpha release. Expect rough edges, fast iteration, and occasional changes while the app is being tested.

For bugs or feature ideas, use the buttons inside the app or open an issue from this repository.
