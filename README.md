# Brain

Brain reads your Obsidian vault and turns it into a map of the people, ideas and
questions in your notes: what you've been thinking about, how things connect, and
answers to questions about your own notes. It also lets you dictate anywhere on Windows.

Brain keeps everything it builds on your computer. To read your notes it sends their
text to OpenAI with your own API key (nowhere else), and shows the price before anything
costs money.

This repository holds release files only: installers and the update manifest the app
checks. Every update is signed, and Brain refuses any file whose signature doesn't match.

## Install

1. Open the [latest release](https://github.com/PamirSevincel/brain-releases/releases/latest)
   and download **one** installer:
   - `BrainSetup-x64.exe` for most Windows PCs;
   - `BrainSetup-arm64.exe` for ARM laptops (Surface Pro X / 11, Snapdragon PCs).

   Not sure? Settings → System → About → *System type* says "x64-based" or "ARM-based".
2. Run it. Windows may say **"Windows protected your PC"** because Brain isn't signed
   by a known publisher yet: click **More info**, then **Run anyway**.
3. Brain opens and asks a few questions: where your vault is, your OpenAI API key, your
   name and the key you'll hold to dictate.

You need Windows 10 or 11 and an OpenAI API key with a little credit
([platform.openai.com](https://platform.openai.com) → API keys; credit under Billing).
Building Brain reads every note once; Brain shows what that will cost before it starts.

## Updates

Brain updates itself: when a new version is out it shows **UPDATE** at the top, and
Settings → Updates → **Restart to update** installs it. Your data is kept.

## Uninstall

Settings → Apps → Installed apps → Brain → Uninstall. Your Brain data is kept unless you
tick "Delete the application data".

## Help

Settings → Diagnostics → **Save a support report** saves a zip to your Downloads folder
(Brain's logs and state; never the text of your notes or your key). Send it along with
what happened.
