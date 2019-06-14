# sample-web-server
テクノロジー（藤原）Node.jsによるサンプルWebサーバ

```
ここffuyang@DESKTOP-8E6S251:~/fujiwara$ cd sample-web-server/
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ ^M$ curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
$: command not foundffuyang:

ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
[sudo] password for ffuyang:

## Installing the NodeSource Node.js 12.x repo...


## Populating apt-get cache...

+ apt-get update
Hit:1 http://security.ubuntu.com/ubuntu bionic-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu bionic InRelease
Hit:3 http://archive.ubuntu.com/ubuntu bionic-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu bionic-backports InRelease
Reading package lists... Done

## Confirming "bionic" is supported...

+ curl -sLf -o /dev/null 'https://deb.nodesource.com/node_12.x/dists/bionic/Release'

## Adding the NodeSource signing key to your keyring...

+ curl -s https://deb.nodesource.com/gpgkey/nodesource.gpg.key | apt-key add -
OK

## Creating apt sources list file for the NodeSource Node.js 12.x repo...

+ echo 'deb https://deb.nodesource.com/node_12.x bionic main' > /etc/apt/sources.list.d/nodesource.list
+ echo 'deb-src https://deb.nodesource.com/node_12.x bionic main' >> /etc/apt/sources.list.d/nodesource.list

## Running `apt-get update` for you...

+ apt-get update
Get:1 https://deb.nodesource.com/node_12.x bionic InRelease [4584 B]
Hit:2 http://security.ubuntu.com/ubuntu bionic-security InRelease
Hit:3 http://archive.ubuntu.com/ubuntu bionic InRelease
Get:4 https://deb.nodesource.com/node_12.x bionic/main amd64 Packages [765 B]
Hit:5 http://archive.ubuntu.com/ubuntu bionic-updates InRelease
Hit:6 http://archive.ubuntu.com/ubuntu bionic-backports InRelease
Fetched 5349 B in 2s (2470 B/s)
Reading package lists... Done

## Run `sudo apt-get install -y nodejs` to install Node.js 12.x and npm
## You may also need development tools to build native addons:
     sudo apt-get install gcc g++ make
## To install the Yarn package manager, run:
     curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
     echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
     sudo apt-get update && sudo apt-get install yarn


ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ $ sudo apt install -y build-essential
$: command not found
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ sudo apt install -y build-essential
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following package was automatically installed and is no longer required:
  libfreetype6
Use 'sudo apt autoremove' to remove it.
The following additional packages will be installed:
  binutils binutils-common binutils-x86-64-linux-gnu cpp cpp-7 dpkg-dev fakeroot g++ g++-7 gcc gcc-7
  gcc-7-base gcc-8-base libalgorithm-diff-perl libalgorithm-diff-xs-perl libalgorithm-merge-perl
  libasan4 libatomic1 libbinutils libc-dev-bin libc6-dev libcc1-0 libcilkrts5 libdpkg-perl libfakeroot
  libfile-fcntllock-perl libgcc-7-dev libgcc1 libgomp1 libisl19 libitm1 liblsan0 libmpc3 libmpx2
  libquadmath0 libstdc++-7-dev libstdc++6 libtsan0 libubsan0 linux-libc-dev make manpages-dev
Suggested packages:
  binutils-doc cpp-doc gcc-7-locales debian-keyring g++-multilib g++-7-multilib gcc-7-doc
  libstdc++6-7-dbg gcc-multilib autoconf automake libtool flex bison gdb gcc-doc gcc-7-multilib
  libgcc1-dbg libgomp1-dbg libitm1-dbg libatomic1-dbg libasan4-dbg liblsan0-dbg libtsan0-dbg
  libubsan0-dbg libcilkrts5-dbg libmpx2-dbg libquadmath0-dbg glibc-doc bzr libstdc++-7-doc make-doc
The following NEW packages will be installed:
  binutils binutils-common binutils-x86-64-linux-gnu build-essential cpp cpp-7 dpkg-dev fakeroot g++
  g++-7 gcc gcc-7 gcc-7-base libalgorithm-diff-perl libalgorithm-diff-xs-perl libalgorithm-merge-perl
  libasan4 libatomic1 libbinutils libc-dev-bin libc6-dev libcc1-0 libcilkrts5 libdpkg-perl libfakeroot
  libfile-fcntllock-perl libgcc-7-dev libgomp1 libisl19 libitm1 liblsan0 libmpc3 libmpx2 libquadmath0
  libstdc++-7-dev libtsan0 libubsan0 linux-libc-dev make manpages-dev
The following packages will be upgraded:
  gcc-8-base libgcc1 libstdc++6
3 upgraded, 40 newly installed, 0 to remove and 205 not upgraded.
Need to get 37.6 MB of archives.
After this operation, 161 MB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 gcc-8-base amd64 8.3.0-6ubuntu1~18.04.1 [18.7 kB]
Get:2 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libstdc++6 amd64 8.3.0-6ubuntu1~18.04.1 [400 kB]
Get:3 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libgcc1 amd64 1:8.3.0-6ubuntu1~18.04.1 [40.7 kB]
Get:4 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 binutils-common amd64 2.30-21ubuntu1~18.04.2 [193 kB]
Get:5 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libbinutils amd64 2.30-21ubuntu1~18.04.2 [503 kB]
Get:6 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 binutils-x86-64-linux-gnu amd64 2.30-21ubuntu1~18.04.2 [1856 kB]
Get:7 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 binutils amd64 2.30-21ubuntu1~18.04.2 [3396 B]
Get:8 http://archive.ubuntu.com/ubuntu bionic/main amd64 libc-dev-bin amd64 2.27-3ubuntu1 [71.8 kB]
Get:9 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 linux-libc-dev amd64 4.15.0-51.55 [1005 kB]
Get:10 http://archive.ubuntu.com/ubuntu bionic/main amd64 libc6-dev amd64 2.27-3ubuntu1 [2587 kB]
Get:11 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 gcc-7-base amd64 7.4.0-1ubuntu1~18.04.1 [18.9 kB]
Get:12 http://archive.ubuntu.com/ubuntu bionic/main amd64 libisl19 amd64 0.19-1 [551 kB]
Get:13 http://archive.ubuntu.com/ubuntu bionic/main amd64 libmpc3 amd64 1.1.0-1 [40.8 kB]
Get:14 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 cpp-7 amd64 7.4.0-1ubuntu1~18.04.1 [6742 kB]
Get:15 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 cpp amd64 4:7.4.0-1ubuntu2.3 [27.7 kB]Get:16 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libcc1-0 amd64 8.3.0-6ubuntu1~18.04.1 [47.4 kB]
Unpacking manpages-dev (4.15-1) ...
Setting up libquadmath0:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up libgomp1:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up libatomic1:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up libcc1-0:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up make (4.1-9.1ubuntu1) ...
Setting up libtsan0:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up linux-libc-dev:amd64 (4.15.0-51.55) ...
Setting up libdpkg-perl (1.19.0.5ubuntu2.1) ...
Setting up liblsan0:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up gcc-7-base:amd64 (7.4.0-1ubuntu1~18.04.1) ...
Setting up binutils-common:amd64 (2.30-21ubuntu1~18.04.2) ...
Setting up libfile-fcntllock-perl (0.22-3build2) ...
Setting up libmpx2:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Processing triggers for libc-bin (2.27-3ubuntu1) ...
Setting up libfakeroot:amd64 (1.22-2ubuntu1) ...
Setting up libalgorithm-diff-perl (1.19.03-1) ...
Processing triggers for man-db (2.8.3-2) ...
Setting up libmpc3:amd64 (1.1.0-1) ...
Setting up libc-dev-bin (2.27-3ubuntu1) ...
Setting up manpages-dev (4.15-1) ...
Setting up libc6-dev:amd64 (2.27-3ubuntu1) ...
Setting up libitm1:amd64 (8.3.0-6ubuntu1~18.04.1) ...
Setting up libisl19:amd64 (0.19-1) ...
Setting up libasan4:amd64 (7.4.0-1ubuntu1~18.04.1) ...
Setting up libbinutils:amd64 (2.30-21ubuntu1~18.04.2) ...
Setting up libcilkrts5:amd64 (7.4.0-1ubuntu1~18.04.1) ...
Setting up libubsan0:amd64 (7.4.0-1ubuntu1~18.04.1) ...
Setting up fakeroot (1.22-2ubuntu1) ...
update-alternatives: using /usr/bin/fakeroot-sysv to provide /usr/bin/fakeroot (fakeroot) in auto mode
  python2.7-minimal
0 upgraded, 8 newly installed, 0 to remove and 205 not upgraded.
Need to get 20.7 MB of archives.
After this operation, 97.5 MB of additional disk space will be used.
Get:1 https://deb.nodesource.com/node_12.x bionic/main amd64 nodejs amd64 12.4.0-1nodesource1 [16.7 MB]
Get:2 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libpython2.7-minimal amd64 2.7.15-4ubuntu4~18.04 [335 kB]
Get:3 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 python2.7-minimal amd64 2.7.15-4ubuntu4~18.04 [1295 kB]
Get:4 http://archive.ubuntu.com/ubuntu bionic/main amd64 python-minimal amd64 2.7.15~rc1-1 [28.1 kB]
Get:5 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 libpython2.7-stdlib amd64 2.7.15-4ubuntu4~18.04 [1915 kB]
Get:6 http://archive.ubuntu.com/ubuntu bionic-updates/main amd64 python2.7 amd64 2.7.15-4ubuntu4~18.04 [239 kB]
Get:7 http://archive.ubuntu.com/ubuntu bionic/main amd64 libpython-stdlib amd64 2.7.15~rc1-1 [7620 B]
Get:8 http://archive.ubuntu.com/ubuntu bionic/main amd64 python amd64 2.7.15~rc1-1 [140 kB]
Fetched 20.7 MB in 18s (1161 kB/s)
Selecting previously unselected package libpython2.7-minimal:amd64.
(Reading database ... 33987 files and directories currently installed.)
Preparing to unpack .../0-libpython2.7-minimal_2.7.15-4ubuntu4~18.04_amd64.deb ...
Unpacking libpython2.7-minimal:amd64 (2.7.15-4ubuntu4~18.04) ...
Selecting previously unselected package python2.7-minimal.
Preparing to unpack .../1-python2.7-minimal_2.7.15-4ubuntu4~18.04_amd64.deb ...
Unpacking python2.7-minimal (2.7.15-4ubuntu4~18.04) ...
Selecting previously unselected package python-minimal.
Preparing to unpack .../2-python-minimal_2.7.15~rc1-1_amd64.deb ...
Unpacking python-minimal (2.7.15~rc1-1) ...
Selecting previously unselected package libpython2.7-stdlib:amd64.
Preparing to unpack .../3-libpython2.7-stdlib_2.7.15-4ubuntu4~18.04_amd64.deb ...
Unpacking libpython2.7-stdlib:amd64 (2.7.15-4ubuntu4~18.04) ...
Selecting previously unselected package python2.7.
Preparing to unpack .../4-python2.7_2.7.15-4ubuntu4~18.04_amd64.deb ...
Unpacking python2.7 (2.7.15-4ubuntu4~18.04) ...
Selecting previously unselected package libpython-stdlib:amd64.
Preparing to unpack .../5-libpython-stdlib_2.7.15~rc1-1_amd64.deb ...
Unpacking libpython-stdlib:amd64 (2.7.15~rc1-1) ...
Setting up libpython2.7-minimal:amd64 (2.7.15-4ubuntu4~18.04) ...
Setting up python2.7-minimal (2.7.15-4ubuntu4~18.04) ...
Linking and byte-compiling packages for runtime python2.7...
Setting up python-minimal (2.7.15~rc1-1) ...
Selecting previously unselected package python.
(Reading database ... 34735 files and directories currently installed.)
Preparing to unpack .../python_2.7.15~rc1-1_amd64.deb ...
Unpacking python (2.7.15~rc1-1) ...
Selecting previously unselected package nodejs.
Preparing to unpack .../nodejs_12.4.0-1nodesource1_amd64.deb ...
Unpacking nodejs (12.4.0-1nodesource1) ...
Processing triggers for mime-support (3.60ubuntu1) ...
Setting up nodejs (12.4.0-1nodesource1) ...###################################......................]
Processing triggers for man-db (2.8.3-2) ...
Setting up libpython2.7-stdlib:amd64 (2.7.15-4ubuntu4~18.04) ...
Setting up python2.7 (2.7.15-4ubuntu4~18.04) ...





















Progress: [ 76%] [##############################################################....................]









Progress: [ 78%] [################################################################..................]









Progress: [ 85%] [######################################################################............]














Progress: [ 88%] [########################################################################..........] Setting up libpython-stdlib:amd64 (2.7.15~rc1-1) ...
Setting up python (2.7.15~rc1-1) ...##########################################################......]
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ node - v
Welcome to Node.js v12.4.0.
Type ".help" for more information.
>
(To exit, press ^C again or ^D or type .exit)
>
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ git add .
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ mkdir mywebapi
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server$ cd mywebapi/
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (mywebapi)
version: (1.0.0)
description:
entry point: (index.js)
test command:
git repository:
keywords:
author:
license: (ISC)
About to write to /mnt/c/Users/raiden/Documents/fujiwara/sample-web-server/mywebapi/package.json:

{
  "name": "mywebapi",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}


Is this OK? (yes) yes
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$ npm install - -save express
npm ERR! code E404
npm ERR! 404 Not Found - GET https://registry.npmjs.org/- - Not found
npm ERR! 404
npm ERR! 404  '-@latest' is not in the npm registry.
npm ERR! 404 You should bug the author to publish it (or use the name yourself!)
npm ERR! 404
npm ERR! 404 Note that you can also install from a
npm ERR! 404 tarball, folder, http url, or git url.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/ffuyang/.npm/_logs/2019-06-14T02_45_11_118Z-debug.log
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$ npm install --save express
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN mywebapi@1.0.0 No description
npm WARN mywebapi@1.0.0 No repository field.

+ express@4.17.1
added 50 packages from 37 contributors and audited 126 packages in 111.578s
found 0 vulnerabilities

ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$ node index.js
Listening on port 3000
^C
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$ node index.js
Listening on port 3000
^C
ffuyang@DESKTOP-8E6S251:~/fujiwara/sample-web-server/mywebapi$に書く
```
