This is the source for the Tribblix package

TRIBsys-install-media-internal

which is responsible for the variations in booting on live media
(net, cd, usb) during install. It follows the same general model
established by the OpenSolaris live CD, which is also used by other
illumos distributions.

The two commands required in sbin can be created by:

$CC -o sbin/listcd -ldevinfo listcd.c
$CC -o sbin/listusb -ldevinfo listusb.c

The original source was:

http://hipster.openindiana.org/components/illumos/slim_source/slim_source/usr/src/cmd/slim-install/

The listcd and listusb utilities are the same, as they do the same thing,
but the SMF services have been substantially modified.
