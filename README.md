# wowrealmchanger

**wowrealmchanger** is a shellscript that changes between World of Warcraft realms listed in your **realmlist.wtf** file, designed for players who play in multiple realms under Linux

## How to use this script

### Prepare your realmlist.wtf file

put every entry you want in your **realmlist.wtf** file, i.e:

```
set realmlist logon.warmane.com

set realmlist realm.wow-brasil.com
set patchlist 127.0.0.1

set realmlist 192.168.0.9
set patchlist 192.168.0.9

```

blank lines will be ignored, so you can safely put blank lines between entries if you want, except for **patchlist** entries, that should be in the next line following it's relative **realmlist** entry


### Install the script into your system
1. replace the value at line 4 with the absolute path to your `realmlist.wtf` file

2. give this script **execute** permission if needed:
 
 - `chmod +x wowrealmchanger`

3. copy or move it to a directory listed in your `$PATH` environment variable, i.e:
 
 - `sudo mv wowrealmchanger /usr/local/bin`
 
4. run `wowrealmchanger` from terminal any time you want to change between realms listed in your `realmlist.wtf` file. The script will list all entries and allow you to pick which of them you want to play next
