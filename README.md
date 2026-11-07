<!--
  Quantum Launcher
  Keep this README aligned with the implementation in app/src/main.
-->

<div align="center">

  <img src="app/src/main/res/mipmap-xxhdpi/ic_launcher.png" alt="Quantum Launcher app icon" width="112" />

  <h1>Quantum Launcher</h1>
  <p><strong>Your home screen. Your space. Your rules.</strong></p>
  <p>
    A highly customizable Android launcher with a distinctive visual language,
    expressive motion, flexible home-screen organization, and a native Java foundation.
  </p>

  <p>
    <a href="https://github.com/DS-ann/Quantum-Launcher/actions/workflows/Build.yml">
      <img src="https://github.com/DS-ann/Quantum-Launcher/actions/workflows/Build.yml/badge.svg?branch=main" alt="Build status" />
    </a>
    <img src="https://img.shields.io/badge/version-18.7.0-8B7CFF?style=flat" alt="Version 18.7.0" />
    <img src="https://img.shields.io/badge/Android-6.0%2B-3DDC84?style=flat&logo=android&logoColor=white" alt="Android 6.0 and newer" />
    <img src="https://img.shields.io/badge/language-Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java" />
    <img src="https://img.shields.io/badge/UI-Native%20Android-5271FF?style=flat" alt="Native Android UI" />
  </p>

  <p>
    <a href="#what-is-quantum-launcher">Discover</a> ·
    <a href="#the-design">The design</a> ·
    <a href="#features">Features</a> ·
    <a href="#getting-started">Get started</a> ·
    <a href="#building-from-source">Build</a>
  </p>

</div>

---

## What is Quantum Launcher?

Quantum Launcher is an Android home-screen replacement built for people who want more control over how their device feels and works.

It combines a deliberately compact **two-page workspace** with a configurable app drawer, movable home-screen items, widgets, app groups, a richly styled clock, and a deep set of visual controls in **Home Studio**.

The idea is simple: the launcher should feel like a personal environment, not just a grid of shortcuts. You can shape its layout, tune its motion, change the visual character of icons and clocks, and give the home screen a signature of its own.

| Project detail | Value |
|:--|:--|
| Current app version | `18.7.0` |
| Android application ID | `com.dsann.launcher` |
| Minimum Android version | `Android 6.0 · API 23` |
| Target / compile SDK | `37` |
| Main language | `Java` |
| UI foundation | Native Android views |
| Main development branch | `main` |

## The design

Quantum Launcher follows a **dark, atmospheric, high-contrast** design direction. Its interface uses deep surfaces to keep the workspace visually calm, then adds color where it matters: identity, focus, controls, and motion.

### A visual system with a point of view

- **Layered dark surfaces** give panels and controls depth without turning the screen into a wall of bright cards.
- **Aurora-inspired gradients** move through cyan, blue, violet, pink, and warm orange.
- **Rounded geometry** gives dialogs, controls, icon treatments, and app groups a consistent visual rhythm.
- **Typography with contrast** combines clean system text with expressive cursive and monospace treatments in selected areas.
- **Motion with purpose** gives page changes and drawer transitions a sense of direction, instead of treating every interaction as the same animation.

### Color themes

The app includes four selectable launcher themes. These are the underlying visual directions; wallpapers and other customizations can change the final appearance.

| Theme | Character | Palette |
|:--|:--|:--|
| **Midnight** | Deep, restrained dark surfaces | `#0F1424` → `#0A0D18` |
| **Ocean** | Cool blue and deep teal | `#082B3F` → `#08111F` |
| **Violet** | Purple-toned depth | `#31184C` → `#0C0D1D` |
| **Graphite** | Neutral, low-key contrast | `#242A37` → `#0C0F17` |

### Motion is part of the interface

Choose the page transition that best fits your setup:

- **3D Wheel**
- **3D Cube**
- **Parallax**
- **Page Flip**

The app drawer has its own transition choices: Parallax, 3D Card Flip, Depth Slide, and Rotating Carousel. Motion speed and wheel rotation can also be adjusted in Home Studio.

## Features

### 1. A focused two-page workspace

Keep your most-used apps and widgets close without creating an endless collection of home screens.

- Two stable home pages with independent item placement.
- Horizontal swipes to move between pages.
- Drag apps and supported workspace items to organize the layout.
- Move items between pages using the screen edge.
- Configurable home grid columns and icon size.
- Optional app labels, page indicator, and launcher signature.
- A dock for frequently used apps.

### 2. Home Studio: make the launcher yours

Home Studio is the central customization space. It brings layout, identity, clock, motion, drawer, and appearance controls into one place.

| Area | What you can customize |
|:--|:--|
| Home layout & icons | Grid columns, icon size, label size, label font, label color, and label visibility |
| Icon appearance | Background enablement, background color, fit, shape, artwork theme, and shortcut artwork |
| Widgets | Add Android widgets and create app groups |
| Clocks | Clock style, background opacity, artwork matching, gradient digits, and live color transitions |
| Clock typography | Date and AM/PM sizes, fonts, and date color |
| Page animations | Transition type, wheel rotation angle, and animation speed |
| App drawer | Opening effect, columns, icon size, font size, labels, sorting, spacing, and background opacity |
| Appearance | Midnight, Ocean, Violet, and Graphite themes; photo and system wallpaper options |
| Launcher identity | Change the home-screen brand label |

### 3. Distinctive icon treatments

Give the icon grid a consistent visual style, or make it more expressive.

**Available background shapes**
- Square
- Round
- Hexagon
- Pentagon
- Tilted Pear

**Artwork themes**
- Original Colours
- Spectrum Mix
- Ocean Gradient
- Sunset Gradient
- Nothing Monochrome

You can also toggle icon backgrounds, adjust their color, fit artwork inside the background, and apply themed artwork to supported shortcuts.

### 4. A clock that can be the centerpiece

The clock is designed as a customizable part of the workspace, not a fixed system decoration.

Choose from six visual styles:

1. Digital
2. Cyber HUD
3. Neon Circuit
4. Tech Minimal
5. Terminal Digital
6. 7-Segment Digital

Then tune its presentation with background opacity, optional date display, date and AM/PM typography, icon-artwork matching, gradient digits, and live gradient color transitions. Date and AM/PM sizing can be configured separately for each home page.

### 5. App drawer controls

The drawer has its own layout and appearance settings:

- Select the number of columns and icon size.
- Adjust app-name text size and label visibility.
- Sort app names from A to Z or Z to A.
- Choose compact or comfortable spacing.
- Set drawer background opacity.
- Choose an independent opening animation.

The app list also uses cached labels and icons, reusable grid cells, and package-change refresh handling.

### 6. Groups, widgets, and shortcuts

- Create rounded app groups on the home screen.
- Add or remove group members and rename or delete groups.
- Add Android-provided widgets through the widget picker.
- Move and resize supported workspace widgets.
- Add contact / direct-call shortcuts and adjust their icon size.

Widget availability and behavior depend on the provider app, Android version, and device manufacturer.

### 7. Wallpaper and personalization

Use a photo from the device or open Android's system wallpaper picker. Combine the wallpaper with one of the built-in color themes, icon artwork treatments, clock styles, and page transitions.

### 8. A personal launcher signature

The home-screen signature is editable in Home Studio:

`Home Studio → Launcher identity → Home brand label`

The default is **Q.Launcher**. Custom labels are limited to **10 words**. The same saved label is used in the launcher identity areas.

---

## Getting started

### Install and set as the default launcher

1. Download the latest successful APK artifact from the [Build Quantum Launcher APK workflow](https://github.com/DS-ann/Quantum-Launcher/actions/workflows/Build.yml).
2. Install the APK on your Android device.
3. Press the device's **Home** button.
4. When Android asks which home app to use, select **Quantum Launcher** and choose the default option.
5. If Android does not show a chooser, open **Settings → Apps → Default apps → Home app** (the exact menu name varies by device) and select Quantum Launcher.

### Essential navigation

| Gesture / action | Result |
|:--|:--|
| Hold an empty area on Home screen 1 for about 2 seconds | Open **Home Studio** |
| Swipe left or right | Switch between the two home pages |
| Swipe up on Home | Open the app drawer |
| Swipe down on Home | Open Control Centre / Android Quick Settings |
| Hold a home-screen app icon, then drag | Move the app |
| Hold an item in place for about 2 seconds | Open its available actions |

**Quick Settings note:** opening Android Quick Settings with the downward launcher gesture uses the launcher's accessibility service. Enable **Quantum Launcher** in Android Accessibility settings when prompted. The service description states that it does not read or collect screen content.

### First customization to try

Open Home Studio and start with the home grid, icon artwork, clock style, page animation, and color theme. Then set your own brand label under **Launcher identity**.

## Compatibility

Quantum Launcher is configured with **Android 6.0 (API 23)** as its minimum SDK and is intended for Android 6.0 and newer.

| Build setting | Configuration |
|:--|:--|
| Minimum SDK | 23 |
| Target SDK | 37 |
| Compile SDK | 37 |
| Java source / target compatibility | Java 8 |
| Application ID | `com.dsann.launcher` |
| Version name | `18.7.0` |
| Version code | `180700` |

Android's widget framework, default-home selection, wallpaper picker, accessibility settings, and permission flows can differ by OS version and manufacturer. Compatibility settings do not replace real-device testing.

## Building from source

### Requirements

- JDK 17
- Android SDK Platform 37
- Android Build Tools 37.0.0
- Gradle 9.3.1
- The repository's configured release-signing secrets when producing the signed release APK through GitHub Actions

### Build locally

From the repository root:

```bash
gradle assembleDebug
```

To build the release variant locally:

```bash
gradle assembleRelease
```

The release variant is signed only when the signing keystore environment is configured. The repository's GitHub Actions workflow prepares the configured PKCS#12 signing key from repository secrets and verifies the resulting APK signature.

### Build a signed APK with GitHub Actions

1. Open [Actions → Build Quantum Launcher APK](https://github.com/DS-ann/Quantum-Launcher/actions/workflows/Build.yml).
2. Select **Run workflow**.
3. Keep the branch set to `main`.
4. Start the workflow and open the completed run.
5. Download the **Quantum-Launcher-18.7.0-signed-APK** artifact.

The workflow builds the release APK, verifies its signature, and uploads the `.apk` directly as an artifact. It does not create a GitHub Release. Artifacts are configured to be retained for 14 days.

Release signing secrets must remain in GitHub Actions Secrets. Never commit keystores, signing passwords, private keys, or generated APKs to the repository.

## Project structure

```text
.
├── .github/
│   └── workflows/
│       └── Build.yml
├── app/
│   ├── build.gradle
│   └── src/main/
│       ├── AndroidManifest.xml
│       ├── java/com/dsann/launcher/
│       │   ├── MainActivity.java
│       │   ├── BlankActivity.java
│       │   ├── HomePageController.java
│       │   ├── HomePageModel.java
│       │   ├── LauncherAppAdapter.java
│       │   ├── LauncherDrawerController.java
│       │   ├── LauncherScreenTransitions.java
│       │   ├── LauncherIconDrawable.java
│       │   ├── WidgetController.java
│       │   ├── WidgetInteractionController.java
│       │   └── LauncherUiUtils.java
│       └── res/
│           ├── anim/
│           ├── mipmap-xxhdpi/
│           ├── values/
│           └── xml/
├── build.gradle
├── gradle.properties
└── settings.gradle
```

### Architecture at a glance

| Component | Responsibility |
|:--|:--|
| `MainActivity` | Main launcher experience, navigation, Home Studio, clock, drawer, gestures, and workspace integration |
| `HomePageModel` | Stable two-page workspace model and saved page membership |
| `HomePageController` | Home-page rendering, layout, and item positioning |
| `LauncherAppAdapter` | App-cell rendering and app label / icon presentation |
| `LauncherDrawerController` | Drawer behavior and presentation |
| `LauncherScreenTransitions` | Home / drawer transition effects |
| `LauncherIconDrawable` | Icon shape and artwork rendering |
| `WidgetInteractionController` | Widget movement, resizing, and workspace interaction |
| `BlankActivity` | Launcher identity page shown by the app's drawer entry |

The project uses Java and Android's native view system, keeping the UI foundation close to the platform rather than introducing a third-party UI framework.

## Testing and known limits

The GitHub Actions workflow checks that the release APK builds and that its signature verifies. **A successful workflow is not the same as a full device test.**

Before treating a build as ready for daily use, test it on the Android versions and devices that matter to you. In particular, verify:

- Home and drawer gestures, including reverse swipes during transitions.
- App movement, page-edge transfer, and layout recovery after rotation.
- Widget add, resize, restore, and provider-specific behavior.
- Clock sizing and text placement across both pages.
- Wallpaper selection and default-home behavior.
- Accessibility-mediated Quick Settings access.

If something behaves differently on a device, include the Android version, device model, steps to reproduce, and a log or screenshot where possible.

## Contributing

Changes should preserve the project's Android 6.0 minimum support unless a compatibility change is intentional.

When contributing:

1. Keep the existing Java / native-view architecture in mind.
2. Avoid adding heavyweight dependencies for effects that can be implemented with platform APIs.
3. Preserve saved workspace positions when changing grid, icon, widget, or orientation behavior.
4. Test both home pages and the drawer after gesture or layout changes.
5. Distinguish a successful CI build from behavior verified on a physical device.

## License

No license is currently included in this repository. Until a license is added, you should not assume that the source is available for unrestricted reuse, redistribution, or modification.

---

<div align="center">

  **Quantum Launcher**  
  <sub>Make the space you come home to feel like yours.</sub>

</div>
