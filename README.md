LineageOS For Huawei P9 Lite Smart codename ("diego")
==========================================

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/lineage13

Next, naviate into that new directory via the terminal:

	cd ~/lineage13

To initialize your local repository using the Turbo ROM trees, use this command:

	repo init -u git://github.com/LineageOS/android.git -b cm-13.0

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

	$ echo "export USE_CCACHE=1" >> ~/.bashrc
	$ prebuilts/misc/linux-x86/ccache/ccache -M 30G

Third:

	. build/envsetup.sh
	brunch diego

-------------
 
_Developers contributors_
---------------

	@EfranDev

