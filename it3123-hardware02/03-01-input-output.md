# MODULE 03 INPUT AND OUTPUT

I-O speed considerations:

* CPU much faster than I-O (nano vs milliseconds)
* Burst data requirements

I-O coordination issues:

* Unexpected input and input formats

I-O control module:

* Gets messages from device(s)
* Accepts commands from CPU
* Buffers data in memory until transferred to I-O device
* Notifies CPU interrupts

Programmed I-O:

* Much slower than waiting on memory (busy waiting checks)

RAID - redundant array of inexpensive disks (level 01 - mirrored disk volumes)