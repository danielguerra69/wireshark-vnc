#### Wireshark vnc/html5 service for docker


### Usage

Start wireshark vnc/html5 server

```bash
docker run --name wireshark --privileged -v /Users/pcap:/home/wireshark/pcap -d -p 5900:5900 -p 6080:6080 danielguerra/wireshark-vnc
```
& check
```bash
docker logs wireshark
```
After this use a vnc client to connect (dockerhost:5900)
Or use wireshark in your browser http://<dockerhost>:6080/

Everything should start automaticly.

Right click opens a menu to start wireshark or xterm.

Everything runs under user wireshark, the user
has sudo rights.

Password for user wireshark = wireshark

```bash
sudo su -
```
