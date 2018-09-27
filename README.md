# jersey-jetty

Small REST server for downloading CSV file
Small example that should explain how to setup jersey to run on embedded jetty web server.

Goto http://localhost:8080/api/csv and a file called some.csv will be downloaded.

open the some.csv file in emacs/vi shows this text:
Ärkel

$ hexdump ~/Downloads/some.csv 
0000000 ff fe c4 00 72 00 6b 00 65 00 6c 00            
000000c

fffe is the UTF-16 BOM
c400 Ä
7200 r
6b00 k
6500 e
6c00 l