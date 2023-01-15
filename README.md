# amiga-esp-link

This document uses the excellent esp-link firmware available here:<br />
https://github.com/jeelabs/esp-link <br />

With the wifi-serial bridge we can connect a PC and an Amiga together just like with a null-modem cable (PC ⇄ Amiga) but without having to use a physical cable between the machines.

The esp-link will make it possible to do file transfers over Wi-Fi from the PC to the Amiga and vice versa using a file transfer protocol like `Zmodem` or `Kermit` on each end. A popular program for doing this on the Amiga was [Ncomm](https://aminet.net/search?query=ncomm) back in the days. On the PC side we can use for example `Tera Term` (Windows) or `Minicom` (Linux).

It's also possible to get Console output of diagrom displayed from your Amiga to your PC this way. No cable needed :)

No driver needs to be installed on the Amiga side as long as you don't want to replace the `serial.device` that comes with AmigaOS. A better replacement is `8n1.device` available in two versions on Aminet here: https://aminet.net/search?query=8n1  <br />
one is for AmigaDOS 2.04+ (ONLY V37+), pick the correct one for your system. I have successfully used the `8n1.device` driver at `38400` baud speed setting on a plain standard A500.

