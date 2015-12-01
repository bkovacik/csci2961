#Installation

Running ubuntu 15.10

I installed MongoDB and npm from the ubuntu repositories (sudo apt-get ...). I had git preinstalled, but I probably got it from the repositories as well.

NodeJS is not current at all. It is 0.10.25, so I installed the most recent stable version (4.2.2) from [the official website](https://nodejs.org/en/).
The PPA link's latest version is Utopic (14.10). For my system, Wily (15.10), ubuntu refuses to take this older version, so I needed to download it from the website.

I forked and checked out the develop branch without issue.

Originally, the npm install commands outputted fatal errors. Getting the most recent version of node seemed to resolve these.

I needed to run `bower update` as per [the troubleshooting guide](http://habitica.wikia.com/wiki/Installation_troubleshooting), but running `grunt run:dev` returned errors and ultimately seemed not to be needed.

Simply running `mongod` returns that it is already running. It might be running by default on ubuntu. I resolved this by running a `sudo killall mongod` then `sudo mongod`.

When in doubt, wipe node_modules then repeat the npm install steps.
