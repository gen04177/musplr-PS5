# musplr

This is a simple music player compatible with MP3 and OGG formats, developed in C using SDL2, designed to be played on a jailbroken PS5 (1.xx-5.xx).

## Prerequisites
- elfldr.elf
- shsrv.elf
- ftpsrv.elf

## How to Use
1. Send the elfldr.elf payload to port 9020.
2. Send the shsrv.elf payload to port 9021.
3. Send the ftpsrv.elf payload to port 9021.
4. Copy the musplr.elf payload to `/data` directory on your PS5.
5. Execute `telnet [PS5-IP] 2323`.
6. Run the command `hbldr /data/musplr.elf --help`

## Known limitations:

- Audio files must be less than 50MB.
- File names must be less than 64 characters long.
- List of supported characters for file names: abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789&()'´’-_. ÁÀÃÂáàãâÉÊéêÍÎíîÓÔÕóôõÚÛúûÇç

This app was tested with a list containing 500 audio files and no problems were detected.

## Credits
- ps5-payload-sdk
