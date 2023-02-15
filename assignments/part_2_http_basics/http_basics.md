# Part 2 - HTTP basics
## 2.1 🧱 Client  - talking to some internetservices
Let's call some web services on the internet and talk to them.
From part 1 we learned some useful tricks to talk HTTPS using ncat.
```ncat --ssl HOSTNAME PORT```

HTTP messages in all its simplicity
```
VERB PATH VERSION
Host: HOSTNAME
```
As for example 
```
GET / HTTP/1.1
Host: bjartnes.dev
```


## 2.2 🧱 Server
Let's be a server and talk to curl or postman or something.

## 2.3 🧱 Host headers
Let's connect with curl to the same IP with different hostnames.

## 2.4 🎓 TCP Dump

Using tcpdump to monitor what was going on in the previous challenges. (Or Wireshark, if you have it) 
```
sudo tcpdump -i lo port 8080 -v
```
or 
```
tcpdump -i lo port 8080 -v
```

<details>
    <summary>An example</summary>

https://user-images.githubusercontent.com/1174441/219039131-e325d2b2-d3c2-47c3-bffe-f1d2d468b181.mp4
</details>

