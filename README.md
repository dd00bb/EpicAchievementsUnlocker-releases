English | **[中文](README.zh.md)**

# Epic Achievement Unlocker — User Guide

> **Bilibili: IPhoneP40Pro | Xiaoheihe: letmethink**
>
> ⚠️ **This software is completely FREE!** If you paid for this tool, you have been scammed — please report the seller immediately.
> This software only supports genuine Epic / games using the Epic achievements system. Please support game developers.

**Notes:**
- Run the unlocker as **Administrator**, otherwise the two "Unlock Achievements" buttons won't work.
- When selecting the game executable and `EOSSDK-Win64-Shipping.dll`, the game **must be closed**.
- After replacement, **launch the game manually from Epic** — this tool will not launch it for you.
- If you pick the wrong DLL, close the unlocker and start over.
- Always close the game first, then close the unlocker.

---

## 1. Introduction

This tool unlocks achievements in Epic platform games that **have met their unlock conditions but were not counted properly**, and can also restore achievements lost due to missing/corrupted save data.

---

## 2. System Requirements

| Item | Requirement |
|------|-------------|
| Operating System | Windows 10 / 11 (64-bit) |
| Game Platform | Epic Games Store, or games using Epic Online Services |
| Privileges | Recommended to run this tool as **Administrator** (required for the unlock buttons) |
| Antivirus Software | If flagged, add the tool to your whitelist (modifying DLLs is a sensitive operation — false positives are normal) |

---

## 3. Important: How to Choose the Correct EXE for Unreal Engine Games

> **This is the step where mistakes happen most often — read carefully!**

Games made with Unreal Engine often contain **a huge pile of EXE files** in their directory: launchers, crash handlers, UnityPak, UnrealEditor, and so on. Picking the wrong one will cause the tool to fail to find the correct game directory.

### ✅ Correct choice

Select the file named like:

~~~text
GameName-Win64-Shipping.exe
~~~

For example:

| Game | File to select |
|------|----------------|
| A game called `MyGame` | `MyGame\Binaries\Win64\MyGame-Win64-Shipping.exe` |
| Elden Ring–style naming | `xxx\Binaries\Win64\xxx-Win64-Shipping.exe` |
| Chinese game `XYZ` | `XYZ\Binaries\Win64\XYZ-Win64-Shipping.exe` |

It is usually located in the **`Binaries\Win64\`** folder under the game directory.

### ❌ Do NOT select these

- `启动游戏.exe`, `启动器.exe`, `Launcher.exe` (these are just launchers)
- `UnityCrashHandler64.exe`, `CrashReportClient.exe` (crash reporters)
- Any EXE with `Editor`, `Pak`, `Installer`, or `Unreal` in its name

### 💡 Quick trick if you can't find it

Open the game's installation root folder and search directly in the top-right search box:

~~~text
Win64-Shipping.exe
~~~

The result (usually only one) is the file you need. If multiple results appear, pick the one **with the same name as the game**, and confirm its path contains `Binaries\Win64`.

### 📁 Full directory structure example

~~~text
E:\Games\MyGame\          ← Game root directory
├── MyGame.exe            ← ❌ This is usually a launcher, don't pick it
├── Engine\
└── MyGame\
    └── Binaries\
        └── Win64\
            ├── MyGame-Win64-Shipping.exe    ← ✅ Pick this one!
            └── EOSSDK-Win64-Shipping.dll    ← EOSSDK is usually here too
~~~

### Non-UE games (e.g., Unity games)

Select the main EXE in the game's root directory that has the same name as the game. The prerequisite is that the game uses Epic Online Services (i.e., you can find `EOSSDK-Win64-Shipping.dll` in the directory), otherwise this tool will not work.

---

## 4. Achievement List & Unlock Operations

### Selecting achievements

- Click the checkboxes to select the achievements you want; hover over an achievement to view its description.
- The **Select All / Deselect All / Invert** buttons allow one-click operations.

### Unlocking achievements (operate while the game is running)

- ⚠️ Both of these buttons only work when clicked **while the game is running**.
- After clicking, the tool will automatically switch back to the game window; wait a few seconds and you should see the achievement popup.
- Hotkeys for the two buttons: **Unlock All Achievements = `U`**, **Unlock Selected Achievements = `I`**.
- If nothing happens, you are probably not running as Administrator. Go back into the game and press the corresponding hotkey (`U` or `I`) manually once.

---

## 5. Frequently Asked Questions (FAQ)

**Q1: The achievement list never appears?**
- Confirm that the game EXE you selected is `GameName-Win64-Shipping.exe` (see Section 3);
- Confirm that EOSSDK was replaced successfully under `Binaries\Win64\`;
- Confirm that the game actually uses Epic Online Services.
- Note: for some games, the unlocker may not display the achievement list, but "Unlock All Achievements" still works.

**Q2: Nothing happens after clicking Unlock?**
- Make sure the game is running and not frozen;
- Make sure the unlocker is running as Administrator.

**Q3: Unlocked achievements don't show up on the Epic platform?**
- Platform achievement sync may be delayed — restart the Epic client or wait a few minutes;
- Make sure the game is genuine and you are logged into your Epic account.

**Q4: The software is flagged by antivirus?**
- False positives are normal. Simply add this tool to your whitelist.

**Q5: Could I get banned?**
- As with any tool that interacts with online services, some theoretical risk cannot be ruled out. Please use your own judgment. It is recommended **not to use this tool in competitive games or online games with anti-cheat systems**.

---

## 6. Notices & Disclaimer

1. This software is for learning and communication purposes only. **Reselling is strictly prohibited.** This software is free — any charging behavior has nothing to do with the author.
2. Please use this tool on genuine games and support the game developers.
3. All consequences arising from the use of this tool are borne by the user. The author is not responsible for account risks, save corruption, or anything else.
4. It is recommended to back up your game saves before use.

---

If this tool helps you, feel free to click [Donate] inside the app to buy the author a coffee ❤
