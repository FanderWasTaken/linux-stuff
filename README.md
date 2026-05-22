Hi! I really started disliking Windows lately and went over to the Tux side. I was having some issues moving over, but overall my system is now much more stable and more functional on Linux. I wanted to write down some stuff I found to be helpful on my journey, so it might help someone else as well :)

# Choosing a Distro
What distro you're on matters little, as far as it's capable of doing what you wanna be doing - stick with it. Personally I distro-hopped a lot, but I always keep coming back to Linux Mint - that's my recommendation for newbies and everyone who just wants a working computer. Be sure to research which distro does what and why it should be used, compare to your own preferences and make a decision.

A generic breakdown would be as follows: Arch - bleeding edge updates, latest features, breaks often. Debian - rock solid and quite old on Stable, a mess on Testing and Sid, requires manual setup for almost everything. Fedora - somewhere in between Debian and Arch update wise, but with a heavy focus on FOSS, thus no proprietary software in official repos. Ubuntu - stable, reasonably up to date, somewhat intrusive on user activities (forks remove bloat and keep the good stuff).

# Nvidia
It can be quite awful, but in general, if set up correctly, the issues are quite minimal. Generally I found that using X11 over Wayland causes less problems. Some programs don't use Nvidia GPU correctly still...
In order to fix Steam being laggy on Nvidia, add '-system-composer' launch option to your Steam shortcut. This way it works correctly. I'd add more fixes if I run into any issues later on.

# Gaming
I found that using Flatpak specifically for gaming on Linux offers huge benifits. Games turn from somewhat working to fully functional, when going from Native to Flatpak. So my personal suggestion is to install Steam (also applies to Lutris, Heroic, and other launchers) via Flatpak, in order to avoid various conflicts. Only install 'steam-libs' and similar packages as native ones, for drivers and proper client functionality.

# Audio
I personally found that PulseAudio simply works better by default over PipeWire. So switch to PulseAudio for audio, look up a guide on how to do that on your distro online.
Disable power-saving for audio devices to remove buzzing noise, here's [the guide](https://www.makeuseof.com/fix-static-noise-from-speakers-linux/)
