# DSCC Tauri Dance Player Releases

Public download repository for DSCC Tauri Dance Player portable builds.

## Latest Download

Download the latest portable zip from the Releases page:

https://github.com/0dot77/theme-toon-dance-release/releases/latest

Unzip the file and run `dscc-tauri-dance-player.exe`.

The zip includes the runtime avatar/choreography media assets. Put the show video in the extracted `media` folder root.

## Spout Notes

Spout output is enabled in `config/show.local.json` and publishes the app window as `JejuToon_Dance`.

The bundled app starts the Spout sender script automatically, but the PC must have Python with:

```powershell
pip install SpoutGL PyOpenGL glfw opencv-python numpy
```

If `python` is not on `PATH`, edit `config/show.local.json` and set `spout.pythonExecutable` to the full `python.exe` path.

## MediaSync Notes

MediaSync is auto-started 4 seconds after the app starts. The default path is:

```text
C:\MediaSync_11_14_21_Player\MediaSyncM2\MediaSyncM2.exe
```

If the MediaSync install path is different, edit `config/show.local.json` and change `mediaSync.executable`.
