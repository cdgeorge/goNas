# rpiplex


# Plex Media Scanner

```
if [ -f /usr/lib/plexmediaserver/Plex\ Media\ Scanner ]; then
   function pms () { echo Plex\ Media\ Scanner $*;sudo -H -u plex bash -c "export LD_LIBRARY_PATH=/usr/lib/plexmediaserver; /usr/lib/plexmediaserver/Plex\ Media\ Scanner $*"; }
fi
```

## Check access to the directories before adding them

```
sudo -u plex bash
```

## Add directories

```
pms --add-section Movie --type 1 --location /media/cdg/T7/MyPassport/Media/DVDs/Movie/ --lang dan
pms --add-section Tv --type 2 --location /media/cdg/T7/MyPassport/Media/DVDs/Tv/ --lang dan
```

# Sources
- https://roboticsbackend.com/enable-ssh-on-raspberry-pi-raspbian/
- https://pimylifeup.com/raspberry-pi-plex-server/
- https://github.com/cdgeorge/ups3
- https://howchoo.com/g/mwnlytk3zmm/how-to-add-a-power-button-to-your-raspberry-pi
