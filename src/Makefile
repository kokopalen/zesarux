EMULATOR_VERSION=6.1
CFLAGS= -Wall -Wextra -fsigned-char -I/mipsel-buildroot-linux-uclibc/sysroot/usr/include
LDFLAGS= -L/opt/buildroot-2018.02.9/output/host/mipsel-buildroot-linux-uclibc/sysroot/usr/lib -lSDL -lpthread
CC=mipsel-linux-gcc
INSTALLPREFIX=/usr/local


all: zesarux


zesarux: charset.o       scrsdl.o audiosdl.o common_sdl.o  autoselectoptions.o chardetect.o textspeech.o scrnull.o     audionull.o ay38912.o cpu.o codsinpr.o codprddfd.o codpred.o operaciones.o debug.o tape.o tape_tap.o tape_tzx.o tape_smp.o audio.o screen.o mem128.o chloe.o prism.o tbblue.o timex.o zx8081.o jupiterace.o z88.o cpc.o sam.o atomlite.o zxuno.o snap.o snap_zsf.o snap_z81.o snap_zx8081.o snap_rzx.o snap_spg.o spg_depack.o menu.o core_spectrum.o core_zx8081.o core_z88.o core_cpc.o core_ace.o core_sam.o core_ql.o core_mk14.o mk14.o scmp.o timer.o contend.o disassemble.o utils.o playtzx.o mdvtool.o joystick.o ula.o mmc.o ide.o pd765.o divmmc.o divide.o diviface.o zxpand.o superupgrade.o dandanator.o betadisk.o codetests.o kartusho.o spritefinder.o multiface.o spectra.o spritechip.o printers.o realjoystick.o ulaplus.o if1.o ds1307.o ql.o m68kcpu.o m68kdasm.o m68kops.o  m68kopac.o m68kopdm.o m68kopnz.o chrome.o tsconf.o remote.o esxdos_handler.o main_unix.o 
	$(CC) $(CFLAGS) cpu.o main_unix.o charset.o       scrsdl.o audiosdl.o common_sdl.o  autoselectoptions.o chardetect.o textspeech.o scrnull.o screen.o mem128.o chloe.o prism.o tbblue.o timex.o     audionull.o ay38912.o codsinpr.o codprddfd.o codpred.o operaciones.o debug.o tape.o tape_tap.o tape_tzx.o tape_smp.o audio.o zx8081.o jupiterace.o z88.o cpc.o sam.o atomlite.o zxuno.o snap.o snap_zsf.o snap_z81.o snap_spg.o spg_depack.o snap_zx8081.o snap_rzx.o menu.o core_spectrum.o core_zx8081.o core_z88.o core_cpc.o core_ace.o core_sam.o core_ql.o core_mk14.o mk14.o scmp.o timer.o contend.o disassemble.o utils.o playtzx.o mdvtool.o joystick.o ula.o mmc.o ide.o pd765.o divmmc.o divide.o diviface.o zxpand.o superupgrade.o dandanator.o betadisk.o codetests.o kartusho.o spritefinder.o multiface.o spectra.o spritechip.o printers.o realjoystick.o ulaplus.o ds1307.o if1.o ql.o m68kcpu.o m68kdasm.o m68kops.o  m68kopac.o m68kopdm.o m68kopnz.o chrome.o tsconf.o remote.o esxdos_handler.o -o zesarux $(LDFLAGS)
	@echo
	@echo "Compilation finished"
	@echo

charset.o: charset.c
	$(CC) $(CFLAGS) -c charset.c

scrnull.o: scrnull.c scrnull.h debug.h screen.h cpu.h
	$(CC) $(CFLAGS) -c scrnull.c

codprddfd.o: codprddfd.c cpu.h operaciones.h debug.h contend.h utils.h compileoptions.h
	$(CC) $(CFLAGS) -c codprddfd.c

codpred.o: codpred.c cpu.h operaciones.h debug.h contend.h zxuno.h tbblue.h
	$(CC) $(CFLAGS) -c codpred.c

codsinpr.o: codsinpr.c cpu.h operaciones.h debug.h contend.h utils.h compileoptions.h z88.h snap_rzx.h esxdos_handler.h
	$(CC) $(CFLAGS) -c codsinpr.c

operaciones.o: operaciones.c cpu.h operaciones.h debug.h audio.h tape.h ay38912.h mem128.h chloe.h prism.h tbblue.h timex.h zx8081.h menu.h screen.h compileoptions.h contend.h joystick.h ula.h utils.h printers.h disassemble.h z88.h ulaplus.h zxuno.h chardetect.h mmc.h ide.h divmmc.h divide.h diviface.h zxpand.h spectra.h spritechip.h jupiterace.h cpc.h sam.h if1.h timer.h pd765.h superupgrade.h snap_rzx.h multiface.h chrome.h tsconf.h ds1307.h mk14.h
	$(CC) $(CFLAGS) -c operaciones.c

cpu.o: cpu.c cpu.h scrnull.h scrstdout.h scrsimpletext.h operaciones.h debug.h compileoptions.h tape.h tape_tap.h tape_tzx.h audio.h screen.h ay38912.h chloe.h prism.h tbblue.h mem128.h timex.h scrcurses.h scraa.h scrxwindows.h scrsdl.h scrnull.h scrfbdev.h audiodsp.h audiosdl.h audionull.h audioalsa.h audiopulse.h zx8081.h snap.h menu.h core_spectrum.h core_zx8081.h core_z88.h tape_smp.h contend.h utils.h ula.h printers.h joystick.h realjoystick.h z88.h ulaplus.h autoselectoptions.h zxuno.h chardetect.h textspeech.h mmc.h ide.h divmmc.h divide.h diviface.h zxpand.h spectra.h spritechip.h jupiterace.h cpc.h sam.h if1.h atomlite.h dandanator.h kartusho.h spritefinder.h superupgrade.h ql.h remote.h snap_rzx.h multiface.h chrome.h tsconf.h scmp.h mk14.h esxdos_handler.h betadisk.h codetests.h pd765.h
	$(CC) $(CFLAGS) -c cpu.c

core_spectrum.o: core_spectrum.c core_spectrum.h cpu.h debug.h tape.h audio.h screen.h ay38912.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h ula.h utils.h realjoystick.h divmmc.h divide.h diviface.h timex.h zxuno.h prism.h snap_rzx.h superupgrade.h pd765.h tsconf.h
	$(CC) $(CFLAGS) -c core_spectrum.c

core_zx8081.o: core_zx8081.c core_zx8081.h cpu.h debug.h tape.h audio.h screen.h ay38912.h operaciones.h snap.h zx8081.h timer.h menu.h chardetect.h compileoptions.h contend.h snap_zx8081.h utils.h realjoystick.h ula.h
	$(CC) $(CFLAGS) -c core_zx8081.c

core_ace.o: core_ace.c core_ace.h cpu.h debug.h tape.h audio.h screen.h ay38912.h operaciones.h snap.h jupiterace.h timer.h menu.h chardetect.h compileoptions.h contend.h snap_zx8081.h utils.h realjoystick.h ula.h
	$(CC) $(CFLAGS) -c core_ace.c

core_ql.o: core_ql.c core_ql.h cpu.h debug.h tape.h audio.h screen.h ay38912.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h snap_zx8081.h utils.h realjoystick.h ula.h
	$(CC) $(CFLAGS) -c core_ql.c

core_mk14.o: core_mk14.c core_mk14.h scmp.h cpu.h debug.h tape.h audio.h screen.h ay38912.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h snap_zx8081.h utils.h realjoystick.h ula.h
	$(CC) $(CFLAGS) -c core_mk14.c

mk14.o: mk14.c mk14.h cpu.h debug.h scmp.h utils.h menu.h
	$(CC) $(CFLAGS) -c mk14.c

core_z88.o: core_z88.c core_z88.h cpu.h debug.h tape.h audio.h screen.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h ula.h utils.h z88.h audio.h utils.h
	$(CC) $(CFLAGS) -c core_z88.c

core_cpc.o: core_cpc.c core_cpc.h cpu.h debug.h tape.h audio.h screen.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h ula.h utils.h audio.h utils.h tape.h cpc.h realjoystick.h
	$(CC) $(CFLAGS) -c core_cpc.c


core_sam.o: core_sam.c core_sam.h cpu.h debug.h tape.h audio.h screen.h operaciones.h snap.h timer.h menu.h chardetect.h compileoptions.h contend.h ula.h utils.h audio.h utils.h tape.h cpc.h realjoystick.h
	$(CC) $(CFLAGS) -c core_sam.c

scmp.o: scmp.c scmp.h cpu.h operaciones.h
	$(CC) $(CFLAGS) -c scmp.c


timer.o: timer.c timer.h cpu.h audio.h debug.h menu.h tape.h screen.h compileoptions.h zx8081.h joystick.h utils.h printers.h z88.h autoselectoptions.h zxuno.h textspeech.h mmc.h ide.h zxpand.h superupgrade.h snap.h snap_rzx.h ql.h esxdos_handler.h betadisk.h pd765.h
	$(CC) $(CFLAGS) -c timer.c


debug.o: debug.c cpu.h debug.h mem128.h timex.h screen.h menu.h zx8081.h operaciones.h core_spectrum.h core_zx8081.h core_z88.h core_ace.h core_cpc.h disassemble.h utils.h prism.h core_sam.h core_ql.h spectra.h tbblue.h zxuno.h ulaplus.h timex.h ay38912.h ula.h ql.h m68k.h superupgrade.h core_mk14.h scmp.h dandanator.h kartusho.h spritefinder.h multiface.h chloe.h cpc.h sam.h snap.h diviface.h betadisk.h
	$(CC) $(CFLAGS) -c debug.c

tape.o: tape.c tape.h cpu.h operaciones.h debug.h tape_tap.h tape_tzx.h tape_smp.h chloe.h prism.h mem128.h timex.h snap.h compileoptions.h screen.h zx8081.h menu.h snap_z81.h utils.h audio.h screen.h autoselectoptions.h zxuno.h timer.h superupgrade.h multiface.h chrome.h tsconf.h snap_spg.h tbblue.h
	$(CC) $(CFLAGS) -c tape.c

tape_tap.o: tape_tap.c tape_tap.h tape.h cpu.h operaciones.h debug.h
	$(CC) $(CFLAGS) -c tape_tap.c

tape_smp.o: tape_smp.c tape_smp.h tape.h cpu.h operaciones.h debug.h zx8081.h snap.h menu.h snap_zx8081.h utils.h
	$(CC) $(CFLAGS) -c tape_smp.c

tape_tzx.o: tape_tzx.c tape_tzx.h tape.h cpu.h operaciones.h debug.h utils.h
	$(CC) $(CFLAGS) -c tape_tzx.c

audio.o: audio.c cpu.h audio.h debug.h screen.h utils.h zx8081.h audionull.h jupiterace.h autoselectoptions.h operaciones.h cpc.h
	$(CC) $(CFLAGS) -c audio.c

audionull.o: audionull.c audionull.h cpu.h debug.h audio.h
	$(CC) $(CFLAGS) -c audionull.c

ay38912.o: ay38912.c ay38912.h cpu.h audio.h joystick.h
	$(CC) $(CFLAGS) -c ay38912.c

screen.o: screen.c screen.h debug.h mem128.h chloe.h prism.h timex.h cpc.h prism.h operaciones.h zx8081.h charset.h menu.h audio.h contend.h ula.h tape_smp.h z88.h ulaplus.h zxuno.h spectra.h spritechip.h timer.h sam.h ql.h chrome.h tsconf.h mk14.h
	$(CC) $(CFLAGS) -c screen.c

mem128.o: mem128.c cpu.h mem128.h debug.h contend.h zxuno.h chloe.h prism.h timex.h sam.h ula.h tbblue.h superupgrade.h chrome.h tsconf.h
	$(CC) $(CFLAGS) -c mem128.c

timex.o: timex.c timex.h cpu.h debug.h contend.h tape.h mem128.h menu.h
	$(CC) $(CFLAGS) -c timex.c

chloe.o: chloe.c chloe.h cpu.h timex.h mem128.h debug.h contend.h zxuno.h timex.h prism.h 
	$(CC) $(CFLAGS) -c chloe.c

chrome.o: chrome.c chrome.h cpu.h mem128.h debug.h contend.h  
	$(CC) $(CFLAGS) -c chrome.c

tsconf.o: tsconf.c tsconf.h cpu.h mem128.h debug.h contend.h menu.h screen.h ula.h operaciones.h
	$(CC) $(CFLAGS) -c tsconf.c

prism.o: prism.c prism.h cpu.h timex.h mem128.h debug.h contend.h zxuno.h timex.h utils.h menu.h
	$(CC) $(CFLAGS) -c prism.c

remote.o: remote.c remote.h cpu.h debug.h utils.h compileoptions.h ql.h disassemble.h menu.h audio.h timer.h screen.h ay38912.h charset.h diviface.h ula.h superupgrade.h tbblue.h tsconf.h operaciones.h snap.h
	$(CC) $(CFLAGS) -c remote.c

esxdos_handler.o: esxdos_handler.c esxdos_handler.h cpu.h operaciones.h debug.h menu.h utils.h diviface.h screen.h
	$(CC) $(CFLAGS) -c esxdos_handler.c

tbblue.o: tbblue.c tbblue.h cpu.h mem128.h debug.h contend.h utils.h menu.h divmmc.h diviface.h screen.h timex.h
	$(CC) $(CFLAGS) -c tbblue.c

zx8081.o: zx8081.c zx8081.h cpu.h screen.h debug.h audio.h core_zx8081.h operaciones.h menu.h ula.h
	$(CC) $(CFLAGS) -c zx8081.c

jupiterace.o: jupiterace.c jupiterace.h cpu.h screen.h debug.h audio.h core_ace.h operaciones.h menu.h
	$(CC) $(CFLAGS) -c jupiterace.c

z88.o: z88.c z88.h cpu.h screen.h debug.h core_z88.h contend.h joystick.h menu.h operaciones.h utils.h timer.h
	$(CC) $(CFLAGS) -c z88.c

cpc.o: cpc.c cpc.h cpu.h screen.h debug.h core_cpc.h contend.h joystick.h menu.h operaciones.h utils.h ay38912.h
	$(CC) $(CFLAGS) -c cpc.c

sam.o: sam.c sam.h cpu.h screen.h debug.h core_sam.h contend.h joystick.h menu.h operaciones.h utils.h
	$(CC) $(CFLAGS) -c sam.c

atomlite.o: atomlite.c atomlite.h cpu.h screen.h debug.h menu.h operaciones.h utils.h ide.h
	$(CC) $(CFLAGS) -c atomlite.c

zxuno.o: zxuno.c zxuno.h cpu.h debug.h contend.h mem128.h utils.h ula.h screen.h menu.h divmmc.h diviface.h ay38912.h ulaplus.h
	$(CC) $(CFLAGS) -c zxuno.c

#ql.o: 68000.c 68000_debug.c op68kadd.c op68karith.c op68ksub.c op68klogop.c op68kmisc.c op68kmove.c op68kshift.c 68000_additional.c ql.c
#	$(CC) $(CFLAGS) -c 68000.c 68000_debug.c op68kadd.c op68karith.c op68ksub.c op68klogop.c op68kmisc.c op68kmove.c op68kshift.c 68000_additional.c ql.c

ql.o: ql.c ql.h debug.h m68k.h utils.h menu.h operaciones.h
	$(CC) $(CFLAGS) -c ql.c


m68kcpu.o: m68kcpu.c
	$(CC) $(CFLAGS) -c m68kcpu.c

m68kdasm.o: m68kdasm.c
	$(CC) $(CFLAGS) -c m68kdasm.c

m68kops.o: m68kops.c
	$(CC) $(CFLAGS) -c m68kops.c

m68kopac.o: m68kopac.c
	$(CC) $(CFLAGS) -c m68kopac.c

m68kopdm.o: m68kopdm.c
	$(CC) $(CFLAGS) -c m68kopdm.c

m68kopnz.o: m68kopnz.c
	$(CC) $(CFLAGS) -c m68kopnz.c



snap.o: snap.c snap.h cpu.h debug.h operaciones.h zx8081.h mem128.h ay38912.h compileoptions.h autoselectoptions.h ay38912.h tape_smp.h audio.h screen.h menu.h tape.h snap_z81.h snap_zx8081.h snap_rzx.h utils.h ula.h joystick.h realjoystick.h z88.h chardetect.h jupiterace.h cpc.h timex.h zxuno.h ulaplus.h chloe.h prism.h diviface.h snap_rzx.h chrome.h tsconf.h snap_spg.h
	$(CC) $(CFLAGS) -c snap.c

snap_zsf.o: snap_zsf.c snap_zsf.h cpu.h debug.h operaciones.h zx8081.h mem128.h ay38912.h compileoptions.h autoselectoptions.h ay38912.h tape_smp.h audio.h screen.h menu.h tape.h snap_z81.h snap_zx8081.h snap_rzx.h utils.h ula.h joystick.h realjoystick.h z88.h chardetect.h jupiterace.h cpc.h timex.h zxuno.h ulaplus.h chloe.h prism.h diviface.h snap_rzx.h chrome.h tsconf.h divmmc.h
	$(CC) $(CFLAGS) -c snap_zsf.c

snap_z81.o: snap_z81.c snap_z81.h cpu.h debug.h operaciones.h snap.h
	$(CC) $(CFLAGS) -c snap_z81.c

snap_spg.o: snap_spg.c snap_spg.h cpu.h debug.h operaciones.h snap.h mem128.h tsconf.h
	$(CC) $(CFLAGS) -c snap_spg.c

spg_depack.o: spg_depack.c
	$(CC) $(CFLAGS) -c spg_depack.c

snap_zx8081.o: snap_zx8081.c snap_zx8081.h cpu.h debug.h operaciones.h zx8081.h audio.h screen.h tape.h tape_smp.h snap_z81.h menu.h snap.h utils.h
	$(CC) $(CFLAGS) -c snap_zx8081.c

snap_rzx.o: snap_rzx.c snap_rzx.h snap.h cpu.h debug.h operaciones.h utils.h menu.h screen.h
	$(CC) $(CFLAGS) -c snap_rzx.c

menu.o: menu.c menu.h screen.h cpu.h debug.h zx8081.h ay38912.h compileoptions.h tape.h audio.h timer.h snap.h operaciones.h disassemble.h utils.h contend.h joystick.h ula.h printers.h realjoystick.h scrstdout.h z88.h ulaplus.h autoselectoptions.h zxuno.h charset.h chardetect.h textspeech.h  mmc.h ide.h divmmc.h divide.h diviface.h zxpand.h spectra.h spritechip.h jupiterace.h timex.h chloe.h cpc.h prism.h sam.h if1.h pd765.h atomlite.h tbblue.h dandanator.h kartusho.h spritefinder.h multiface.h superupgrade.h m68k.h remote.h snap_rzx.h multiface.h scmp.h esxdos_handler.h tsconf.h snap_spg.h betadisk.h tape_tzx.h snap_zsf.h
	$(CC) $(CFLAGS) -c menu.c

disassemble.o: disassemble.c disassemble.h cpu.h operaciones.h debug.h ql.h utils.h scmp.h menu.h
	$(CC) $(CFLAGS) -c disassemble.c

utils.o: utils.c utils.h cpu.h debug.h joystick.h compileoptions.h tape.h snap.h screen.h realjoystick.h menu.h z88.h playtzx.h tape_tzx.h operaciones.h zx8081.h autoselectoptions.h ulaplus.h ay38912.h textspeech.h spectra.h zxuno.h spritechip.h timex.h cpc.h sam.h divmmc.h divide.h superupgrade.h chardetect.h zx8081.h jupiterace.h mmc.h ide.h zxpand.h diviface.h divmmc.h divide.h dandanator.h kartusho.h spritefinder.h ql.h m68k.h remote.h ula.h snap_rzx.h scmp.h mk14.h esxdos_handler.h tbblue.h tsconf.h mdvtool.h betadisk.h pd765.h
	$(CC) $(CFLAGS) -c utils.c

playtzx.o: playtzx.c playtzx.h debug.h audio.h utils.h
	$(CC) $(CFLAGS) -c playtzx.c

mdvtool.o: mdvtool.c mdvtool.h debug.h utils.h ay38912.h
	$(CC) $(CFLAGS) -c mdvtool.c

contend.o: contend.c contend.h cpu.h debug.h screen.h compileoptions.h ulaplus.h zxuno.h ula.h tbblue.h
	$(CC) $(CFLAGS) -c contend.c

joystick.o: joystick.c joystick.h cpu.h debug.h screen.h
	$(CC) $(CFLAGS) -c joystick.c

ula.o: ula.c ula.h cpu.h debug.h screen.h contend.h menu.h multiface.h betadisk.h
	$(CC) $(CFLAGS) -c ula.c

mmc.o: mmc.c mmc.h cpu.h debug.h utils.h menu.h screen.h divmmc.h
	$(CC) $(CFLAGS) -c mmc.c

ide.o: ide.c ide.h cpu.h debug.h utils.h menu.h screen.h divide.h
	$(CC) $(CFLAGS) -c ide.c

pd765.o: pd765.c pd765.h cpu.h debug.h utils.h menu.h screen.h mem128.h operaciones.h
	$(CC) $(CFLAGS) -c pd765.c

zxpand.o: zxpand.c zxpand.h mmc.h cpu.h debug.h utils.h menu.h screen.h zx8081.h joystick.h
	$(CC) $(CFLAGS) -c zxpand.c

dandanator.o: dandanator.c dandanator.h cpu.h debug.h utils.h operaciones.h ula.h
	$(CC) $(CFLAGS) -c dandanator.c

betadisk.o: betadisk.c betadisk.h cpu.h debug.h utils.h operaciones.h ula.h mem128.h screen.h
	$(CC) $(CFLAGS) -c betadisk.c

codetests.o: codetests.c codetests.h cpu.h debug.h utils.h operaciones.h ula.h mem128.h screen.h
	$(CC) $(CFLAGS) -c codetests.c

kartusho.o: kartusho.c kartusho.h cpu.h debug.h utils.h operaciones.h ula.h
	$(CC) $(CFLAGS) -c kartusho.c

spritefinder.o: spritefinder.c spritefinder.h cpu.h debug.h utils.h operaciones.h ula.h screen.h
	$(CC) $(CFLAGS) -c spritefinder.c

multiface.o: multiface.c multiface.h cpu.h debug.h utils.h operaciones.h
	$(CC) $(CFLAGS) -c multiface.c

superupgrade.o: superupgrade.c superupgrade.h cpu.h debug.h utils.h operaciones.h mem128.h menu.h screen.h
	$(CC) $(CFLAGS) -c superupgrade.c

spectra.o: spectra.c spectra.h cpu.h debug.h utils.h menu.h screen.h operaciones.h mem128.h ulaplus.h
	$(CC) $(CFLAGS) -c spectra.c

spritechip.o: spritechip.c spritechip.h cpu.h debug.h utils.h screen.h ula.h ulaplus.h mem128.h
	$(CC) $(CFLAGS) -c spritechip.c

divmmc.o: divmmc.c divmmc.h divide.h diviface.h cpu.h debug.h utils.h
	$(CC) $(CFLAGS) -c divmmc.c

divide.o: divide.c divide.h divmmc.h diviface.h cpu.h debug.h utils.h
	$(CC) $(CFLAGS) -c divide.c

diviface.o: diviface.c diviface.h cpu.h debug.h utils.h menu.h screen.h operaciones.h zxuno.h contend.h prism.h tbblue.h tsconf.h
	$(CC) $(CFLAGS) -c diviface.c

if1.o: if1.c if1.h cpu.h debug.h utils.h operaciones.h menu.h
	$(CC) $(CFLAGS) -c if1.c

ds1307.o: ds1307.c ds1307.h cpu.h debug.h utils.h operaciones.h menu.h
	$(CC) $(CFLAGS) -c ds1307.c

printers.o: printers.c printers.h cpu.h debug.h utils.h screen.h menu.h
	$(CC) $(CFLAGS) -c printers.c

realjoystick.o: realjoystick.c realjoystick.h cpu.h debug.h joystick.h menu.h utils.h  screen.h compileoptions.h
	$(CC) $(CFLAGS) -c realjoystick.c

ulaplus.o: ulaplus.c ulaplus.h cpu.h debug.h screen.h spectra.h menu.h
	$(CC) $(CFLAGS) -c ulaplus.c

autoselectoptions.o: autoselectoptions.c autoselectoptions.h debug.h zx8081.h cpu.h screen.h joystick.h tape.h realjoystick.h ulaplus.h menu.h utils.h chardetect.h
	$(CC) $(CFLAGS) -c autoselectoptions.c

chardetect.o: chardetect.c chardetect.h cpu.h operaciones.h debug.h screen.h textspeech.h disassemble.h menu.h
	$(CC) $(CFLAGS) -c chardetect.c

textspeech.o: textspeech.c textspeech.h cpu.h operaciones.h debug.h screen.h chardetect.h menu.h utils.h sam.h
	$(CC) $(CFLAGS) -c textspeech.c


clean:
	rm -f *.o zesarux zesarux.exe smpatap sp_z80 tapabin leezx81 file_to_eprom bmp_to_prism_4_planar bmp_to_sprite install.sh 
	rm -fR bintargztemp/ sourcetargztemp/ ZEsarUX_win-$(EMULATOR_VERSION)/
	rm -fR macos/zesarux.app
	rm -fR macos/zesarux.dmg
	rm -fR macos/zesarux.dmg.gz
	rm -fR macos/ZEsarUX_macos*gz
	rm -f ZEsarUX_bin-*tar.gz
	rm -f ZEsarUX_src-*tar.gz
	rm -f ZEsarUX_win-*.zip
	rm -f ZEsarUX_extras-*.zip

COMMONFILES=ACKNOWLEDGEMENTS LICENSE LICENSE_MOTOROLA_CORE LICENSE_SCMP_CORE Changelog TODO README HISTORY FEATURES INSTALL INSTALLWINDOWS ALTERNATEROMS INCLUDEDTAPES DONATE FAQ zesarux.odt mantransfev3.bin *.rom zxuno.flash tbblue.mmc speech_filters my_soft zesarux.mp3 zesarux.xcf editionnamegame.tap bin_sprite_to_c.sh

ONLYSOURCEFILES=macos *.c *.m *.h *.tpl DEVELOPMENT CHECKLIST configure generate_install_sh.sh join_tzx.sh testsound.sh txt_to_basic_lines.sh automatic_tests.sh zxuno_roms_bin_a_flash.sh *.asm benchmark_*.txt current_checklist.txt patches prism_change_boot.txt pruebas_screen_rgb32 nuevo_core_zx8081 pruebas_z88_core_topspeed/


ONLYUNIXBINARIES=install.sh zesarux
ONLYWINBINARIES=zesarux.exe -L/opt/buildroot-2018.02.9/output/host/mipsel-buildroot-linux-uclibc/sysroot/usr/lib -lSDL -lpthread.dll 

sourcetargz:
	rm -fR sourcetargztemp
	mkdir -p sourcetargztemp/ZEsarUX-$(EMULATOR_VERSION)
	cp -a $(COMMONFILES) $(ONLYSOURCEFILES) sourcetargztemp/ZEsarUX-$(EMULATOR_VERSION)/
	tar -C sourcetargztemp -cvzf ZEsarUX_src-$(EMULATOR_VERSION).tar.gz ZEsarUX-$(EMULATOR_VERSION)
	echo
	echo "Generated file is : ZEsarUX_src-$(EMULATOR_VERSION).tar.gz"

bintargz: all
	./generate_install_sh.sh
	rm -fR bintargztemp
	mkdir -p bintargztemp/ZEsarUX-$(EMULATOR_VERSION)
	cp -a $(COMMONFILES) $(ONLYUNIXBINARIES) bintargztemp/ZEsarUX-$(EMULATOR_VERSION)/
	tar -C bintargztemp -cvzf ZEsarUX_bin-$(EMULATOR_VERSION).tar.gz ZEsarUX-$(EMULATOR_VERSION)
	echo
	echo "Generated file is : ZEsarUX_bin-$(EMULATOR_VERSION).tar.gz"

extra_files:
	zip -r ZEsarUX_extras-$(EMULATOR_VERSION).zip extras
	echo "Generated file is: ZEsarUX_extras-$(EMULATOR_VERSION).zip"

windows:
	mkdir -p ZEsarUX_win-$(EMULATOR_VERSION)
	cp -a $(COMMONFILES) $(ONLYWINBINARIES) ZEsarUX_win-$(EMULATOR_VERSION)/
	zip -r ZEsarUX_win-$(EMULATOR_VERSION).zip ZEsarUX_win-$(EMULATOR_VERSION)/
	echo
	echo "Generated file is: ZEsarUX_win-$(EMULATOR_VERSION).zip"

macapp: all
	mkdir -p macos/zesarux.app
	cp -r macos/apptemplate/* macos/zesarux.app/
	cp zesarux macos/zesarux.app/Contents/MacOS/zesarux
	cp -a $(COMMONFILES) macos/zesarux.app/Contents/Resources/
	rm -f macos/zesarux.dmg
	rm -f macos/zesarux.dmg.gz
	hdiutil create -megabytes 100 -fs HFS+ -volname ZEsarUX macos/zesarux.dmg
	hdiutil attach -mountpoint macos/tempmount macos/zesarux.dmg
	cp -R macos/zesarux.app macos/tempmount
	ln -s /Applications/ macos/tempmount/Applications
	sleep 5
	hdiutil detach macos/tempmount
	gzip macos/zesarux.dmg


#CC32=gcc $(CFLAGS) -m32
#CC64=gcc $(CFLAGS) -m64

#UTILS32=smpatap_x32 sp_z80_x32 tapabin_x32 leezx81_x32
#UTILS64=smpatap_x64 sp_z80_x64 tapabin_x64 leezx81_x64

#utilities32: $(UTILS32)

#utilities64: $(UTILS64)


#smpatap_x32: smpatap_unix.c
#	$(CC32) $(CFLAGS) smpatap_unix.c -o smpatap_x32

#smpatap_x64: smpatap_unix.c
#	$(CC64) $(CFLAGS) smpatap_unix.c -o smpatap_x64

#leezx81_x32: leezx81_unix.c
#	$(CC32) $(CFLAGS) leezx81_unix.c -o leezx81_x32

#leezx81_x64: leezx81_unix.c
#	$(CC64) $(CFLAGS) leezx81_unix.c -o leezx81_x64

#sp_z80_x32: sp_z80_unix.c
#	$(CC32) $(CFLAGS) sp_z80_unix.c -o sp_z80_x32

#sp_z80_x64: sp_z80_unix.c
#	$(CC64) $(CFLAGS) sp_z80_unix.c -o sp_z80_x64

#tapabin_x32: tapabin_unix.c
#	$(CC32) $(CFLAGS) tapabin_unix.c -o tapabin_x32

#tapabin_x64: tapabin_unix.c
#	$(CC64) $(CFLAGS) tapabin_unix.c -o tapabin_x64


#UTILITIES=smpatap sp_z80 tapabin leezx81


install: all
	./generate_install_sh.sh
	./install.sh

#utilities: $(UTILITIES)
utilities: smpatap sp_z80 tapabin leezx81 file_to_eprom bmp_to_prism_4_planar bmp_to_sprite


smpatap: smpatap_unix.c
	$(CC) $(CFLAGS) smpatap_unix.c -o smpatap

leezx81: leezx81_unix.c
	$(CC) $(CFLAGS) leezx81_unix.c -o leezx81

sp_z80: sp_z80_unix.c
	$(CC) $(CFLAGS) sp_z80_unix.c -o sp_z80

tapabin: tapabin_unix.c
	$(CC) $(CFLAGS) tapabin_unix.c -o tapabin

file_to_eprom: file_to_eprom.c
	$(CC) $(CFLAGS) file_to_eprom.c -o file_to_eprom

bmp_to_prism_4_planar: bmp_to_prism_4_planar.c
	$(CC) $(CFLAGS) bmp_to_prism_4_planar.c -o bmp_to_prism_4_planar

bmp_to_sprite: bmp_to_sprite.c
	$(CC) $(CFLAGS) bmp_to_sprite.c -o bmp_to_sprite

main_unix.o: main_unix.c cpu.h
	$(CC) $(CFLAGS) -c main_unix.c

