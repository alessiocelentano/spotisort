# Spotisort
Spotisort is a small script to sort Spotify playlists by release date. It allows your playlist to stay tidy and keep new releases always on top.

![screenshot](screenshot.png)

## Requirements
- Python3;
- A Spotify throwaway playlist;

## Installation
You'll need Spotipy in order to run the script
```
pip3 install spotipy
```
Also, you have to [create a Spotify app](https://developer.spotify.com/dashboard/applications) and edit `config.ini` with your data. Remember to whitelist your Redirect URI in the app settings.

![Eedirect URI in the app settings](redirecturis.png)

## Usage
Run `./spotisort`, add your songs in a throwaway playlist (in the screenshot above I called it "Add Later") and select the playlist you want to add songs to. The script will delete songs from the throwaway playlist and add them to the chosen playlist. Additionally you can exclude some songs in case you have multiple playlists.
