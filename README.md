# Musicly

Automated tool built on Raspberry Pi to scan, organize, tag, and sort MP3 music files from external/non-Apple devices. Edits metadata (artist, album, genre), creates structured folders (e.g., Artist/Album/Genre), handles batches, and avoids data loss with error checking.

## Features
- Scans mounted storage for MP3 files
- Reads/edits ID3 tags using mutagen
- Sorts into folders by artist/album/year/genre (customizable rules)
- Duplicate detection and safe renaming
- Command-line interface for easy use on Pi

## Technologies
- Python 3 (currently converting to C#) 
- Raspberry Pi (Linux-based)
- Libraries: os, shutil, mutagen, etc.

## Installation & Setup
1. Clone the repo: `git clone https://github.com/AndresIXxH/musicly.git`
2. Install dependencies: `pip install -r requirements.txt` 
3. Run: `python main.py`
- Works on Raspberry Pi OS; connect external drive via USB.

## Usage Example
```bash
python musicly.py --source /media/usb/music --organize-by artist-album
