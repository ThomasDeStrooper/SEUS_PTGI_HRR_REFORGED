# SEUS PTGI HRR 2.1 Reforged

A community-made edit of **Sonic Ether's SEUS PTGI HRR 2.1**, focused on improving image quality and performance, adding more configuration options, fixing visual issues, and bringing in selected features from **Photon** alongside original features developed specifically for Reforged.

Reforged is built around the original SEUS PTGI HRR 2.1 shader. It is not a shader made from scratch. The original SEUS shader provides the foundation, with selected Photon features and my own features and improvements added on top of it.

The main goal of this project is to improve and extend SEUS PTGI HRR 2.1 while maintaining and enhancing its performance and without losing the look that made the original shader recognizable in the first place.

> [!NOTE]
> SEUS PTGI HRR 2.1 Reforged is an unofficial community edit. It is not affiliated with or endorsed by Sonic Ether.

## Non-Commercial Project

This project is made for the Minecraft shader community and is not intended to generate profit.

SEUS PTGI HRR 2.1 remains the work of **Sonic Ether**. Photon remains the work of its respective developers.

---

# Installation

## Installation 1 — Manual Drag & Drop

1. Install **OptiFine HD U G5+** or **Iris**.
2. Download the **SEUS PTGI HRR 2.1 Reforged** from this [repository](https://github.com/ThomasDeStrooper/SEUS_PTGI_HRR_REFORGED/releases?utm_source=chatgpt.com).
3. Download the original **SEUS PTGI HRR 2.1** from [Patreon](https://www.patreon.com/sonicether/posts/download-seus-2-45141775?utm_source=chatgpt.com) and **Photon v1.3b** from [Modrinth](https://modrinth.com/shader/photon-shader/versions).
4. Extract the **SEUS PTGI HRR 2.1 Reforged** ZIP.
5. Simply **drag and drop both the original SEUS PTGI HRR 2.1 ZIP and the Photon v1.3b ZIP onto `Apply Patch.bat`**.
6. Double-click **Apply Patch.bat** if needed.
7. The patcher will automatically detect the two shader ZIPs and generate your final **SEUS PTGI HRR 2.1 Reforged** shader pack.
8. The patcher will then ask whether you want to automatically install the generated shader into your shaderpacks folder. Enter **Y** for Yes or **N** for No. You can also simply **press Enter** to use the default option and automatically add the generated shader to your shaderpacks folder.

## Installation 2 — Automatic File Search

1. Install **OptiFine HD U G5+** or **Iris**.
2. Download the **SEUS PTGI HRR 2.1 Reforged** from this [repository](https://github.com/ThomasDeStrooper/SEUS_PTGI_HRR_REFORGED/releases?utm_source=chatgpt.com).
3. Download the original **SEUS PTGI HRR 2.1** from [Patreon](https://www.patreon.com/sonicether/posts/download-seus-2-45141775?utm_source=chatgpt.com) and **Photon v1.3b** from [Modrinth](https://modrinth.com/shader/photon-shader/versions).
4. Extract the **SEUS PTGI HRR 2.1 Reforged** ZIP.
5. Once you have downloaded the required shader files, you can **double-click `Apply Patch.bat`** without manually dragging the shaders onto it.
6. The patcher will automatically search for the **SEUS PTGI HRR 2.1** and **Photon v1.3b** shader ZIPs in common locations, such as your **Downloads folder and Desktop**.
7. If you have downloaded the same shader multiple times, Windows may automatically add **`(1)`**, **`(2)`**, etc. to the filename. For example, the file may be named **`SEUS PTGI HRR 2.1 (1).zip`**. If this happens, **remove the `(1)` (or any other number in parentheses) from the filename** so that it is named **`SEUS PTGI HRR 2.1.zip`**. Otherwise, the automatic file search may not recognize it.
8. If the patcher finds both shaders, it will automatically use them to generate your final **SEUS PTGI HRR 2.1 Reforged** shader pack.
9. The patcher will then ask whether you want to automatically install the generated shader into your shaderpacks folder. Enter **Y** for Yes or **N** for No. You can also simply **press Enter** to use the default option and automatically add the generated shader to your shaderpacks folder.
10. If the patcher cannot find one or both shader files, make sure the filenames are correct and place them somewhere the patcher can find them, then run **`Apply Patch.bat`** again.

### File names

The automatic search expects the original shader to be named:

```text
SEUS PTGI HRR 2.1.zip
```

If Windows has renamed it to something like:

```text
SEUS PTGI HRR 2.1 (1).zip
```

remove the `(1)` so the filename is:

```text
SEUS PTGI HRR 2.1.zip
```

The same applies if Windows has added another number to the filename.

---

# Integrity and Verification

The patcher performs several checks before and during the patching process to make sure the shader files are not modified or corrupted.

The clean **SEUS PTGI HRR 2.1** pack and **Photon v1.3b** are both verified using **SHA-256** before patching begins.

The original SEUS and Photon shader files are **not redistributed by the patcher**. You provide the required files yourself, and the patcher only works with the copies on your system.

Every file that is patched is also checksummed both **before and after patching**. This allows the patcher to verify that the expected changes were made and that the resulting file is correct.

If all checks pass, the patcher can finish normally and the resulting files are verified **byte-for-byte** against what the patcher expects.

If any verification check fails, **nothing is written**. The patcher will stop instead of producing a potentially corrupted or incomplete shader pack.

In short:

```text
SEUS PTGI HRR 2.1
        |
        v
   SHA-256 check
        |
        v
   Photon v1.3b
        |
        v
   SHA-256 check
        |
        v
      Patching
        |
        v
  File checksums
 before and after
        |
        v
   Verification
        |
   +----+----+
   |         |
  PASS      FAIL
   |         |
   v         v
Output     Nothing
written    written
```

This is intended to make the patching process predictable and prevent the patcher from silently producing an incorrect result.

---

# What Reforged Changes

Reforged adds a number of changes to the original SEUS PTGI HRR 2.1 shader.

Some changes are fairly small, while others affect lighting, reflections, vegetation, or shader configuration.

## Visual Settings

The shader menu includes additional options for things such as:

* Held light shadows
* Screenspace reflection intensity
* Sharpening
* Reflection thickness threshold
* Water reflection sky leak
* Held item lighting
* Sun and moon reflections
* Cloud shadows
* Moonlight intensity
* Held light intensity
* Rain drop screen effect
* Nametag background
* Underwater distortion
* Underwater distortion speed
* Wind intensity
* Stained sunlight
* Godray stained-glass tint
* Parallax depth
* Rain splashes
* Water wave height
* Shadow map resolution
* Anisotropic LOD bias

These options can be adjusted from the shader settings instead of requiring changes to the shader files themselves.

---

# Ray-Traced Light Emission

Several blocks have been updated so that their ray-traced light uses more appropriate colors.

Currently this includes:

* End Rods
* Candles
* Froglights
* Copper Lanterns
* Copper Torches
* Beacons
* Brewing Stands
* Vaults

Candles, for example, can produce ray-traced light based on their actual candle color instead of using the same light color for every candle.

---

# Wavy Vegetation

Reforged also adds additional wavy animations.

This includes:

* Leaves
* Flowers
* Plants

The intention is to make vegetation feel a little more alive without changing the overall appearance of the shader too much.

---

# Photon Features

Photon is an important part of Reforged.

Reforged uses **Photon v1.3b** during the patching process and incorporates selected Photon features into the SEUS PTGI HRR 2.1 base.

This is why the patcher requires both the original SEUS PTGI HRR 2.1 shader and Photon.

In simple terms:

```text
SEUS PTGI HRR 2.1
        +
Selected Photon features
        +
Reforged changes and fixes
        =
SEUS PTGI HRR 2.1 Reforged
```

The project is still based on SEUS PTGI HRR 2.1. Photon is used to extend what the original shader can do rather than replacing the SEUS foundation entirely.

---

# Feature Showcase

These videos show some of the changes and features currently included in Reforged.

# Comparison

The images below were taken using the default shader settings.

The original SEUS PTGI HRR 2.1 is on the left and Reforged is on the right.

The comparisons show some of the differences introduced by Reforged, particularly around reflections, lighting, and other visual effects.

<table>
<tr>
<th>SEUS PTGI HRR 2.1</th>
<th>SEUS PTGI HRR 2.1 Reforged</th>
</tr>

<tr>
<td>
<img src="https://github.com/user-attachments/assets/824bf962-dd80-4a1e-9f44-6eb1ed995ba9" />
</td>
<td>
<img src="https://github.com/user-attachments/assets/2368197f-a857-49d4-924c-7f89e76904cb" />
</td>
</tr>

<tr>
<td>
<img src="https://github.com/user-attachments/assets/68af4811-99b2-455f-8245-6bff252b2386" />
</td>
<td>
<img src="https://github.com/user-attachments/assets/64b3e821-2366-4260-ad10-cd05aff42c28" />
</td>
</tr>

</table>

---

# Requirements

## Minecraft

* Minecraft **1.16.4 or newer**
* **OptiFine HD U G5+** or **Iris**

## Hardware

| Component       | Recommendation  |
| --------------- | --------------- |
| Minimum GPU     | NVIDIA RTX 2050 |
| Recommended GPU | NVIDIA RTX 3060 |

These are general recommendations rather than strict requirements. Actual performance depends on resolution, Minecraft settings, view distance, shader settings, and the rest of the system.

---

# Known Issues

## General

* Light rays can sometimes shine through buildings or other geometry.

## NVIDIA

NVIDIA GPUs are currently the main tested hardware for Reforged.

## AMD

Some visual issues or occasional crashes may occur.

A possible workaround is to start Minecraft, or enable shaders, while the game is in a small window before switching back to fullscreen.

## Intel

Intel GPU compatibility is currently not guaranteed.

---

# Credits

### Sonic Ether

The original **SEUS PTGI HRR 2.1** shader and its underlying work were created by **Sonic Ether**.

### Photon

Reforged incorporates selected features from **Photon**. Photon is developed separately from this project.

### Reforged

The additional modifications, fixes, configuration options, and integration work in this project are maintained by the Reforged community.

---

# Disclaimer

**SEUS PTGI HRR 2.1 Reforged is an unofficial community edit.**

It is not affiliated with, sponsored by, or endorsed by Sonic Ether.

The original SEUS PTGI HRR 2.1 shader is required to build Reforged. Please obtain it through its official distribution.

Photon is also distributed separately and remains the property of its respective developers.

This project does not redistribute the original SEUS PTGI HRR 2.1 shader.

---
