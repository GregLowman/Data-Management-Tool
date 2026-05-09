# Media Organizer

A cross-platform media management tool built for an independent drone footage company. Scans a source folder and automatically sorts photos and videos into platform-specific directories based on file type and rotation metadata, converts CSV captions into organized text files, and separates videos by aspect ratio for Instagram Reels vs YouTube.

## Files

| File | Description |
|------|-------------|
| `database.py` | Core organizer — builds directory structure, sorts media, processes captions, and routes videos by rotation via exiftool |
| `test_file.py` | ffprobe utility for detecting video rotation |

## Requirements

- Python 3.x
- [exiftool](https://exiftool.org/) installed and accessible at the path defined by `sorting_software` in `database.py`

## Usage

1. Update `starting_folder` and `ending_folder` in `database.py` to match your source and destination paths
2. Run the organizer:

```bash
python database.py
```

## Platform Support

Configured for both Windows and macOS.
