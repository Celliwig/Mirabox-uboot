Dumped uboot using:

	dd if=/dev/mtd0 of=uboot.mtd0.dd

Old binaries extracted using information from:

	http://wtarreau.blogspot.com/2013/02/mirabox-much-better-than-guruplug.html

DDR3 Training:

	tail -c +37 uboot.mtd0.dd |head -c 48584 > ddr3_training.bin

uboot:

	tail -c +49153 uboot.mtd0.dd |head -c 675420 > uboot.bin
