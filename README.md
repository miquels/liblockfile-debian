## debian packaging for liblockfile

To build a debian package, run `./buildpackage` instead of `dpkg-buildpackage`.
This will extract the upstream tarball into a temporary build directory, copy
the debian/ directory into it, chdir into it, and run dpkg-buildpackage there.

To clean, run `./buildpackage clean` or, alternatively `git clean -xf`.

