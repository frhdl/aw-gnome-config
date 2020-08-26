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

#Move autostart file
sudo mv awstart.sh /etc/init.d/

#Set permissions and move scripts
sudo chmod +x *.sh && \
mv *.sh activitywatch/
```
```shell
#Move program to opt folder
mkdir ~/.local/opt/ & \
sudo mv ~/Downloads/aw/activitywatch ~/.local/opt/
```
```shell
#Set permissions of autostart file
cd /etc/init.d/
chmod +x awstart.sh
```
```shell
#Add aliases to your .bash_aliases
 alias awstart='nohup ~/.local/opt/activitywatch/start.sh > /dev/null &'
 alias awstop='~/.local/opt/activitywatch/kill.sh'
```