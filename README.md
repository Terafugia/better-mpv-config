# better-mpv-config

Version 1.0 is out! It's an improved MPV Media Player configuration file that:

- has useful defaults
- offers profiles
- hides the window title bar
- auto-hides the cursor after 1 second
- saves the seekbar position on exit
- uses an extra large RAM cache
- normalizes audio
- sets Color Space, Dithering, Debanding, Subtitles
- sets Motion Interpolation, Anti-Ringing and Upscaling & Processing
- now uses shaders for improved visuals
- improves profiles for https and http protocols
- adds no additional cruft...

## Requirements

* official MPV Player: https://mpv.io/
* PC with at least 4GB of RAM
* PC with integrated (CPU) or discreet GPU (card)

![usage preview](https://raw.githubusercontent.com/hl2guide/better-mpv-config/master/preview%20image.png)

Includes selected lines from Mike Connelly's work on MPV.

* GitHub Repo: https://github.com/classicjazz/mpv-config
* Article: https://freetime.mikeconnelly.com/archives/5371

## Configuration

Please Note: this config will need your own additional work if you happen to use a Mac PC (since Macs only support OpenGL).

### Windows Users
Extract the ZIP in the releases section to the location: `%APPDATA%/mpv/`

### Linux Users
* You can put all of the options in configuration files which will be read every time mpv is run.
* The system-wide configuration file 'mpv.conf' is in your configuration directory (e.g. `/etc/mpv` or `/usr/local/etc/mpv`).
* The user-specific one is `~/.config/mpv/mpv.conf`.

## Usage

* Save to the correct location (as above) for your Operating System.
* Next time MPV is launched, and thereafter the settings should load. (command line or GUI)

### Vital Notes

If you run into playback issues then remove the __first 5 lines__ and save changes to the file 'mpv.conf'.

## Custom Profiles
This config uses specific naming convensions for shorter easier typing.

By default MPV plays video streams at the highest available quality (even 4K on a 1080p display).

Using my custom profiles allows for finer grain control over quality and framerate.

### Naming Convensions

Profiles use the format: `\<letter\>\<number\>`

The _letter_ referring to the video's __quality level__ and the _number_ the __FPS (frames per second)__.

| 480p | 720p | 1080p | 1440p (2.5K) | 2160p (4K) | 4320p (8K) |
| ------ | ------ | ------ | ------ | ------ | ------ |
| Very Low  | Low | Medium | High | Ultra | Supreme |

| Very Low  | Low | Medium | High | Ultra | Supreme |
| ------ | ------ | ------ | ------ | ------ | ------ |
| V | L | M | H | U | S |

| 30 FPS | 60 FPS |
| ------ | ------ |
| 30 | 60 |

## Examples

__Using the "profile" switch__

#### Windows

4K @ 60 FPS:

`mpv.exe --profile=U60`

4K @ 30 FPS:

`mpv.exe --profile=U30`

1080p @ 60 FPS:

`mpv.exe --profile=M60`

1080p @ 30 FPS:

`mpv.exe --profile=M30`

#### Linux

Same as above but remove the `.exe` in the examples.
