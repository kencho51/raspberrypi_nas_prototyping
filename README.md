# raspberry pi nas prototyping
Using a Raspberry Pi 3B+ to prototype NAS setup 

### raspberry pi spec
1. cpu info `cat /proc/cpuinfo`
```
processor	: 0
BogoMIPS	: 38.40
Features	: fp asimd evtstrm crc32 cpuid
CPU implementer	: 0x41
CPU architecture: 8
CPU variant	: 0x0
CPU part	: 0xd03
CPU revision	: 4

processor	: 1
BogoMIPS	: 38.40
Features	: fp asimd evtstrm crc32 cpuid
CPU implementer	: 0x41
CPU architecture: 8
CPU variant	: 0x0
CPU part	: 0xd03
CPU revision	: 4

processor	: 2
BogoMIPS	: 38.40
Features	: fp asimd evtstrm crc32 cpuid
CPU implementer	: 0x41
CPU architecture: 8
CPU variant	: 0x0
CPU part	: 0xd03
CPU revision	: 4

processor	: 3
BogoMIPS	: 38.40
Features	: fp asimd evtstrm crc32 cpuid
CPU implementer	: 0x41
CPU architecture: 8
CPU variant	: 0x0
CPU part	: 0xd03
CPU revision	: 4

Hardware	: BCM2835
Revision	: a020d3
Serial		: 00000000e2cb201f
Model		: Raspberry Pi 3 Model B Plus Rev 1.3
```
2. Model information `cat /proc/device-tree/model`
```
Raspberry Pi 3 Model B Plus Rev 1.3
```
### progress
- [] 0.Connect with BGI network
- [] 1.Install docker and pull rclone image
- [] 2.Pull files from the CNGB server and push files the other way too using rclone
- [] 3.From an AWS EC2 instance in Hong Kong region, (maybe we can use the instance I deploy to [fuw.rija.dev](http://fuw.rija.dev/) for file upload wizard for added realism and ease), copy files to the Pi
- [] 4.From the Pi, copy files to the EC2 instance using rclone
- [] 5.Try remote management of the Pi from internet
- [] 6.Try various hardening configuration and test security of the setup