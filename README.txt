Seirei Senshi Spriggan English Version
================================

English version patch for Seirei Senshi Spriggan on PC Engine CD-ROM².

This version provides the following:

  English subtitles for voiced cutscenes and in-level dialogue
  Translated title cards, menus and credits
  QoL features
    Auto-save progression and options settings
    Shorter load times and other bug fixes

English text that was already present in the game hasn't been modified except for obvious errors.

Note on audio sync: Subtitle timing was calibrated for original PC Engine hardware. Audio synchronization can vary substantially under emulation. If the audio and text drift out of sync, especially during in-level dialogs, try another emulator.

Note on BIOS: The patch has been tested and will work with all system card versions. In fact, system cards older than 3.0 have a nicer 12x12 font for menu/credits text, I recommend it =).

Downloads
=========
patches: 
https://github.com/gagnonpl/spriggan-en/releases/download/v1.1/spriggan-english-track02-v1.1.xdelta
https://github.com/gagnonpl/spriggan-en/releases/download/v1.1/spriggan-english-track27-v1.1.xdelta
xdelta: https://github.com/jmacd/xdelta/releases

Patching
========

Tracks 02 and 27 are the data tracks and are patched separately with xdelta3.
1. Copy the original Track 02 and Track 27 BIN files to the directory where you want the patched files.
2. Apply each patch separately:
  xdelta3 -f -d -s "Seirei Senshi Spriggan (Japan) (Track 02).bin"  spriggan-english-track02-v1.1.xdelta "Seirei Senshi Spriggan (Japan) (Track 02)-patched.bin"
  xdelta3 -f -d -s "Seirei Senshi Spriggan (Japan) (Track 27).bin" spriggan-english-track27-v1.1.xdelta "Seirei Senshi Spriggan (Japan) (Track 27)-patched.bin"
3. Replace the original Track 02 and Track 27 files with the patched files, renaming the patched files to their original filenames.
4. Keep the original .cue file and all other track files unchanged.

Note that track 27 contains a copy of the data in track 02, used as a redundant copy in case it cannot be read correctly by the PCE.  Patching it should only matter if you play with a disc on original hardware.

Hashes
=========

Expected original files:

Redump set:   NEC - PC Engine CD & TurboGrafx CD
Redump name:  Seirei Senshi Spriggan (Japan)

Seirei Senshi Spriggan (Japan) (Track 02).bin
  CRC32:        14DB03F6
  MD5:          b954963517d3f32e7bf32b853eb08b49
  SHA-1:        b2de7d99dd68593a23b7baed3966c3e599f0ee4b

Seirei Senshi Spriggan (Japan) (Track 27).bin
  CRC32:        4C484E7B
  MD5:          be1c30e45be4d0d74aa4c1961a7c217b
  SHA-1:        1d75203d18641be129650869e4beb120e854dbe9

Patched output images:
Seirei Senshi Spriggan (Japan) (Track 02).bin
  CRC32:        C4CC8CC3
  MD5:          ddf338a7e468c7b6f4a483dc6dda06c8
  SHA-1:        d9bc840ab10cecae6cb82a8915f75a06d84340d3
Seirei Senshi Spriggan (Japan) (Track 27).bin
  CRC32:        07A6FA40
  MD5:          9adcb8637667afdb16b15abc7a6e1771
  SHA-1:        859862f835a1a57181cc14d4b80d19ed903dbff1

ROMhacking.net
==============
https://www.romhacking.net/translations/7742/


Credits
=======

English version by Luke Gagnon.
