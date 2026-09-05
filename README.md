<img src="icon.png" alt="Burn" width="110">

# Burn

A Mac menu bar app that shows your Claude, ChatGPT Codex and Notion AI usage at a glance. A second Claude account appears when one is connected.

This repository holds the downloads only. Burn's source code is private.

**[Download the latest version](../../releases/latest)**

## What It Does

Burn keeps a live reading in your menu bar. Choose Inline for one row or Stacked for two rows, then pick the tools, usage windows and countdowns you want to see. You can use different settings on the laptop screen and an external monitor.

The numbers are pace aware. They stay calm while you are comfortably inside your window and warm toward red as you start burning faster than the time left allows, so 80 percent with half an hour to go reads very differently from 80 percent with four hours to go.

Click the menu bar to open the full panel. Choose Classic, Classic with Heroes or Rails to see your session and longer budgets, reset countdowns and usage history. Supported accounts also show separate model allowances and a breakdown of model usage recorded on this Mac.

Plan badges follow your current subscription: Pro, Max 5x or Max 20x for Claude, and Plus, Pro 5x or Pro 20x for Codex. The small macOS widget shows the full plan too.

Burn includes an optional small widget in the macOS widget gallery. It can also send notifications when you cross a usage level or start running hot.

## Requirements

- macOS 13 Ventura or later
- An Apple Silicon Mac. This build will not run on an Intel Mac.
- The `claude` or `codex` command line tool installed and signed in. Burn reads the sign in they have already saved, so it never asks you for a password.

## Installing

The first install has to be done by hand. Every update after that installs itself.

1. Download the zip from the [latest release](../../releases/latest) and double click it to unzip.
2. Drag **Burn** into your Applications folder.
3. Open it. macOS will refuse the first time and say it cannot verify the developer. That is expected, because Burn is a personal app rather than something from the App Store.
4. Open System Settings, go to Privacy and Security, scroll to the bottom, and press **Open Anyway**. Confirm, and Burn will start.
5. The first time it reads your sign in, macOS asks for permission. Choose **Always Allow** so it stops asking.

Burn lives in the menu bar. Open its dropdown to reach the Settings window.

## Updating

Burn checks this repository once a day on its own. When a newer version is here it downloads it, verifies the app and its developer signature, replaces itself, and shows you what changed after relaunching. You can also check from Settings, General, Updates.

## Privacy

Burn contacts Anthropic and OpenAI to read your usage and current plan using the sign-in already saved on this Mac. If you use Notion AI, it reads that usage through your signed-in Notion desktop app. Burn also contacts GitHub to check for and download app updates. There is no analytics and no separate Burn account to create.

The figures it gets back are kept in a plain text file on your Mac at `~/Library/Application Support/Burn/state.json`, which you are welcome to read from your own scripts. It stays current while Burn is running.

## Source Code

Kept private on purpose. This repository exists so that Burn has somewhere public to fetch its updates from, without anything else being exposed.
