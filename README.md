# publius
## Share files to the web3 swarm.

### Short Description

publius uses webtorrent to share a folder to be viewed by federalist.

### Long Description

publius is a helper/server for federalist, which is a proof of concept to show that it's possible, today, to create an uncensorable and generally unblockable, distributed high performance 
viewable page.  federalist achieves this by using several amazing technologies and weaves them together:  

- [WebTorrent](https://github.com/webtorrent) - Provides torrenting capabilities and the bulk of the system.  federalist pages are torrents that are
distributed via magnet links and DHT is used to find peers.                            

- [Handshake](https://github.com/handshake-org/) - Provides decentralized DNS

- [nodeJS](https://github.com/nodejs) - Provides the Javascript engine built on V8 by Chrome

- [Electron](https://github.com/electron) - Provides the GUI


### Screenshot

![Federalist Screenshot](https://github.com/publiusfederalist/federalist/blob/master/federalist.png?raw=true)

## Use Cases

- Create an unblockable blog

- Whistleblow

- Share information

- Share meta information about other torrents

- Create an unblockable personal link site

## publius

The publius app share/seeds your page and gets the infohash to which an on-chain Handshake
name can be resolved.  Use the [federalist](https://github.com/publiusfederalist/federalist) app to browse pages in the federalist world.


## Installation

Required
```
npm
nodejs
```

1. Clone this repo
```
git clone https://github.com/publiusfederalist/publius
cd publius
```

2. Install npm modules
```
npm install webtorrent supercop.js
```

3. Create files in the web3root folder
```
cd web3root
vi index.html
```

4. Run seed
```
cd ..
./seed &
```

5. For mutable (updatable) sites, also run publius
```
./publius
```
6. Update Handshake Address on chain with TXT Record to your magnet link (depending on mutable or immutable from seed or publius -- see 'federalistpapers' as an example).

## Copyright and License

(c) 2021 Publius

MIT LICENSED
