# Qt SQL driver plugin for SQLCipher ( for Qt 5 )

Builds on Qt >= **5.8.0**.
See https://github.com/sijk/qt5-sqlcipher to build up to Qt 5.5.x

The qsqlcipher.pro and smain.cpp are based on files from qsqlite
 qtbase/src/plugins/sqldrivers/sqlite.
The qsql_sqlite.cpp and qsql_sqlite_p.h were copied without
modifications from the same source.

## Dependencies

The SQLCipher headers and libraries should be installed before
compiling this plugin. Also, if pkg-config is not available you should
edit the qsqlcipher.pro and set the INCLUDEPATH and LIBS variables.


## Build instructions

```bash
git clone https://github.com/sjemens/qsqlcipher-qt5.git
cd qsqlcipher-qt5
mkdir -p build && cd build
qmake ../qsqlcipher-qt5.pro
make
make install  # most propably with sudo
```

Tested on Archlinux (x64) and MSYS2 (x64 only) with every Qt version after 5.8.0.


## Licences

For this plugin see LICENCE (**LGPLV3**)

[SQLCipher](https://www.zetetic.net/sqlcipher/license/) (**BSD**)

[Qt5 libraries](https://www.qt.io/licensing/) (**LGPLV3  GPLV2/GPLV3**)
