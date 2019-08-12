<h1 align="center">
  <br>
  <a href="https://www.facebook.com/PerthIronKingArena/"><img src="https://i.imgur.com/fZBgAit.png" alt="pika-overlay" width="200"></a>
  <br>
    Perth Iron King Arena overlay
  <br>
</h1>

<p align=center>
  <b> A NodeCG overlay designed for the <a href="https://www.facebook.com/PerthIronKingArena/">Perth Iron King Arena</a> tournament streams. </b>
</p>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#download">Download</a> •
  <a href="#Acknowledgments">Acknowledgments</a> •
  <a href="#license">License</a>
</p>

![](https://i.imgur.com/B8IMVQh.gif)

## Key features
* Scoreboard overlays for Tekken 7 and Street Fighter V
* Commentator overlays
* Intuitive user interface
* Easily customisable
* Persistent players and commentators via SQLite database

## How to use
* [Download](#download) or [build](#building) pika-overlay
* Start the pika-overlay server
    * Windows users: run `Start server.bat`
    * Everyone else: run `node index.js`
* Navigate to [http://localhost:9090](http://localhost:9090), preferably with Chromium
* This is the dashboard, you use this screen to modify the overlay state
* Click the graphics button at the top right corner
* Copy the URL of the overlay you would like to use
* Create a new browser source in OBS
* Paste the overlay URL
* Set the width to 1920 and the height to 1080
* Ensure "shutdown source when not visible" and "refresh browser when scene
    becomes active" are disabled

## Download
Portable binaries for Windows are available in the
[repository tags.](https://github.com/opeik/pika-overlay/tags)

## Building
### Prerequisites
* nodejs >= 8.3
* npm >= 2

Begin by installing nodecg:
```
npm install -g bower
git clone https://github.com/nodecg/nodecg.git
cd nodecg
npm install --production
bower install
```

Install pika-overlay:
```
cd bundles
git clone --recurse-submodules https://github.com/opeik/pika-overlay.git
npm install --production sqlite3
```

Run the server:
```
node ../../index.js
```

## Built with
* [nodecg](https://github.com/nodecg/nodecg)
* [country-list](https://github.com/fannarsh/country-list)
* [flag-icon-css](https://github.com/lipis/flag-icon-css)
* [jquery](https://jquery.com/)
* [jquery-ui](https://jqueryui.com)
* [Montserrat](https://fonts.google.com/specimen/Montserrat)

## Versioning
We use [Semantic Versioning](http://semver.org/) for versioning.

## License
This project is licensed under the ISC license. Please see the [`LICENSE.md`](LICENSE.md)
file for details.

## Acknowledgments
* The [PIKA](https://www.facebook.com/PerthIronKingArena/) tournament organisers for hosting amazing events
* [Escape Portal](https://www.escapeportal.com.au) for providing an amazing venue
