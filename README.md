# Brain

Brain reads your Obsidian vault and turns it into a map of the people, ideas and
questions in your notes: what you've been thinking about, how things connect, and
answers to questions about your own notes. It also lets you dictate anywhere on your
computer.

Brain keeps everything it builds on your computer. To read your notes it sends their
text to OpenAI with your own API key (nowhere else), and shows the price before anything
costs money.

This repository holds release files only: installers and the update files the app
checks. Every update is signed, and Brain refuses any file whose signature doesn't match.

You need an Obsidian vault and an OpenAI API key with a little credit
([platform.openai.com](https://platform.openai.com) → API keys; credit under Billing).
Building Brain reads every note once; Brain shows what that will cost before it starts.

## Install on Windows (10 or 11)

1. Open the [latest release](https://github.com/PamirSevincel/brain-releases/releases/latest)
   and download **one** installer:
   - `BrainSetup-x64.exe` for most Windows PCs;
   - `BrainSetup-arm64.exe` for ARM laptops (Surface Pro X / 11, Snapdragon PCs).

   Not sure? Settings → System → About → *System type* says "x64-based" or "ARM-based".
2. Run it. Windows may say **"Windows protected your PC"** because Brain isn't signed
   by a known publisher yet: click **More info**, then **Run anyway**.
3. Brain opens and asks a few questions: where your vault is, your OpenAI API key, your
   name and the key you'll hold to dictate.

## Install on a Mac (Apple silicon: M1, M2, M3, M4; macOS 13 or later)

1. Download **`Brain-arm64.dmg`** from the
   [latest release](https://github.com/PamirSevincel/brain-releases/releases/latest),
   open it, and drag **Brain** into **Applications**.
2. Open Brain from Applications. Brain isn't signed by Apple yet, so the first time macOS
   stops it:
   - **macOS 15 (Sequoia) and later:** macOS says Brain "Not Opened". Click **Done**. Open
     **System Settings → Privacy & Security**, scroll down to *"Brain" was blocked*, click
     **Open Anyway**, confirm with your password or Touch ID, and click **Open Anyway**
     once more.
   - **macOS 13 or 14:** Control-click (right-click) Brain in Applications, choose
     **Open**, then **Open** again.

   You only do this once.
3. Brain opens and asks a few questions: where your vault is, your OpenAI API key, your
   name and the key you'll hold to dictate (Right Option ⌥ by default).
4. For dictation, Brain asks for two permissions, with buttons that open the right place:
   **Accessibility** (to notice your dictation key and paste what you said) and the
   **Microphone**. Turn on **Brain** in System Settings → Privacy & Security.

## Updates

Brain updates itself: when a new version is out it shows **UPDATE** at the top, and
Settings → Updates → **Restart to update** installs it. Your data is kept.

On a Mac, because Brain isn't signed by Apple yet, after an update macOS may:
- ask once whether Brain may use the key saved in your keychain: enter your Mac password
  and choose **Always Allow**;
- need Accessibility again: Brain says so in Settings → Dictation. In System Settings →
  Privacy & Security → Accessibility, turn Brain off and on again.

## Uninstall

- **Windows:** Settings → Apps → Installed apps → Brain → Uninstall. Your Brain data is
  kept unless you tick "Delete the application data".
- **Mac:** to remove everything, first choose Settings → Diagnostics → **Delete all Brain
  data…** in Brain (it quits), then move Brain from Applications to the Trash. Moving it
  to the Trash alone keeps your Brain data, for a later reinstall.

## Help

Settings → Diagnostics → **Save a support report** saves one zip (Brain's logs and state;
never the text of your notes or your key): to Downloads on Windows, and in a folder Brain
opens in Finder on a Mac. Send it along with what happened.
