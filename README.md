# security-iauda
# openssl is very secure
	openssl genrsa -des3 -out server.key 4096 
	بعد از این دستور یک پسورد رو با تکرار برای کلید وارد میکنیم
openssl req -new -key server.key -out server.csr
openssl x509 -req -days 365 -in server.csr -signkey server.key -out server.crt
p=11; q=3; n=p*q
11*3=33
M=(p-1)(q-1)    10*2=20
e=az m kochektar ,nebat be m aval=3
(d*e)mod m=1   dar natije  d=7 
private key=e,n    public key=d,n
c=m^e mod n=encrypt
M=c^d mod n= decrypt
crs
# openssl req-new-newkey rs:1024-keyout hostkey.pem-nodes-outhostcsr.pem
-newkey rsa:1024-->create key1024 byte kamtarin meghdar512byte
-keyout hostkey.pem:kelide khosusi generate shode ra tuye file hostkey.pem zakhire mikone va zamane tolide govahi ssl ehtiyaj mishe
-nodes:baraye web server
-out hostcsr.pem: csr generate shodera dar file hostcsr.pem save mikone-mitavanim in ra be markaze tolid ssl bedim va baraye tolid govahi self-signed az an estefade konim
