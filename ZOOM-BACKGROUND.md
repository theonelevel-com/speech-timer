# Zoom Speech Timer Background

**Show the Speech Timer colours to everyone in a Zoom meeting, as your camera feed (Mac)**

When you are the Timer in an online meeting, you can send the Speech Timer to Zoom as your video. Everyone, including the speaker, sees green, orange and red in your video tile. You can show the timer on its own, or with yourself cut out and placed in front of it, like a virtual background.

This uses **Meld Studio**, a free app for Mac that now includes a virtual camera. Zoom sees that virtual camera as a webcam.

[← Back to the Help Guide](./HELP.md)

---

## Contents

- [What you need](#what-you-need)
- [1. Install Meld Studio](#1-install-meld-studio)
- [2. Install and approve the virtual camera](#2-install-and-approve-the-virtual-camera)
- [3. Open the Speech Timer in its own window](#3-open-the-speech-timer-in-its-own-window)
- [4. Build the scene in Meld Studio](#4-build-the-scene-in-meld-studio)
- [5. Choose Meld Studio as your camera in Zoom](#5-choose-meld-studio-as-your-camera-in-zoom)
- [During the meeting](#during-the-meeting)
- [Troubleshooting](#troubleshooting)

---

## What you need

- A Mac running **macOS 12 or later**, either Apple silicon or Intel
- **Meld Studio**: free, from [meldstudio.co/download](https://meldstudio.co/download/)
- **Zoom**: a recent version
- The **Speech Timer**: [theonelevel-com.github.io/speech-timer](https://theonelevel-com.github.io/speech-timer/)
- To put yourself in front of the timer, you need an **Apple silicon Mac** (M1 or later), because Meld Studio's background removal needs one. On an Intel Mac you can still show the timer on its own.

---

## 1. Install Meld Studio

1. Go to [meldstudio.co/download](https://meldstudio.co/download/) and click **Download for macOS**
2. Double-click **MeldStudioInstaller.dmg**
3. Drag **Meld Studio** into the **Applications** folder
4. Close the window and eject the installer (⏏ in Finder)
5. Open **Meld Studio** from Applications

---

## 2. Install and approve the virtual camera

The virtual camera is a macOS camera extension, so you need to approve it once.

1. In Meld Studio, go to **Settings → General → Virtual Camera** and click **Install**. You can also start the install from the **Outputs** panel on the right.
2. Meld Studio shows **Awaiting Approval** until macOS approves it.
3. Open the Mac's **System Settings**, type **login** in the search box and choose **Login Items & Extensions**
4. Scroll down to **Extensions**, click the **ⓘ** next to **Camera Extensions**, turn on **Meld Studio** and click **Done**. Your Mac may ask for your password or Touch ID.
5. Back in Meld Studio, the **Install** button is now a **Virtual Camera** switch in the **Outputs** panel.

---

## 3. Open the Speech Timer in its own window

Run the timer in its own window so Meld Studio can capture it while you click Start, Finished and so on as usual.

- **Best:** install the Speech Timer as an app from Chrome or Edge (see [Install as an App](./HELP.md#install-as-an-app)). It then opens in its own window.
- **Or:** open the timer in its own browser window, with nothing else in that window.

Make the window roughly **16:9** (wide rather than tall) so the colour fills the Zoom frame.

**Tip:** tick **Competition mode** if the speaker should see only the colour, not the time.

---

## 4. Build the scene in Meld Studio

### Add the timer

1. In the **Layers** panel on the left, click **╋** and choose **Display capture**
2. Pick the **Speech Timer** window. If macOS asks for permission to record the screen, allow it, then reopen Meld Studio if it asks you to.
3. Drag and resize the layer on the canvas so the timer fills the frame

That is all you need to show the timer on its own.

### Optional: put yourself in front of the timer (Apple silicon only)

1. In **Layers**, click **╋** and choose **Video device**, then pick your webcam
2. Drag the webcam layer **above** the timer layer in the Layers list, so it sits in front
3. With the webcam layer selected, go to the **Background** section of the **Inspector**, turn **Background** on and choose **Remove**
4. Adjust **Threshold** and **Feather** until the edges around you look clean. The timer now shows through behind you.
5. Move and resize yourself on the canvas, for example into a lower corner, so the colour stays easy to see

---

## 5. Choose Meld Studio as your camera in Zoom

1. In Meld Studio's **Outputs** panel, turn **Virtual Camera** on
2. In Zoom, click the **^** arrow next to **Start Video / Stop Video** (or go to **Settings → Video**) and choose **Meld Studio** as the camera. Depending on the version it may be called **Meld Studio Virtual Camera**.
3. If Zoom was already open and Meld Studio is not in the list, **quit Zoom completely (⌘Q)** and open it again. Most apps only look for cameras when they start.

---

## During the meeting

- Keep Meld Studio running, even minimised, or Zoom loses the picture
- Work the timer in its own window: Start, Pause, Finished and Reset all show up live in Zoom
- Ask the host to **spotlight** or **pin** your video so the speaker can see the colours
- Zoom shows **your own** preview mirrored by default, so the timer's text may look backwards to you. Everyone else sees it the right way round. To change your own view, untick **Mirror my video** in **Zoom → Settings → Video**.
- To switch back to your normal camera, choose your webcam in Zoom again. You can leave Meld Studio's virtual camera installed.

---

## Troubleshooting

| Problem | What to try |
|---------|-------------|
| Meld Studio isn't in Zoom's camera list | Check the virtual camera is switched on in Meld Studio's **Outputs** panel, then quit Zoom completely (⌘Q) and reopen it |
| Meld Studio keeps saying "Awaiting Approval" | Repeat step 2 in **System Settings → Login Items & Extensions → Camera Extensions** |
| The virtual camera won't start | Quit Meld Studio and open it again |
| The timer layer is black or empty | Allow screen recording for Meld Studio in **System Settings → Privacy & Security**, then reopen Meld Studio |
| Your webcam doesn't show in Meld Studio | Check **System Settings → Privacy & Security → Camera** and make sure **Meld Studio** is allowed |
| No **Background** option for the webcam | Background removal needs an Apple silicon Mac. Show the timer on its own instead. |

Meld Studio's own instructions: [Virtual Camera on macOS](https://meldstudio.co/docs/outputs/virtual-camera/macos/) · [Background removal and blur](https://meldstudio.co/docs/tips-tricks/background-removal-blur/)

---

*Meld Studio is a separate, free app made by Meld. It isn't part of the Speech Timer, and its menus may change in later versions.*

[← Back to the Help Guide](./HELP.md)
