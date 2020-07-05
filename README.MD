# Download
Check the [lastest release from github](https://github.com/ActivityWatch/activitywatch/releases).

# Installation

## to write ```install.sh``` script...

```shell
#Extract installation
cd ~/Downloads & \
mkdir aw & \
mv activitywatch-v* aw & \
cd aw & \
unzip activitywatch-v*

#Download config files 
gitclone https://github.com/getchipman/aw-gnome-config.git & \
cd aw-gnome-config

#Move autostart files
mv *.desktop ~/.local/share/applications/

#Set permissions and move scripts
sudo chmod +x *.sh && \
mv *.sh activitywatch/
```
```shell
#Move program to opt folder
mkdir ~/.local/opt/ & \
sudo mv ~/Downloads/aw/activitywatch ~/.local/opt/
```

