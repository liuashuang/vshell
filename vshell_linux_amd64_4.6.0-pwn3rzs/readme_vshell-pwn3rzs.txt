vshell c2 4.6.0 linux64 // pwn3rzs 20240908
c2 command and control for remote access

Linux unpacked and provided by rootkies! I just applied same technique as for win64.

Notice: This is a closed-source c2 software, an exe file that's over 400 megabytes in
size, where the author has sent a goodbye message and claims it is to be the last version.
The exe itself was provided by a third party, which is likely to be legit, but origins
of this are murky and you should treat it as malware and only run it in a VM (as we say
for all our releases, but this sort of thing here especially!).  Our crack is clean but
we're talking about the source material which is beyond our control.

INSTRUCTIONS

1. Make any edits to conf/vshell.conf to set options and settings. (you can do this later
   and restart)

2. Run the vshell console application (already cracked / bypass license and password);
   it should start a web service at http://localhost:8082

3. Access http://localhost:8082 with credentials admin/pwn3rzs. It might ask you multiple
   times - this is because one layer is http auth, the other is the application. You
   can configure this in the conf file mentioned at step 1.
     user: admin
     pass: pwn3rzs

4. If you don't read Chinese, you can use the TWP browser extension (twp = translate web
   pages) to get real-time translation of the interface.
   Someone pointed out there is selection of English but I had the impression it didn't
   work as well as translation - I might be wrong so give it a try!

enjoy
