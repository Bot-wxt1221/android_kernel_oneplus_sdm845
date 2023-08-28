# Hola amiguitos

It maybe can be used for roms which don't use Retrofit Dynamic Partitions.

This is my attempt to fix up and add a little CrDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

Rebased on bananafunction's lineage-20-test branch as of July 2023, which is based on the official android_kernel_oneplus_sdm845 lineage-20 branch from LineageOS, plus additional backported updates & fixes, with some extra goodies and optimization curated by mcdachpappe from MCD kernel, and a couple other useful things I've picked up along the way, and clang 16 support. Includes vibration control, digital audio gain controls, OOS panel color modes, battery idle mode support in op_disable_charge switch, zstd support for zram, updated sdfat and exfat drivers, updated CLO wifi drivers, and so on. Fancy!

If anyone is actually reading this, hi. You're pretty cool. There has been a lot of work on this, and most of it will never be visible, but at least you know I spent many hours of blood, sweat, and hair-pulling trying to test & fix things; and then most of that work was repeatedly rendered moot, but some of it at least has been getting picked up & cleaned up by smarter people than me and hopefully everyone will get to benefit from it.

Not TOO shabby for someone who doesn't actually know any c/c++/java. :D

Currently includes some temp hax to fix compiling under clang 16/17. If you're using clang-14 or older, you might be better off dropping the last two clang-related commits.

Clang-15 is also OK.
