# Spotisort
Spotisort is a small script to sort Spotify playlists by release date. It allows your playlist to stay tidy and keep new releases always on top.

## Requirements
- Spotipy module (`pip3 install spotipy`)
- [a Spotify app](https://developer.spotify.com/dashboard/applications)
- To whitelist your Redirect URI in the Spotify app settings as in figure

![Redirect URI in the app settings](images/redirecturis.png)

## Installation
```
git clone https://github.com/alessiocelentano/spotisort
```
 
Remember to edit `config.ini` with the data you got from the Spotify app.

Also, in order to be able to use the command everywhere in the terminal, I suggest to follow these steps:

```
$ cd spotisort
$ cp spotisort config.ini .cache /usr/local/bin
$ sudo chmod 777 /usr/local/bin/.cache
```

If `.cache` doesn't exist, run Spotisort first.

## Usage
Run `./spotisort`, add your songs in a throwaway playlist (in the screenshot above I called it "Add Later") and select the playlist you want to add songs to. The script will delete songs from the throwaway playlist and add them to the chosen playlist. Additionally you can exclude some songs in case you have multiple playlists.

![screenshot](images/screenshot.png)

 ## License
 MIT
