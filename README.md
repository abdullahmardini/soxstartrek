# soxstartrek
Simple systemd timer to play some white noise using sox to help me sleep.

Inspired by: https://news.ycombinator.com/item?id=6513338

## Installation

Place the `soxstartrek.timer` and `soxstartek.service` files in `/etc/systemd/system/` and enable with `sudo systemctl daemon-reload && sudo systemctl enable --now soxstartrek.timer`.


## Random Notes
1. I personally am running this *smart speaker* with pulseaudio system-wide (https://www.freedesktop.org/wiki/Software/PulseAudio/Documentation/User/SystemWide/) which is generally considered to be a bad idea, but is necessary if you have no logged in users.
	*	You may need to alter the User line if this is true for you.

See https://askubuntu.com/questions/789465/generate-white-noise-to-calm-a-baby for ideas about altering this for your use.
