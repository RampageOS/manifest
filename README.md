
💀 RampageOS Rifle 💀
===========
RampageOS is a AospExtended decendent aiming to 
give old devices android devices which cannot 
handle modern android a new life. With Upto date
Security. 

🏂 How to Build?
-------------

To initialize your local repository using the AospExtended trees, use a 
command like this:

```bash
  repo init -u https://github.com/RampageOS/manifest.git -b rifle
```
To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
  repo init --depth=1 -u https://github.com/RampageOS/manifest.git -b rifle
```
  
💾 Then to sync up:
----------------

```bash
  repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
🔨 Finally to build:
-----------------

```bash
  source build/envsetup.sh
  lunch aosp_device_codename-userdebug
  m bacon -j$(nproc --all) | tee log.txt
```

Follow Me On github 😊

* [**PrabhatProxy**](https://github.com/PrabhatProxy)
