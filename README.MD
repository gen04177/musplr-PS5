# musplr

This is a simple music player compatible with MP3, WAV and OGG formats, developed in C using SDL2, designed to be played on a PS5 Jailbreak (3.xx-4.xx).

## Prerequisites
- elfldr.elf
- shsrv.elf
- ftpsrv.elf

## How to Use
1. Send the elfldr.elf payload do port 9020.
1. Send the shsrv.elf payload to port 9021.
2. Send the ftpsrv.elf payload to port 9021.
3. Copy the musplr.elf payload to `/data` directory on your PS5.
4. Copy the arial.ttf font to `/data` directory on your PS5.
4. Execute `telnet [PS5-IP] 2323`.
5. Run the command `hbldr /data/musplr.elf --help`

## Known limitations:

- Audio files must be less than 10MB.
- File names must be less than 64 characters long.
- List of supported characters for file names: abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789&()'´’-_. ÁÀÃÂáàãâÉÊéêÍÎíîÓÔÕóôõÚÛúûÇç

This app was tested with a list containing 500 audio files and no problems were detected.

## Credits
Credits to J. Tornblom for the SDK, SDL2 port for PS5, and required payloads.
