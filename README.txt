# gentoo-mate-desktop
mate-1.14.0 ebuild for rinaldus-overlay

Here's an ugly kluge that I wrote for the mate-1.14.0 rinaldus overlay, (based on the mate-1.12.0 ebuild)

layman -a rinaldus-overlay

download mate-1.14.0.ebuild and put it into: 

/var/lib/layman/rinaldus-overlay/mate-base/

cd /var/lib/layman/rinaldus-overlay/mate-base/

ebuild mate-1.14.0.ebuild digest
ebuild mate-1.14.0.ebuild clean
ebuild mate-1.14.0.ebuild manifest

emerge --ask mate mate-system-monitor

You can probably remove the SRC_URI and FILESDIR variables.. I just put them there for future reference.

Good luck with MATE!
