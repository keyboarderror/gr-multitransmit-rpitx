# gr-multitransmit-rpitx
A simple AM/FM/SSB modulator for rpitx in GRC 3.7x

To connect run on the pi:

while true; do (nc 192.168.0.x 8011; dd if=/dev/zero bs=4096 count=30); done | sudo rpitx -i- -m IQFLOAT -f 434000

Where 192.168.0.x 8011 represents the IP address and port of the host running GRC.
Configure TCP Server Sink with your network adapter address and port.
