# Bubble Generator

Fully synthesized bubble and water sounds, from cartoon to hyper-realistic foley. Every
sound is modelled on the physics of real water; the interface is a bundle of bubbles that
are the controls.

This page holds the installers. **[Download the latest version](https://github.com/bigdougmoney/bubble-generator-releases/releases/latest)**

- VST3 plug-in for your DAW, and a standalone app that plays without one.
- macOS 11 or newer, Apple Silicon and Intel.

## Installing on a Mac

Download `BubbleGenerator-<version>-macOS.zip` from the release and unzip it. The folder has
the installer (`.pkg`) and a `READ ME FIRST.txt` with these same steps.

The installer isn't registered with Apple (that costs a yearly fee), so the first time you
open it, macOS blocks it with a warning. You approve it once, then it installs normally.
Pick one of these two ways:

**Option A: System Settings (no Terminal)**

1. Double-click the `.pkg`. macOS says it "can't be opened" because Apple can't check it.
   Click **Done** (not Move to Trash).
2. Open **System Settings > Privacy & Security** and scroll down. Next to the message about
   BubbleGenerator being blocked, click **Open Anyway** and enter your Mac password.
3. The installer opens. Choose the VST3 plug-in, the standalone app, or both, and install.

**Option B: Terminal (skips the warning)**

1. Open Terminal (Applications > Utilities) and type this, with a space at the end:

   ```
   xattr -d com.apple.quarantine 
   ```

2. Drag the `.pkg` file onto the Terminal window, then press Return.
3. Double-click the `.pkg`. It opens straight away; install as usual.

Right-click > Open no longer skips the warning (Apple removed that in macOS 15).

## After installing

- **VST3:** restart your DAW or rescan plug-ins. In Ableton Live: Settings > Plug-Ins, turn
  on "Use VST3 Plug-In System Folders", then Rescan. It shows up as an instrument.
- **Standalone:** open Bubble Generator from Applications. It starts making sound as soon as
  it opens.

## Uninstall

Delete `/Library/Audio/Plug-Ins/VST3/Bubble Generator.vst3` and
`/Applications/Bubble Generator.app`.
