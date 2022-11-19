# install-qt-static
action to install static qt to windows

## usage
````yml
- name: install qt static
    uses: orestonce/install-qt-static@v0.4.0
    with:
      version: Qt5.15.7-Windows-x86_64-MinGW8.1.0-staticFull-20221104
      dir: qt_static_install
````
* version support value list
  * [x] Qt5.6.3-Windows-x86-MinGW4.9.4-staticFull-20200104
  * [x] Qt5.15.7-Windows-x86-MinGW8.1.0-staticFull-20221104
  * [x] Qt5.15.7-Windows-x86_64-MinGW8.1.0-staticFull-20221104
* runner.os support
  * [x] Windows
