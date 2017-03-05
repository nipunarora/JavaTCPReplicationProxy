Raw TCP Proxy
=====

> This is a protocol independent TCP proxy. It is compatible with **any** TCP software; such as web servers, Minecraft servers, secure shell, and much much more. It was developed to have no limitations - literally.

[![Build Status](https://travis-ci.org/brendanashworth/Raw-TCP-Proxy.png?branch=master)](https://travis-ci.org/brendanashworth/Raw-TCP-Proxy)

### Usage
Usage is very simple, as a Perl wrapper is provided.
```bash
$ git clone https://github.com/boboman13/Raw-TCP-Proxy.git && cd Raw-TCP-Proxy
```

The usage is as follows:
```bash
$ java -jar target/Raw-TCP-Proxy-1.0-SNAPSHOT.jar -l 0.0.0.0:220005 -o 127.0.0.1:22000 -r 138.15.170.34:22001
```

```
-l listening IP:Port
-o output production server IP:Port
-r replica server IP:Port
```

The first argument is the listening IP / port, and the second argument is the output IP / port.

If you want to access the Java .jar directly, you can access the flags at [the Main file](./src/main/java/net/boboman13/raw_tcp_proxy/main/Main.java).

### Compilation
This is without the Perl wrapper.
```bash
$ git clone https://github.com/boboman13/Raw-TCP-Proxy.git
$ mvn clean package
```
