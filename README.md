LineageOS 21.0 for Samsung Galaxy A10s
------------------------------------

Create directories

	$ mkdir lineage-21  
	$ cd lineage-21

Init the base manifest

	$ repo init -u git://github.com/LineageOS/android.git -b lineage-21 --git-lfs
  
Add the local manifest

  Take the xml file and copy it to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync 

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_a10s-ap2a-userdebug
	$ mka bacon
