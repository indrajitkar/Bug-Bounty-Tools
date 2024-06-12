# Bug-Bounty-Tools
# First we need to give permission to the files

 sudo chmod 755 *
 ./subdomain-recon.sh example.com
# results
├── alive.json
├── alive.txt
├── domains.json
├── domains.txt
└── enum.sh0 directories, 5 files

 ./response.sh alive.txt

./jsfiles.sh

./endpoints.sh

./nmap.sh domains.txt

cat alive.txt | aquatone -out ~/example.com/screenshots/

root@ubuntu:~/example.com$ ./search.sh -h
[+]USAGE: ./search.sh  (OPTIONS)
-j (string) - search in javascript files
-x (string) - search in header files
-e (string) - search in  html files
-n (string) - search nmap scans
-h - help


$ ./search.sh -j "admin"
$ ./search.sh -x "nginx"
$ ./search.sh -e "s3.amazonaws"
$ ./search.sh -n "ssh" #searching nmap scans for the string ssh
