# My-Pure-Data-Patches
A couple of patches created to understand various objects in Pure Data. 

## Documentation
- [Pure Data documentation](http://archive.flossmanuals.net/pure-data/)
- [Pure Data documentation - PDF](http://archive.flossmanuals.net/_booki/pure-data/pure-data.pdf)
- [List of Pure Data objects](http://blazicek.net/list_of_pure_data_objects.html)
- [Pure Data Reference Card](https://puredata.info/docs/tutorials/pd-refcard)

## Tutorials
- [Running Pure Data on a headless Raspberry Pi](https://guitarextended.wordpress.com/2012/08/28/running-pd-on-a-headless-raspberry-pi/)
- [Pure Data Filters](https://archive.flossmanuals.net/pure-data/audio-tutorials/filters.html)
- [Pure Data Tutorial](https://puredata.info/docs/StartHere/)
- [Pure Data error: "priority 6 scheduling failed; running at normal priority"](https://www.reddit.com/r/puredata/comments/88uwyo/installing_pd_for_linux_mint_18/)
 Solution:
	1. Update Kernel    
	2. Create audio group: sudo groupadd audio
	3. Add your user to audio group: sudo gpasswd -a <username> audio
	4. Create group limits file for audio group: sudo nano /etc/security/limits.d/audio.conf
	5. Add the following lines to audio.conf:
  
 		@audio   -  rtprio     95
		@audio   -  memlock    unlimited
		#@audio   -  nice       -19
 
	6. Reboot
- [Pure Data Guitar Pedal - Pure Data Example Project](https://www.youtube.com/watch?v=DJCoOr4uHD4)
- [Sound Simulator - Pure Data Tutorial #1 - Simple Button + Message + Object patch](https://www.youtube.com/watch?v=1o5Wasmd8yU)
- [Sound Simulator - Pure Data Tutorial #2 - Additive Synth, Overtone Generator](https://www.youtube.com/watch?v=JtT_bZeoKzk)
- [Sound Simulator - Pure Data Tutorial #3 - Subtractive Synth, Low-Pass, High-Pass, Band-pass Filters](https://www.youtube.com/watch?v=FVYkQFP1_D4)
- [Sound Simulator - Pure Data Tutorial #4 - Attack-Decay-Sustain-Release Envelope](https://www.youtube.com/watch?v=W7Pp-DhMA_E)
- [Pd for Airports](https://www.youtube.com/watch?v=7sTrn39TT7k)

