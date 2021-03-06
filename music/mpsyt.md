# mps-youtube

> Terminal based YouTube player and downloader.

- [`mps-youtube`](https://github.com/mps-youtube/mps-youtube)

---

## Install & Setup

Download the standalone binary:

- [`mpsyt-0.2.8.exe`](https://github.com/mps-youtube/mps-youtube/releases/download/v0.2.8/mpsyt-0.2.8.exe)

Or install with `pip`:

1. Download and install `python3` & `pip`

   ```sh
   # Install python3 with Chocolately
   $ choco install python3 -y
   # Verify python and pip installations
   $ python -V
   # Python 3.7.3
   $ python -m pip -V # or $ pip -V
   # pip 19.0.3
   ```

2. Upgrade `pip` if required

   ```sh
   # Upgrade pip installation
   $ python -m pip install --upgrade pip
   # List pip packages
   $ python -m pip list
   # Verify upgrade
   $ python -m pip -V
   # pip 19.1.1
   ```

3. Install `mpv` & `ffmpeg`

   ```sh
   # Install mpv with chocolately
   $ choco install mpv -y
   # Install ffmpeg with chocolately
   $ choco install ffmpeg -y
   # Check mpv and ffmpeg installations
   $ mpv -V
   # mpv 0.29.1
   $ ffmpeg -version
   # ffmpeg version 4.1.3
   ```

4. Install required dependencies

   ```sh
   # Install colorama (optional)
   $ python -m pip install colorama
   # Install youtube-dl
   $ python -m pip install youtube_dl
   # Verify youtube-dl installation
   $ youtube-dl --version
   # 2019.06.21
   ```

5. Install `mps-youtube`

   ```sh
   # Install mps-youtube
   $ python -m pip install mps-youtube
   # Verify mps-youtube installation
   $ mpsyt --version # or mpsyt -v
   # mpsyt version : 0.2.8
   ```

6. Run `mps-youtube` and set configuration

   ```sh
   # Start mps-yotube
   $ mpsyt
   # Set configuartion
   $ set order views
   $ set encoder 3
   $ set audio_format m4a
   $ set columns user:14 date rating views likes dislikes category:9
   $ set api_key AIzaSyBQKmHt0Gm0-i12JEp0W-kN-gFOF_cfX1c
   ```

Issues with provided API key:

- [`issues/551`](https://github.com/mps-youtube/mps-youtube/issues/551)
- [`issues/970`](https://github.com/mps-youtube/mps-youtube/issues/970)

---
