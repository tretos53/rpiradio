# SSRPR - SSRPRADIO - Super Simple Raspberry Pi Radio

## Version 1.

1. Tested on Rapsberry pi 3 model B v 1.2 with USB sound card (https://www.ebay.co.uk/itm/392807460055) pluged in and Raspberry Pi OS Lite 32Bit Release 2020-12-02 installed.
2. Connect to the internet.
3. Install by running below commands. Replace YT_PLAYLIST with your YouTube playlist URL.

`curl -H 'Cache-Control: no-cache' -sSL https://raw.githubusercontent.com/tretos53/ssrpr/main/ssrpr.sh | bash $0 YT_PLAYLIST`

4. Set sudo raspi-config to autologin to console.

## Known Issues
1. This script uses .bashrc to start the Tizonia. There is a known issue starting Tizonia at boot.
2. To avoid getting Youtube quota error follow https://tizonia.org/news/2020/03/08/release-0-21-0/
3. There is something wrong with --shuffle option in Tizonia. It often shuffle the same few songs, even of the playlist contains 50 songs.
