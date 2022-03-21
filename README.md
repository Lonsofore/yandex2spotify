# yandex2spotify
Simple Python script, that allow to import favorite tracks, playlists, albums and artists from Yandex.Music to Spotify

## Install requirments
```bash
pip3 install -r requirements.txt
```

Put your Spotify app credentials (get them [here](https://developer.spotify.com/dashboard/applications)) to importer.py, lines 15-17:
```python
CLIENT_ID = ''
CLIENT_SECRET = ''
REDIRECT_URI = ''
```

## Usage
1) Using credentials:
```bash
python3 importer.py -u <spotify_username> -l <yandex_login> -p <yandex_password>
```
2) Using token:
```bash
python3 importer.py -u <spotify_username> -t <yandex_token>
```

3) If you don't want to import some items (likes, playlists, albums, artists) you can exclude them by specifying ignore argument, for example:
```bash
python3 importer.py -u <spotify_username> -t <yandex_token> -i playlists albums artists
```
