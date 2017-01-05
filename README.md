## debian packaging for liblockfile

To build a debian package:

- make sure the .orig tarball is present in the parent directory.
- git clean -xf
- tar --xform s:[^/]\*:.: -xf ../liblockfile\_1.XY.orig.tar.gz
- dpkg-buildpackage -rfakeroot

After building, the directory can be cleaned with

- git clean -xf

