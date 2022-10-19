#  universal5433_Patches
 * Bunch of important patches
 
# Patching
- Apply using `git patch am *.patch` or repopick if on lineage gerrit

## system/core
* Handle empty thread names : [Source](https://review.lineageos.org/c/LineageOS/android_system_core/+/256219)
* Needed to fix `Abort message: 'thread name not provided to Thread::run'`

## packages/modules/NetworkStack
* Opt-out for TCP info parsing on legacy Kernels [Source](https://github.com/ArrowOS/android_packages_modules_NetworkStack/commit/19bbd6fb49222c3849e8f9f8f5f2c56c61bdfc81)
* Needed to fix `TcpSocketTracker AAAAAAAAA*` Spam and `TcpSocketTracker: java.lang.IllegalArgumentException: Bad position 65648/3648`

## Repopick
`repopick 256219 -P system/core -f` # Handle Empty Thread Name
