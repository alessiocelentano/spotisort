# Spotisort
Spotisort is a small script to sort Spotify playlists by release date. It allows your playlist to stay tidy and keep new releases always on top.

## Requirements
- [Spotipy](https://github.com/spotipy-dev/spotipy) module (`pip3 install spotipy`)
- A [Spotify app](https://developer.spotify.com/dashboard/applications)
- [Wrap Genius](https://github.com/fedecalendino/wrap-genius) module (`pip3 install wrap-genius`) [optional]
- A [Genius token](https://genius.com/api-clients/new) (optional)


## Installation
```
git clone https://github.com/alessiocelentano/spotisort
```
 
Remember to edit `config.ini` with the data you got from the Spotify app. The Redirect URI inserted has to be whitelisted in the Spotify app settings as in figure.

![Redirect URI in the app settings](images/redirecturis.png)

## Usage
``` bash
# Genius search active (if configured). Incomplete release date will be searched on Genius.
$ ./spotisort

# Don't search release dates on Genius. Faster but less accurate.
$ ./spotisort --no-genius
# or
$ ./spotisort -ng
```

![screenshot](images/screenshot.png)

 ## License
 MIT
