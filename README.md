# drop
Script to upload files to a variety of filehostings using curl and netcat

drop is a script that works uploading files to a variety of filehostings.

## dependencies

* curl
* netcat

## filehostings list

For now, there are few hosting options; more will be added later, or features will be added to the existing ones.

* [temp.sh](https://temp.sh/)
* [0x0.st](https://0x0.st/)
* [x0.at](https://x0.at/)
* [uguu.se](https://uguu.se/)
* [catbox.moe](https://catbox.moe/)
* [file.io](https://file.io/)
* [tmpfile.link](https://tmpfile.link)
* [termbin](https://termbin.com/)

## usage

```sh
$ drop --help
-> use:
-> $ drop <filehost> <file/text> <extra parameters>

-> filehost list:
-> temp.sh - limit: 4gib - expires: 3d
-> 0x0.st - limit: 512mib - expires: 30d-1y
-> x0.at - limit: 1024mib - expires: 3d-100d
-> uguu.se - limit: 128mib - expires: 3h
-> catbox.moe - limit: 200mib - expires: 2y (without activity)
-> file.io - limit: 4gib - expires: 14d
-> tmpfile.link - limit: 100mib - expires: 7d
-> termbin

# Upload to a service
$ drop catbox.moe config
-> https://files.catbox.moe/rgcylr
$ drop temp.sh config
  % Total    % Received % Xferd  Average Speed  Time    Time    Time   Current
                                 Dload  Upload  Total   Spent   Left   Speed
100 165.1k 100     28 100 165.1k     18 109.5k   00:01   00:01         154.6k
-> https://temp.sh/Wwovx/config
$

# See version
$ drop --version
-> drop 0.2-rc2
$
```

## todo

- [ ] add more hostings
- [ ] further develop the hosting for catbox.moe

## license

MIT License
