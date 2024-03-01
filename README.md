# lisa-priam-datatower-card
 
## Thoughts

If we're going to compile the LOS source code, we're going to need a Priam DataTower. [Said Al Kossow in regard to compiling LOS](https://forum.vcfed.org/index.php?threads/wtb-working-apple-lisa.1246678/page-2):

>you really need something like a Priam Datatower (ie more disk space) to build LOS
>
>the tools are all there in the Version 3 Pascal Workshop.

It seems the compilation process is just too demanding of storage capacity; the 80MB of space the DataTower offered in 1982/3 would have certainly been more than enough (and had a price tag that reflected such a wealth of space).

The driver for the Priam DataTower is baked into LOS and, from the sound of it, no additional software is needed to mount DataTower volumes. Additionally, in the 09/1984 issue of Signal 16, the writers had the following to say regarding the DataTower:

>Signal 16, September 1984
>Priam's DataTower Arrives
>
>Not long after our Signal #13 story about Priam Whamos was published, we got a call from Bill North at Priam, who asked if we would like to find out more about their 86MB disk for the Lisa. The unit is called a DataTower, features a built-in 1/4" tape drive for backup, and is being retailed to the Lisa market as the MassFile by Tecmar. Negotiations began, and phone calls and letters started to wander back and forth between Priam and Semaphore.
>
>Last week, three boxes totaling 110 pounds arrived from San Jose. It was the DataTower. We hate to open a delivery until we're ready to write about it (or at least take good notes), otherwise we might forget some of those interesting first impressions. And, while this copy of Signal was still going through rework at the time (and could easily handle a few last minute changes), we couldn't possibly finish a comprehensive review of the DataTower and include it in the issue. So there was obviously no reason to open the shipment just yet. On the other hand, not opening a newly arrived product is like putting off opening Christmas packages even though it's December 25th. It didn't take long before we reached a compromise: we'd open the shipment, spend just half a day or so checking it out, report on just that much, and then do the rest of the investigation (or at least enough to look like we're making progress) when the next issue rolls around.
>
>We opened the first of the two small boxes and found a blank 1/4" tape cartridge, a power cord, a head cleaning kit, and a photocopy of a 180-page preliminary product specification (slightly too thick for its single staple). The second small box held another blank cartridge, an interface card designed to plug into a Lisa, and a cable to connect the card to the DataTower. The third box held the DataTower itself, contained in a 7" wide, 26" tall and 20" deep metal cabinet that's just right for standing alongside a desk. Unpacking dropped the unit's weight down to about 80 pounds.
>
>It only took us about ten minutes to install everything. The product specification that was included is really engineering documentation designed for programmer types who need to worry about interfacing and writing drivers and all of those esoteric subjects. It doesn't really try to be end user documentation describing how to simply make the unit operate with a Lisa. So we just got out our old Apple documentation on installing a Lisa two-port card, followed all the pictures and went through all the installation steps (but with the Priam card), attached the cable, and powered everything on.
>
>The Lisa we used was an original model that was upgraded to a 2/5, but which still has old ROMs so that the Startup Menu shows two twiggy slots. With the Priam's interface card installed, we were expecting to now find another printed circuit board icon in the Startup Menu. Instead, the menu included an actual little DataTower icon! Those ROMs aren't so old, after all...
>
>We quickly installed a 3.0 Office System on the new disk, and we were off and running. Now Attributes shows 142,420 blocks for our disk device.
>
>One way to think of the DataTower is as something like another Profile, except that it's a lot bigger and faster. Unfortunately, it's noisier too, just enough noisier to be a bit too loud for a nice, calm office environment. Naturally, it's also more expensive. At $8,995 suggested retail, the cost per megabyte is a lot less than on a Profile (and you get the built-in tape drive, too).
>
>Backing up the DataTower is a lot simpler than backing up a Profile, at least in the sense of not requiring a couple of boxes of floppies and lots of operator attention. By duplicating the disk icon, you can start copying the disk to the cartridge tape. So far, we've tried this once and soon realized that 3.0 copies the entire disk image to tape, regardless of how many files are actually stored on the disk, so we canceled the operation once it asked us to insert tape cartridge number two. We'll try a complete save again when we have a bit more time, and let you know how it goes.
>
>We've also started work on an interesting little project that will try to fully exercise the DataTower in a special way. Stay tuned for more details.

This would seem to indicate that the Lisa is capable of booting from a DataTower and that such a boot option will show up at the main boot menu.

The SMART-T protocol documentation is located in the src\priam-src-data directory; this will need to be cross-referenced with the Lisa source code in order to determine next steps for an emulator.