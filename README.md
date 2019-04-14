# openssl

open ssl using tcp sockets 
client and server 

code starts with : 
http://simplestcodings.blogspot.com/2010/08/secure-server-client-using-openssl-in-c.html
http://www.cs.utah.edu/~swalton/listings/sockets/programs/part1/chap4/ttcp-client.c
http://www.cs.utah.edu/~swalton/listings/sockets/programs/part1/chap4/ttcp-server.c

create a certificate first with 
$openssl req -x509 -nodes -days 365 -newkey rsa:1024 -keyout mycert.pem -out mycert.pem

run with : 
Run with:
$sudo ./server 8080
$sudo ./client localhost 8080 

to compile : 
$gcc -o server server.c -L/usr/local/sssl/lib -lssl -lcrypto


