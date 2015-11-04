IwSound
=======

The IwSound modules provides a wrapper around Marmalade System's s3eSound
API, providing more convenient higher-level APIs, and allowing it to interact
with Marmalade Studio's IwResManager resource management system.

It also uses a sound generation callback to provide ADPCM compressed sound that
is decompressed on the fly.

SoundEngine provides functionality including:
- Load and play WAV files, either directly by file name or though IwResManager
- Support for PCM and ADPCM formats
- Sound materials (CIwSoundSpec class)
- Sound groups (controlling how many channels can be used)
- Easy control of volume, pitch, looping, etc.

It is based on the example IwSound/SoundEngine module shipped with the Marmalade
SDK, but with additional features.

SoundEngine.mkf is not designed to be built directly as a library. It can be
included in an MKB project file using: subproject IwSound
