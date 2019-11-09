# gr-multitransmit-rpitx
A simple AM/FM/SSB modulator for rpitx in GRC 3.7x

To connect run rpitx and set frequency on the Raspberry pi for example:

while true; do (nc -l 8011; dd if=/dev/zero bs=4096 count=30); done | sudo rpitx -i- -m IQFLOAT -f 434000

Then set the TCP sink address and port (8011) to the location of the pi running rpitx.
