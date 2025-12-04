Super quick and dirty!

The ezarr submodule will go out and create the individual users and folder structure for the servarr stack. It will create a `docker-compose.yml` file as well, but I substituted a couple things for variables in the .env file. 

The homepage for the submodule is: https://github.com/Luctia/ezarr

It explains what each arr does. The only one that is listed but does not work is Readarr. It is for ebooks and audiobooks. There are some alternatives that I'm looking into to "sub-in" but haven't gotten there yet. If you don't feel like going to the other repo the tldr is:

```
# python main.py

# << Answer a bunch of questions about what to install >>

# ???

# Profit!
```

The questions will be what you want installed. Quick list and a one or two word description:
- Sonarr: You tell it what shows you want to watch and it will scour "indexers" to find all the episodes using TVDB as a source.
- Radarr: Same thing as Sonarr, but for movies.
- Bazarr: Companion app to Sonarr and Radarr to go out and make sure everything has the right kind of subtitles you want. Haven't messed with it yet.
- Lidarr: Same as Sonarr and Radarr but for music
- Readarr: This one does not work. The developer is no longer supporting it. There are other options I'm exploring.
- Mylar3: Comic books! Apparently tricky to setup? Haven't touched it yet.
- Audiobookshelf: self-hosted audiobook and podcast server
- Homarr: Dashboard thing. There is a lot more to it, but that was the dashboard.
- Prowlarr: Tracks the Indexers (basically keeps track of what files are where on the news groups or torrent sites)
- Jackett: Alternative to Prowlarr, I didn't set it up or install it. Didn't fit the asthetic
- FlareSolverr: Proxy server to bypass Cloudflare protection. Used with a lot of Torrent indexers it seems.
- qBittorrent: Torrent client, web based
- SABnzbd: Like qBittorrent, but for news groups
- Plex: Self explanatory
- Overseerr: Show and movie request management and discovery tool. 
- Tautulli: Apparently integrates with Plex to track who is watching when where and why... *shrug*
- Jellyfin: Alternative to Plex
- JellySeerr: Like Overseer, but for Jellyfin.

This all will absolutely run on Docker Desktop in WSL.
