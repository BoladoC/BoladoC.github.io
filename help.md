---
layout: default
---

** Help : HackTheBox **

	Help es un CTF challenge en HackTheBox
		
	Task: Obtener la bandera de user.txt ( Penetración en el sistema ) & bandera de root.txt que se obtiene mediante el pivoting estando dentro del sistema.
	
	#Enumeración:
	
	nmap -sCV -oN nmap/initial 10.10.10.121 --> Vemos los puertos abiertos 
	
	```bash
	┌──(root㉿kali)-[/home/…/Desktop/HackTheBox/Easy/Help]
	└─# nmap -sCV -oN nmap/initial 10.10.10.121
	Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-05 15:29 EDT
	Nmap scan report for help.htb (10.10.10.121)
	Host is up (1.2s latency).
	Not shown: 997 closed tcp ports (reset)
	PORT     STATE SERVICE VERSION
	22/tcp   open  ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.6 (Ubuntu Linux; protocol 2.0)
	| ssh-hostkey: 
	|   2048 e5:bb:4d:9c:de:af:6b:bf:ba:8c:22:7a:d8:d7:43:28 (RSA)
	|   256 d5:b0:10:50:74:86:a3:9f:c5:53:6f:3b:4a:24:61:19 (ECDSA)
	|_  256 e2:1b:88:d3:76:21:d4:1e:38:15:4a:81:11:b7:99:07 (ED25519)
	80/tcp   open  http    Apache httpd 2.4.18
	|_http-title: Apache2 Ubuntu Default Page: It works
	|_http-server-header: Apache/2.4.18 (Ubuntu)
	3000/tcp open  http    Node.js Express framework
	|_http-title: Site doesn't have a title (application/json; charset=utf-8).
	Service Info: Host: 127.0.1.1; OS: Linux; CPE: cpe:/o:linux:linux_kernel

	Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
	Nmap done: 1 IP address (1 host up) scanned in 21.91 seconds

	```
