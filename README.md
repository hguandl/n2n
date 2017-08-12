# n2n_v2 modifed for Openwrt

To compile the binary files used on Openwrt, toolchain is needed. After that, please edit n2n_v2/CMakeLists.txt. The first several lines need to be changed:
```
SET(CMAKE_SYSTEM_NAME Linux)
SET(CMAME_C_COMPILER mips-openwrt-linux-gcc)
SET(CMAKE_CXX_COMPILER mips-openwrt-linux-g++)
SET(CMAKE_FIND_ROOT_PATH ~/mips_34kc_gcc)
```
Modify them according to the develop environment you are using.

---

This is the current development branch of the n2n p2p vpn software.

http://www.ntop.org/products/n2n/

It contains some modifications of the v2 version of n2n, which is the latest stable version
and should be used for productive environments.
All the current development happens in this repository in the new_protocol branch, which is 
intended to be come version v3 of n2n and then merged back into the original svn repository
on ntop.org.

Uses sglib http://sglib.sourceforge.net.

For further information please visit the wiki https://github.com/meyerd/n2n/wiki.
