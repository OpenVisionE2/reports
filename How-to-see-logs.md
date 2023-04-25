Hi everyone,

When you want to tell us about a problem, if that's in Ubuntu you need to attach the log file which bitbake shows you its location as zip file.

If you want to see enigma2 log first do this via telnet (it doesn't matter if your STB boots or not, just use a LAN cable with dhcp enabled):
```diff
@@ (We call this enigma2 with debug enabled in telent) @@
```
```
init 4&& sleep 5&& ENIGMA_DEBUG_LVL=4 enigma2
```
Sometimes you need to check dmesg log:
```
dmesg
```
or others in:
```
/var/log/messages
```
```diff
@@ Always use attach your logs and never paste the whole thing here as we need our eyes. @@
```

Also if GUI/Enigma2 works you can go to Menu->Standby & Restart->Restart GUI in debug mode

Then after reboot go to
```
/home/root/logs
```
and give us the latest enigma2_debug_x.log
