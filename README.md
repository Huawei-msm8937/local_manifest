TWRP For Huawei P9 Lite Smart codename ("diego")
==========================================

Use bootable-recovery from OmniRom

Also add the local manifests:

	git clone https://github.com/Huawei-msm8937/local_manifest -b cm-13.0 .repo/local_manifests

Then sync up with this command:

	repo sync --force-sync
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

First:

	cd ~/lineage13

Second:

	make clean && make clobber
	. build/envsetup.sh
	lunch lineage_diego-userdebug
	make recoveryimage

-------------
 
_Developers contributors_
---------------

	@EfranDev

