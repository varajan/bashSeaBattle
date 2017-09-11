# bashSeaBattle
Play a sea battle game in *nix console;

You can play against an AI player (4 levels) or human but on the same PC.
Don't forget to make the 'run' file executable:
# chmod 755 run
# ./run

How to play it on Windows? I've found the way how to run it on Windows 10 64bit:
https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/

To convert all files from 'Dos' to '*nix'
for file in `ls -p | grep -v /`; do awk '{ sub("\r$", ""); print }' $file > temp$file; mv temp$file $file; done