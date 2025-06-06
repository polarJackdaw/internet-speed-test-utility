# ISTU Internet Speed Test Utility

Python GUI tool to test, log, and visualize internet speeds with optional background music.

## Features

- Internet speed testing (Download, Upload, Ping, ISP, Country, Location)
- Results logged with timestamp to `internet_data.txt`
- Scatter plot of test results using `matplotlib`
- Automatic testing at custom intervals
- Sound effects with mute toggle
- Custom background music support (`.mp3` playback)
- Custom Themes with theme_manager.py

## Theme Customization & Theme manager

- Change the colors of the program and the scatter plot by editing settings.json
- Run theme_manager.py to Apply, Delete or Add themes.
- "Save Current As New" will save settings.json as a new theme
- More & better themes coming soon...

## Custom Music

You can add your own `.mp3` files to play as background music.

### How to Add Music:

1. Navigate to the `sounds/music/` directory.
2. Place your `.mp3` files into this folder (other formats are not supported).
3. Click the **"Music ON"** button to start background playback.
4. The app will randomly loop through all `.mp3` files in that folder.
5. To skip a song, toggle the music OFF and then ON again.

### Custom Music Folder

Change the default music folder in settings.json

Make sure the path has double slashes (example.):
{
  "music_folder": "C:\\Users\\polarjackdaw\\Music\\mp3\\"
}

### How to Customize Sound Effects:

1. Navigate to the `sounds` folder.
2. Replace the `.wav` file with your own. Do not change the filename or file format!


## Requirements

The script requires the following dependencies:
- `speedtest-cli`
- `pandas`
- `matplotlib`
- `numpy`
- `tkinter`
- `Pillow`
- `pygame`

Install dependencies using the following command:
pip install -r requirements.txt
