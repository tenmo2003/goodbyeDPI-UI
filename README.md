![icon](https://github.com/user-attachments/assets/e67c903c-e649-4560-8483-3d0bde4d1e0f)

Welcome to GoodbyeDPI UI! This is a user interface for the [goodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI), [zapret](https://github.com/bol-van/zapret), [byeDPI](https://github.com/hufrea/byedpi) and [spoofDPI](https://github.com/xvzc/SpoofDPI) projects.

> [!NOTE]
> This is an English-first fork of [Storik4pro/goodbyeDPI-UI](https://github.com/Storik4pro/goodbyeDPI-UI). See [About this fork](#about-this-fork) for what is different.

## Description

GoodbyeDPI UI provides a convenient graphical interface for managing GoodbyeDPI, Zapret, ByeDPI and SpoofDPI. With it you can easily change DPI settings and run the application in the system tray.
> [!IMPORTANT]
> Already using other variants? Import the settings from your BAT or CMD file! Click the `"Load settings from file"` button on the Zapret or GoodbyeDPI page

## About this fork

Same application, same engines and tools as upstream. The differences are:

- **Default language is English.** A fresh install starts in English (`language = EN` in `data/settings/settings.ini`). Russian is still available in Settings > Personalization.
- **The updater does not use the upstream repository.** Application updates are read from the repository set in `UPDATE_REPO` in `src/_data.py`. It is set to `tenmo2003/goodbyeDPI-UI`. While it is empty the application does not check for or download application updates from anywhere.
- The remaining Russian text in the English localization and this README were translated.

Help, wiki, website and issue links inside the application still point to the upstream project. Engine components (GoodbyeDPI, Zapret, ByeDPI, SpoofDPI) are still downloaded from their own repositories, and their configs from `Storik4pro/goodbyeDPI-UI-configs` (`CONFIGS_REPO` in `src/_data.py`).

### Set your update repo

1. Open `src/_data.py`.
2. Set `UPDATE_REPO` to your GitHub repository in `owner/name` form, for example:

   ```python
   UPDATE_REPO = "your-name/goodbyedpi-ui"
   ```

3. Publish releases in that repository the same way upstream does: the release tag is the version (the `VERSION` value in `src/_data.py`, e.g. `1.2.14`), with a `.cdpipatch` asset for in-app patching and/or a `.zip` asset (`_portable.zip` layout, top-level folder `goodbyeDPI UI/`) for the full update.

Leave `UPDATE_REPO` empty to keep the updater disabled.

## Installation

> [!IMPORTANT]
> The upstream installation guide is on the [GoodbyeDPI UI website](https://storik4pro.github.io/cdpiui)

### Requirements

- Windows 10 64bit build 15063 or higher

>[!IMPORTANT]
>On Windows 10 versions older than 1809 the "View goodbyeDPI output" feature does not work

### Installation steps

1. Download the latest version of goodbyeDPI UI from the releases page of this fork's repository (this fork has no published releases until you publish them; see [Set your update repo](#set-your-update-repo))
2. Turn off your antivirus
3. Install goodbyeDPI UI
4. Add the goodbyeDPI.exe file to your antivirus exclusion list
5. Turn your antivirus back on
6. Congratulations! You have completed the installation!

## Usage
![1](https://github.com/user-attachments/assets/8e97ea96-3cb9-49c8-b5ff-6bc4a8d57a38)
<details><summary>More screenshots</summary>
  
![3](https://github.com/user-attachments/assets/f108723e-93ff-4e63-a775-42b2ef6375cb)
![4](https://github.com/user-attachments/assets/13f4b1bb-024d-431f-9842-6bb380d1e449)
![2](https://github.com/user-attachments/assets/cb74727b-2c32-491e-8b4c-426a4a7d7921)

</details>


1. Launch the application.
2. Choose the engine (zapret/goodbyeDPI)
3. Choose the region and DNS settings.
4. Press the button to start or stop the process.
5. Minimize the application to the system tray

## Autorun

To add the application to autorun, follow these steps:

1. Launch the application.
2. Enable the autorun option in the application settings.

## Contributing

Contributions to the project are welcome! If you have ideas or suggestions, please create an issue or a pull request.

## Acknowledgements

Special thanks to [ValdikSS](https://github.com/ValdikSS), [bol-van](https://github.com/bol-van/), [xvzc](https://github.com/xvzc) and [hufrea](https://github.com/hufrea/)

## License and attribution

GoodbyeDPI UI is created by [Storik4pro](https://github.com/Storik4pro) and licensed under the [Apache License 2.0](LICENSE). This fork keeps the same license; the changes made in it are listed in [About this fork](#about-this-fork).
