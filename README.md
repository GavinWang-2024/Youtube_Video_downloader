# YouTube Video Downloader

This Python script allows you to download YouTube videos using `pytube` library with a GUI for selecting the download directory.

## Requirements

- Python 3.x
- `pytube`
- `tkinter`
- `certifi`

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/Youtube_video_downloader.git
   
   cd Youtube_video_downloader

2. Create and activate a virtual environment (optional but recommended):
   ```
   python3 -m venv myenv

   source myenv/bin/activater

3. Install packages:
   ```
   pip install pytube certifi



## Usage

### Run the script:
  ```
  python youtube_video_downloader.py
  ```

1. Enter the YouTube video URL when prompted.
2. Select the folder to save the video through the file dialog.

## Functions
```download_video(url, save_path)```
Downloads the YouTube video at the given URL and saves it to the specified directory. Filters streams for progressive download and MP4 format. Selects the highest resolution stream available.

```open_file_dialog()```
Opens a dialog for selecting a directory. Returns the selected directory path.

```SSL Configuration```
ssl._create_default_https_context = ssl._create_unverified_context disables SSL verification for the script to run without errors. certifi provides Mozilla's CA Bundle, ensuring the script uses up-to-date and reliable certificates.
