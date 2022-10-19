#  universal5433_Patches
 * Bunch of important patches
 
# Patching
- Apply using `git patch am *.patch` or repopick if on lineage gerrit

## system/core
* Handle empty thread names : [patch](https://review.lineageos.org/c/LineageOS/android_system_core/+/256219)
* needed to fix `Abort message: 'thread name not provided to Thread::run'`

## Repopick
repopick 256219 -P system/core -f #Handle Empty Thread Name
