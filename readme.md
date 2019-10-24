# playlist2podcast

A python script to convert a YouTube playlist to an mp3 podcast. Utilises youtube-dl and ffmpeg.

Only tested on windows - should work on Linux/MacOS if you provide youtube-dl and ffmpeg paths.

## Requirements:

youtube-dl: download the latest windows binary and put it in the same folder as the script  
ffmpeg: download the latest windows binary and put it in the same folder as the script  

## Command-Line Arguments

| Switch    | Usage                                             |
|-          |-                                                  |
| `-p`      | URL of YouTube Podcast                            |
| `-t`      | String to embed as the podcast title metadata     |
| `-a`      | String to embed as the podcast artist metadata    |
| `-y`      | Path to youtube-dl executable                     |
| `-f`      | Path to ffmpeg executable                         |

## Notes

* Tracks are automatically numbered based on their position in the playlist.
* Artist, podcast title, and track number are embedded into the finished mp3 file.
* track number and track title are set as the file name for easy organization.
* Automatic removal of non-valid characters from the file name.