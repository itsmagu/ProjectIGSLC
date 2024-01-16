This document will embody initial method to implement a synthetic shell around the boot process of a system. This specific specification is made for my personal interest in the subject.
The end goal :
- A system that prompts the users on boot which partition they want to boot into. (See https://wiki.archlinux.org/title/REFInd)
- The system will probe for all bootable devices and display both its normal information plus additional optional information such as data or art
- The system should support normal system bootable partitions, but mainly the system will be made for "special" partitions that may or may not include a kernel. If it is missing a kernel the of this system will be used... What kernel and its configuration will also be in this specification.
- The "special" partitions will also be able to take part in a shared "user/home" partition from this system