# Coqui TTS GUI solution
Graphical user interface by AceOfSpadesProduc100 for using released TTS and vocoder models in the form of a text editor, made using Tkinter.
This is an addon for TTS 0.0.10, as it should hopefully already be part of a version after it.
![Preview](./Screenshot_2021-03-22_173624.png)

## How to use
- Download or clone from this repository: https://github.com/coqui-ai/TTS
- Copy gui.py and synthesize.py into TTS/bin, overwriting the existing synthesize.py
- Install from source as explained in the repository's readme: 
```bash
pip install -e .
```
- Install simpleaudio:
```bash
pip install simpleaudio
```
- Run the following command:
```bash
tts --start_gui
```
- (Linux users) Install the following first:
```bash
sudo apt install python3-tk
sudo apt-get install -y python3-dev libasound2-dev
```
- (WSL2 users) This program requires a desktop environment (https://medium.com/@riley.kao/wsl2-ubuntu20-04-gui-remote-desktop-connection-rdp-2bbd21d2fa71), or else you'll get errors about display variables not being set.
- NOTE: It will take a while to generate audio, especially if you don't have a CUDA-compatible GPU. You should see your CLI to see what's happening.
- DEV NOTE: Changes to synthesize.py and manage.py may require changes to gui.py.
