# Zoom Speech Timer Background

**Show the Speech Timer colours to everyone in a Zoom meeting, as your camera feed (Mac and Windows)**

When you are the Timer in an online meeting, you can send the Speech Timer to Zoom as your video. Everyone, including the speaker, sees green, orange and red in your video tile. You can show the timer on its own, or with yourself cut out and placed in front of it, like a virtual background.

This uses **Meld Studio**, a free app for Mac and Windows with a built-in virtual camera. Zoom sees that virtual camera as a webcam.

[← Back to the Help Guide](./HELP.md)

---

## Contents

- [What you need](#what-you-need)
- [1. Install Meld Studio](#1-install-meld-studio)
- [2. Install the virtual camera](#2-install-the-virtual-camera)
- [3. Open the Speech Timer in its own window](#3-open-the-speech-timer-in-its-own-window)
- [4. Build the scene in Meld Studio](#4-build-the-scene-in-meld-studio)
- [5. Choose Meld Studio as your camera in Zoom](#5-choose-meld-studio-as-your-camera-in-zoom)
- [During the meeting](#during-the-meeting)
- [Troubleshooting](#troubleshooting)

---

## What you need

| | Mac | Windows |
|---|---|---|
| **Computer** | macOS 12 or later, Apple silicon or Intel | 64-bit Windows 10 (version 2004 or later) or Windows 11, on an Intel or AMD processor. Windows on Arm and Windows in S mode aren't supported. |
| **Meld Studio** | Free, from [meldstudio.co/download](https://meldstudio.co/download/) | Free, from [meldstudio.co/download](https://meldstudio.co/download/) |
| **Timer on its own** | ✅ Any supported Mac | ✅ Any supported PC |
| **You in front of the timer** | ✅ **Apple silicon only** (M1 or later) | ✅ Only with an **NVIDIA RTX** graphics card and driver 570 or later |

You also need a recent version of **Zoom** and the **Speech Timer**: [theonelevel-com.github.io/speech-timer](https://theonelevel-com.github.io/speech-timer/)

> **Background effects (Remove and Blur) aren't available on every computer.** On a Mac they need Apple silicon, so **Intel Macs can't use them**. On Windows they need an NVIDIA RTX card. Without that hardware, Meld Studio hides the **Background** option, but you can still show the timer on its own.

---

## 1. Install Meld Studio

### Mac

1. Go to [meldstudio.co/download](https://meldstudio.co/download/) and click **Download for macOS**
2. Double-click **MeldStudioInstaller.dmg**
3. Drag **Meld Studio** into the **Applications** folder
4. Close the window and eject the installer (⏏ in Finder)
5. Open **Meld Studio** from Applications

### Windows

1. Go to [meldstudio.co/download](https://meldstudio.co/download/) and download the Windows version
2. Run **MeldSetup.exe** and follow the installer's steps
3. Open **Meld Studio**

If the installer asks for **Microsoft WebView2**, install the WebView2 Runtime from Microsoft and run **MeldSetup.exe** again. Some antivirus tools wrongly flag the installer. Meld's [install page](https://meldstudio.co/docs/getstarted/install/) explains what to do.

---

## 2. Install the virtual camera

### Mac

The Mac virtual camera is a camera extension, so you need to approve it once.

1. In Meld Studio, go to **Settings → General → Virtual Camera** and click **Install**. You can also start the install from the **Outputs** panel on the right.
2. Meld Studio shows **Awaiting Approval** until macOS approves it.
3. Open the Mac's **System Settings**, type **login** in the search box and choose **Login Items & Extensions**
4. Scroll down to **Extensions**, click the **ⓘ** next to **Camera Extensions**, turn on **Meld Studio** and click **Done**. Your Mac may ask for your password or Touch ID.
5. Back in Meld Studio, the **Install** button is now a **Virtual Camera** switch in the **Outputs** panel.

### Windows

1. In Meld Studio, go to **Settings → Virtual Camera** and click **Install**
2. **Restart Meld Studio**. The virtual camera only works after a restart.
3. The **Install** button is now a **Virtual Camera** switch in the **Outputs** panel.

To remove it later, go back to **Settings → Virtual Camera**.

---

## 3. Open the Speech Timer in its own window

Run the timer in its own window so Meld Studio can capture it while you click Start, Finished and so on as usual.

- **Best:** install the Speech Timer as an app from Chrome or Edge, on Mac or Windows (see [Install as an App](./HELP.md#install-as-an-app)). It then opens in its own window.
- **Or:** open the timer in its own browser window, with nothing else in that window.

Make the window roughly **16:9** (wide rather than tall) so the colour fills the Zoom frame.

**Tip:** tick **Competition mode** if the speaker should see only the colour, not the time.

---

## 4. Build the scene in Meld Studio

These steps are the same on Mac and Windows.

### Add the timer

1. In the **Layers** panel on the left, click **╋** and choose **Display capture**
2. Choose the **Speech Timer** window from the list. If only whole screens are listed, choose the screen the timer is on, then move and resize the layer so the timer fills the frame.
3. Drag and resize the layer on the canvas so the timer fills the frame
4. **Mac only:** if macOS asks for permission to record the screen, allow it, then reopen Meld Studio if it asks you to

That is all you need to show the timer on its own.

### Optional: put yourself in front of the timer

> Needs an **Apple silicon Mac** or a **Windows PC with an NVIDIA RTX card** (see [What you need](#what-you-need)).

1. In **Layers**, click **╋** and choose **Video device**, then pick your webcam
2. Drag the webcam layer **above** the timer layer in the Layers list, so it sits in front
3. With the webcam layer selected, go to the **Background** section of the **Inspector**, turn **Background** on and choose **Remove**
4. Adjust **Threshold** and **Feather** until the edges around you look clean. The timer now shows through behind you.
5. Move and resize yourself on the canvas, for example into a lower corner, so the colour stays easy to see

**Windows:** the first time you use a background effect, Meld Studio downloads NVIDIA's video effects in the background (about 1 GB). If it fails, click **Retry**. If it keeps failing, update your NVIDIA driver and restart Meld Studio. Windows also has a **Remove chair** option.

---

## 5. Choose Meld Studio as your camera in Zoom

1. In Meld Studio's **Outputs** panel, turn **Virtual Camera** on
2. In Zoom, click the **^** arrow next to **Start Video / Stop Video** (or go to **Settings → Video**) and choose **Meld Studio** as the camera. Depending on the version it may be called **Meld Studio Virtual Camera**.
3. If Zoom was already open and Meld Studio is not in the list, **quit Zoom completely** and open it again. Most apps only look for cameras when they start.
   - **Mac:** press **⌘Q**
   - **Windows:** right-click the Zoom icon in the system tray (bottom right, next to the clock) and choose **Exit**

---

## During the meeting

- Keep Meld Studio running, even minimised, or Zoom loses the picture
- Work the timer in its own window: Start, Pause, Finished and Reset all show up live in Zoom
- Ask the host to **spotlight** or **pin** your video so the speaker can see the colours
- Zoom shows **your own** preview mirrored by default, so the timer's text may look backwards to you. Everyone else sees it the right way round. To change your own view, untick **Mirror my video** in Zoom's **Settings → Video**.
- To switch back to your normal camera, choose your webcam in Zoom again. You can leave Meld Studio's virtual camera installed.

---

## Troubleshooting

| Problem | What to try |
|---------|-------------|
| Meld Studio isn't in Zoom's camera list | Check the virtual camera is switched on in Meld Studio's **Outputs** panel, then quit Zoom completely and reopen it. **Windows:** make sure you restarted Meld Studio after installing the virtual camera. |
| **Mac:** Meld Studio keeps saying "Awaiting Approval" | Repeat the Mac part of step 2 in **System Settings → Login Items & Extensions → Camera Extensions** |
| The virtual camera won't start | Quit Meld Studio and open it again |
| **Mac:** the timer layer is black or empty | Allow screen recording for Meld Studio in **System Settings → Privacy & Security**, then reopen Meld Studio |
| Your webcam doesn't show in Meld Studio | **Mac:** **System Settings → Privacy & Security → Camera**, make sure **Meld Studio** is allowed. **Windows:** **Settings → Privacy & security → Camera**, turn on **Camera access** and **Let apps access your camera**, and make sure **Meld Studio** is allowed. Close any other app that is using the camera. |
| No **Background** option for the webcam | Your computer can't run background effects: an Intel Mac, or a PC without an NVIDIA RTX card. Show the timer on its own instead. |
| **Windows:** the installer won't run or is blocked | See Meld's [install troubleshooting](https://meldstudio.co/docs/getstarted/install/) for WebView2, S mode, Windows updates and antivirus |

Meld Studio's own instructions: [Virtual Camera on macOS](https://meldstudio.co/docs/outputs/virtual-camera/macos/) · [Virtual Camera on Windows](https://meldstudio.co/docs/outputs/virtual-camera/windows/) · [Background removal and blur](https://meldstudio.co/docs/tips-tricks/background-removal-blur/) · [Installing Meld Studio](https://meldstudio.co/docs/getstarted/install/)

---

*Meld Studio is a separate, free app made by Meld. It isn't part of the Speech Timer, and its menus may change in later versions.*

[← Back to the Help Guide](./HELP.md)
