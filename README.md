YouTube Video Downloader
A simple Python script to download YouTube videos using the pytube library and a GUI for selecting the download directory.

Requirements
Python 3.x
pytube
tkinter
certifi
Installation
Clone the repository:

sh
Copy code
git clone https://github.com/yourusername/Youtube_video_downloader.git
cd Youtube_video_downloader
Create and activate a virtual environment:

sh
Copy code
python3 -m venv myenv
source myenv/bin/activate
Install the required packages:

sh
Copy code
pip install pytube certifi
Usage
Run the script:

sh
Copy code
python youtube_video_downloader.py
Enter the YouTube video URL when prompted.

Select the folder to save the video through the file dialog.

Functions
download_video(url, save_path)

Downloads the YouTube video at the given URL and saves it to the specified directory.
Filters streams for progressive download and MP4 format.
Selects the highest resolution stream available.
open_file_dialog()

Opens a dialog for selecting a directory.
Returns the selected directory path.
SSL Configuration
Why ssl and certifi are used
Some systems may encounter SSL certificate verification issues.
ssl._create_default_https_context = ssl._create_unverified_context disables SSL verification for the script to run without errors.
certifi provides Mozilla's CA Bundle, ensuring the script uses up-to-date and reliable certificates.
