# install-qt-static
action to install static qt to windows

* version support value list
  * [x] Qt5.6.3-Windows-x86-MinGW4.9.4-staticFull-20200104
  * [x] Qt5.15.7-Windows-x86-MinGW8.1.0-staticFull-20221104
  * [x] Qt5.15.7-Windows-x86_64-MinGW8.1.0-staticFull-20221104
  * [x] Qt6.5.3-Windows-x86_64-MinGW13.2.0-ucrt-staticFull-20240527
* runner.os support
  * [x] Windows

* 静态编译Qt/MinGW来源于: https://build-qt.fsu0413.me/ , 仓库地址 https://github.com/Fsu0413/QtCompile

* 使用方法:

      - name: install qt static
        uses: orestonce/install-qt-static@v0.4.3
        with:
          version: Qt5.15.7-Windows-x86_64-MinGW8.1.0-staticFull-20221104

      - name: build  
        run: |
          cd image2pdf-qt && qmake && mingw32-make release && cd ..
          dir image2pdf-qt\release\image2pdf-qt.exe