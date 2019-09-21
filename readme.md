

Links of interest:
http://oldcomputer.info/others/brother70/index.htm

Mame wip emulator:
https://github.com/kfazz/mame_brother_wp


building on ubuntu 19.04:
sudo apt build-dep mame
QT_SELECT=5  make SOURCES=src/mame/drivers/wp75.cpp REGENIE=1 USE_SYSTEM_LIB_LUA=lua5.3:/usr/include/lua5.3
./mame64 wp75 -debug


loading an apl file:
(in mame debugger)
let the rom run for a while, so memory is intitialized
break
load tutor.apl,5000  (tutor.apl should be in root of mame src)
do PC=5008
go



