<p align="center">
  <img width="290" height="70" src="https://discourse-cdn-sjc1.com/business4/uploads/electroneum/original/1X/ef9300fcffa064903d5ce01bc9e1943f913fc795.jpg">
</p>

<h4 align="center">Electroneum is a fast, secure, mobile based cryptocurrency. </h4>

<p align="center">
  <img width="525" height="315" src="https://discourse-cdn-sjc1.com/business4/uploads/electroneum/original/2X/9/9219c8414cacc641767f8804eccd740443d05fcb.gif">
</p>

<p align="center">
  <a href="#introduction">Introduction</a> •
  <a href="#development-resources">Development Resources</a> •
  <a href="#about-this-project">About this Project</a> •
  <a href="#compiling-electroneum-from-source">Compiling from Source</a> •
  <a href="#license">License</a>
</p>

## Introduction

Electroneum uses a cryptographically sound system to allow you to send and receive your tokens without your transactions being easily revealed on the blockchain. This ensures that all token transfers remain absolutely private by default, but if necessary, can be proven to a third party by providing specific keys.

**Security:** Using the power of a distributed peer-to-peer consensus network, every transaction on the network is cryptographically secured. Individual wallets have a 25 word mnemonic seed that is only displayed once, and can be written down to backup the wallet. Wallet files are encrypted with a passphrase to ensure they are useless if stolen.

Electroneum (and its group companies) have separately developed proprietary software which can be used in conjunction with this project. This software is subject to separate terms and conditions which are available at https://electroneum.com .

## Development Resources

- GitHub: [https://github.com/electroneum/electroneum](https://github.com/electroneum/electroneum)

As with many development projects, the repository on Github is considered to be the "staging" area for the latest changes. Before changes are merged into that branch on the main repository, they are tested by individual developers in their own branches, submitted as a pull request, and then subsequently tested by contributors who focus on testing and code reviews. That having been said, the repository should be carefully considered before using it in a production environment, unless there is a patch in the repository for a particular show-stopping issue you are experiencing. It is generally a better idea to use a tagged release for stability.

**Anyone is welcome to contribute to Electroneum's codebase!** If you have a fix or code change, feel free to submit it as a pull request directly to the "master" branch. In cases where the change is relatively small or does not affect other parts of the codebase it may be merged in immediately by any one of the collaborators. On the other hand, if the change is particularly large or complex, it is expected that it will be discussed at length either well in advance of the pull request being submitted, or even directly on the pull request.

## About this Project

This is the core implementation of Electroneum. It is open source and completely free to use without restrictions, except for those specified in the license agreement below.

## License

See [LICENSE](LICENSE).

## Copyright

Copyright (c) 2017-2019, The Electroneum Project
Copyright (c) 2014-2017, The Monero Project
Portions Copyright (c) 2012-2013, The Cryptonote developers

## Scheduled software upgrades

| Software upgrade block height | Date       | Fork version | Minimum Electroneum version | Recommended Electroneum version | Details                                                                            |
| ------------------------------ | -----------| ----------------- | ---------------------- | -------------------------- | ---------------------------------------------------------------------------------- |
| 307500                         | 2018-05-30 | v6                | v2.0.0.0              | v2.0.0.0                  | Disable Mixin, Disable RingCT, Base Fee to 0.10 from 0.01, 120s Block Time, Anti-Asic Resistance         |
| 324500                         | 2018-07-05 | v7                | v2.1.0.0              | v2.1.0.0                  | Enable ASIC         |
| 589169                         | 2019-07-08 | v8                | v3.0.0.0              | v3.0.0.0                  | Migration to our next generation moderated blockchain with Proof of Responsbility. 300kB Blocks : Increased TPS. Improved Unlock Time (5 Blocks), Many Security Improvements, HackerOne Fixes, Reduced Block Reward By 75% (A Double Halvening)|

X's indicate that these details have not been determined as of commit date.

Please Note that Electroneum no longer supports, develops or maintains any version other than the most recent version.

## Vulnerability Response Process

See [HackerOne](https://hackerone.com/electroneum).

## Installing Electroneum from a Package

Packages are available for

* Ubuntu and [snap supported](https://snapcraft.io/docs/core/install) systems, via a community contributed build.

    snap install electroneum --beta

Installing a snap is very quick. Snaps are secure. They are isolated with all of their dependencies. Snaps also auto update when a new version is released.

* Arch Linux (via [AUR](https://aur.archlinux.org/)):
  - Stable release: [`electroneum`](https://aur.archlinux.org/packages/electroneum)
  - Bleeding edge: [`electroneum-git`](https://aur.archlinux.org/packages/electroneum-git)

| Software upgrade block height  | Date       | Fork version      | Minimum Monero version | Recommended Monero version | Details                                                                            |  
| ------------------------------ | -----------| ----------------- | ---------------------- | -------------------------- | ---------------------------------------------------------------------------------- |
| 1009827                        | 2016-03-22 | v2                | v0.9.4                 | v0.9.4                     | Allow only >= ringsize 3, blocktime = 120 seconds, fee-free blocksize 60 kb       |
| 1141317                        | 2016-09-21 | v3                | v0.9.4                 | v0.10.0                    | Splits coinbase into denominations  |
| 1220516                        | 2017-01-05 | v4                | v0.10.1                | v0.10.2.1                  | Allow normal and RingCT transactions |
| 1288616                        | 2017-04-15 | v5                | v0.10.3.0              | v0.10.3.1                  | Adjusted minimum blocksize and fee algorithm      |
| 1400000                        | 2017-09-16 | v6                | v0.11.0.0              | v0.11.0.0                  | Allow only RingCT transactions, allow only >= ringsize 5      |
| 1546000                        | 2018-04-06 | v7                | v0.12.0.0              | v0.12.3.0                  | Cryptonight variant 1, ringsize >= 7, sorted inputs
| 1685555                        | 2018-10-18 | v8                | v0.13.0.0              | v0.13.0.4                  | max transaction size at half the penalty free block size, bulletproofs enabled, cryptonight variant 2, fixed ringsize [11](https://youtu.be/KOO5S4vxi0o)
| 1686275                        | 2018-10-19 | v9                | v0.13.0.0              | v0.13.0.4                  | bulletproofs required
| 1788000                        | 2019-03-09 | v10               | v0.14.0.0              | v0.14.1.2                  | New PoW based on Cryptonight-R, new block weight algorithm, slightly more efficient RingCT format
| 1788720                        | 2019-03-10 | v11               | v0.14.0.0              | v0.14.1.2                  | forbid old RingCT transaction format
| XXXXXXX                        | 2019-10-XX | XX                | XXXXXXXXX              | XXXXXXXXX                  | X

        docker build -t electroneum .
     
        # either run in foreground
        docker run -it -v /electroneum/chain:/root/.electroneum -v /electroneum/wallet:/wallet -p 26967:26967 electroneum

        # or in background
        docker run -it -d -v /electroneum/chain:/root/.electroneum -v /electroneum/wallet:/wallet -p 26967:26967 electroneum

Approximately three months prior to a scheduled software upgrade, a branch from Master will be created with the new release version tag. Pull requests that address bugs should then be made to both Master and the new release branch. Pull requests that require extensive review and testing (generally, optimizations and new features) should *not* be made to the release branch.

## Compiling Electroneum from Source

### Dependencies

The following table summarizes the tools and libraries required to build. A
few of the libraries are also included in this repository (marked as
"Vendored"). By default, the build uses the library installed on the system,
and ignores the vendored sources. However, if no library is found installed on
the system, then the vendored source will be built and used. The vendored
sources are also used for statically-linked builds because distribution
packages often include only shared library binaries (`.so`) but not static
library archives (`.a`).

| Dep          | Min. version  | Vendored | Debian/Ubuntu pkg  | Arch pkg     | Fedora            | Optional | Purpose        |
| ------------ | ------------- | -------- | ------------------ | ------------ | ----------------- | -------- | -------------- |
| GCC          | 4.7.3         | NO       | `build-essential`  | `base-devel` | `gcc`             | NO       |                |
| CMake        | 3.5           | NO       | `cmake`            | `cmake`      | `cmake`           | NO       |                |
| pkg-config   | any           | NO       | `pkg-config`       | `base-devel` | `pkgconf`         | NO       |                |
| Boost        | 1.58          | NO       | `libboost-all-dev` | `boost`      | `boost-devel`     | NO       | C++ libraries  |
| OpenSSL      | basically any | NO       | `libssl-dev`       | `openssl`    | `openssl-devel`   | NO       | sha256 sum     |
| libzmq       | 3.0.0         | NO       | `libzmq3-dev`      | `zeromq`     | `cppzmq-devel`    | NO       | ZeroMQ library |
| OpenPGM      | ?             | NO       | `libpgm-dev`       | `libpgm`     | `openpgm-devel`   | NO       | For ZeroMQ     |
| libnorm[2]   | ?             | NO       | `libnorm-dev`      |              |               `   | YES      | For ZeroMQ     |
| libunbound   | 1.4.16        | YES      | `libunbound-dev`   | `unbound`    | `unbound-devel`   | NO       | DNS resolver   |
| libsodium    | ?             | NO       | `libsodium-dev`    | `libsodium`  | `libsodium-devel` | NO       | cryptography   |
| libunwind    | any           | NO       | `libunwind8-dev`   | `libunwind`  | `libunwind-devel` | YES      | Stack traces   |
| liblzma      | any           | NO       | `liblzma-dev`      | `xz`         | `xz-devel`        | YES      | For libunwind  |
| libreadline  | 6.3.0         | NO       | `libreadline6-dev` | `readline`   | `readline-devel`  | YES      | Input editing  |
| ldns         | 1.6.17        | NO       | `libldns-dev`      | `ldns`       | `ldns-devel`      | YES      | SSL toolkit    |
| expat        | 1.1           | NO       | `libexpat1-dev`    | `expat`      | `expat-devel`     | YES      | XML parsing    |
| GTest        | 1.5           | YES      | `libgtest-dev`[1]  | `gtest`      | `gtest-devel`     | YES      | Test suite     |
| Doxygen      | any           | NO       | `doxygen`          | `doxygen`    | `doxygen`         | YES      | Documentation  |
| Graphviz     | any           | NO       | `graphviz`         | `graphviz`   | `graphviz`        | YES      | Documentation  |


[1] On Debian/Ubuntu `libgtest-dev` only includes sources and headers. You must
build the library binary manually. This can be done with the following command ```sudo apt-get install libgtest-dev && cd /usr/src/gtest && sudo cmake . && sudo make && sudo mv libg* /usr/lib/ ```
[2] libnorm-dev is needed if your zmq library was built with libnorm, and not needed otherwise

Install all dependencies at once on Debian/Ubuntu:

``` sudo apt update && sudo apt install build-essential cmake pkg-config libboost-all-dev libssl-dev libzmq3-dev libunbound-dev libsodium-dev libunwind8-dev liblzma-dev libreadline6-dev libldns-dev libexpat1-dev doxygen graphviz libpgm-dev```

Install all dependencies at once on macOS with the provided Brewfile:
``` brew update && brew bundle --file=contrib/brew/Brewfile ```

FreeBSD one liner for required to build dependencies
```pkg install git gmake cmake pkgconf boost-libs cppzmq libsodium```

### Cloning the repository

Clone recursively to pull-in needed submodule(s):

`$ git clone --recursive https://github.com/monero-project/monero`

If you already have a repo cloned, initialize and update:

`$ cd monero && git submodule init && git submodule update`

On OSX:
Homebrew installs OpenSSL but doesn’t link it to /usr/local/include, where the compiler looks into during #include<…> Thus, you must manually link it instead:

```ln -s /usr/local/opt/openssl/include/openssl /usr/local/include```
```ln -s /usr/local/Cellar/openssl/[version]/include/openssl /usr/bin/openssl```
```ln -s /usr/local/opt/openssl/lib/libssl.1.0.0.dylib /usr/local/lib/```

### Build instructions

Electroneum uses the CMake build system and a top-level [Makefile](Makefile) that
invokes cmake commands as needed.

#### On Linux and macOS

* Install the dependencies
* Change to the root of the source code directory, change to the most recent release branch, and build:

        cd electroneum
        make

    *Optional*: If your machine has several cores and enough memory, enable
    parallel build by running `make -j<number of threads>` instead of `make`. For
    this to be worthwhile, the machine should have one core and about 2GB of RAM
    available per thread.

    *Note*: If cmake can not find zmq.hpp file on macOS, installing `zmq.hpp` from
    https://github.com/zeromq/cppzmq to `/usr/local/include` should fix that error.

    *Note*: The instructions above will compile the most stable release of the
    Monero software. If you would like to use and test the most recent software,
    use ```git checkout master```. The master branch may contain updates that are
    both unstable and incompatible with release software, though testing is always
    encouraged.

* The resulting executables can be found in `build/release/bin`

* Add `PATH="$PATH:$HOME/electroneum/build/release/bin"` to `.profile`

* Run electroneum with `electroneumd --detach`

* **Optional**: build and run the test suite to verify the binaries:

    ```bash
    make release-test
    ```

    *NOTE*: `core_tests` test may take a few hours to complete.

* **Optional**: to build binaries suitable for debugging:

    ```bash
    make debug
    ```

* **Optional**: to build statically-linked binaries:

    ```bash
    make release-static
    ```

Dependencies need to be built with -fPIC. Static libraries usually aren't, so you may have to build them yourself with -fPIC. Refer to their documentation for how to build them.

* **Optional**: build documentation in `doc/html` (omit `HAVE_DOT=YES` if `graphviz` is not installed):

    ```bash
    HAVE_DOT=YES doxygen Doxyfile
    ```

#### On Windows:

Binaries for Windows are built on Windows using the MinGW toolchain within
[MSYS2 environment](https://www.msys2.org). The MSYS2 environment emulates a
POSIX system. The toolchain runs within the environment and *cross-compiles*
binaries that can run outside of the environment as a regular Windows
application.

**Preparing the build environment**

* Download and install the [MSYS2 installer](https://www.msys2.org), either the 64-bit or the 32-bit package, depending on your system.
* Open the MSYS shell via the `MSYS2 Shell` shortcut
* Update packages using pacman:  

    ```bash
    pacman -Syu
    ```

* Exit the MSYS shell using Alt+F4  
* Edit the properties for the `MSYS2 Shell` shortcut changing "msys2_shell.bat" to "msys2_shell.cmd -mingw64" for 64-bit builds or "msys2_shell.cmd -mingw32" for 32-bit builds
* Restart MSYS shell via modified shortcut and update packages again using pacman:  

    ```bash
    pacman -Syu
    ```


* Install dependencies:

    To build for 64-bit Windows:

    ```bash
    pacman -S mingw-w64-x86_64-toolchain make mingw-w64-x86_64-cmake mingw-w64-x86_64-boost mingw-w64-x86_64-openssl mingw-w64-x86_64-zeromq mingw-w64-x86_64-libsodium mingw-w64-x86_64-hidapi
    ```

    To build for 32-bit Windows:

    ```bash
    pacman -S mingw-w64-i686-toolchain make mingw-w64-i686-cmake mingw-w64-i686-boost mingw-w64-i686-openssl mingw-w64-i686-zeromq mingw-w64-i686-libsodium mingw-w64-i686-hidapi
    ```

* Open the MingW shell via `MinGW-w64-Win64 Shell` shortcut on 64-bit Windows
  or `MinGW-w64-Win64 Shell` shortcut on 32-bit Windows. Note that if you are
  running 64-bit Windows, you will have both 64-bit and 32-bit MinGW shells.

**Cloning**

* To git clone, run:

    ```bash
    git clone --recursive https://github.com/monero-project/monero.git
    ```

**Building**

* Change to the cloned directory, run:

    ```bash
    cd monero
    ```

* If you would like a specific [version/tag](https://github.com/monero-project/monero/tags), do a git checkout for that version. eg. 'v0.14.1.2'. If you don't care about the version and just want binaries from master, skip this step:
	
    ```bash
    git checkout v0.14.1.2
    ```

* If you are on a 64-bit system, run:

    ```bash
    make release-static-win64
    ```

* If you are on a 32-bit system, run:

    ```bash
    make release-static-win32
    ```

* The resulting executables can be found in `build/release/bin`

### Building Portable Statically Linked Binaries

By default, in either dynamically or statically linked builds, binaries target the specific host processor on which the build happens and are not portable to other processors. Portable binaries can be built using the following targets:

* ```make release-static-linux-x86_64``` builds binaries on Linux on x86_64 portable across POSIX systems on x86_64 processors
* ```make release-static-linux-i686``` builds binaries on Linux on x86_64 or i686 portable across POSIX systems on i686 processors
* ```make release-static-linux-armv8``` builds binaries on Linux portable across POSIX systems on armv8 processors
* ```make release-static-linux-armv7``` builds binaries on Linux portable across POSIX systems on armv7 processors
* ```make release-static-linux-armv6``` builds binaries on Linux portable across POSIX systems on armv6 processors
* ```make release-static-win64``` builds binaries on 64-bit Windows portable across 64-bit Windows systems
* ```make release-static-win32``` builds binaries on 64-bit or 32-bit Windows portable across 32-bit Windows systems

## Running electroneumd

The build places the binary in `bin/` sub-directory within the build directory
from which cmake was invoked (repository root by default). To run in
foreground:

    ./bin/electroneumd

To list all available options, run `./bin/electroneumd --help`.  Options can be
specified either on the command line or in a configuration file passed by the
`--config-file` argument.  To specify an option in the configuration file, add
a line with the syntax `argumentname=value`, where `argumentname` is the name
of the argument without the leading dashes, for example `log-level=1`.

To run in background:

    ./bin/electroneumd --log-file electroneumd.log --detach

To run as a systemd service, copy
[electroneumd.service](utils/systemd/electroneumd.service) to `/etc/systemd/system/` and
[electroneumd.conf](utils/conf/electroneumd.conf) to `/etc/`. The [example
service](utils/systemd/electroneumd.service) assumes that the user `electroneum` exists
and its home is the data directory specified in the [example
config](utils/conf/electroneumd.conf).

If you're on Mac, you may need to add the `--max-concurrency 1` option to
electroneum-wallet-cli, and possibly electroneumd, if you get crashes refreshing.

 ## Using Tor

 Whilst Electroneum isn't made to integrate with Tor, it can be used wrapped with torsocks, by
 setting the following configuration parameters and environment variables:

 * `--p2p-bind-ip 127.0.0.1` on the command line or `p2p-bind-ip=127.0.0.1` in
   electroneumd.conf to disable listening for connections on external interfaces.
 * `--no-igd` on the command line or `no-igd=1` in electroneumd.conf to disable IGD
   (UPnP port forwarding negotiation), which is pointless with Tor.
 * `DNS_PUBLIC=tcp` or `DNS_PUBLIC=tcp://x.x.x.x` where x.x.x.x is the IP of the
   desired DNS server, for DNS requests to go over TCP, so that they are routed
   through Tor. When IP is not specified, electroneumd uses the default list of
   servers defined in [src/common/dns_utils.cpp](src/common/dns_utils.cpp).
 * `TORSOCKS_ALLOW_INBOUND=1` to tell torsocks to allow electroneumd to bind to interfaces
    to accept connections from the wallet. On some Linux systems, torsocks
    allows binding to localhost by default, so setting this variable is only
    necessary to allow binding to local LAN/VPN interfaces to allow wallets to
    connect from remote hosts. On other systems, it may be needed for local wallets
   as well.
* Do NOT pass `--detach` when running through torsocks with systemd, (see
  [utils/systemd/electroneumd.service](utils/systemd/electroneumd.service) for details).
* If you use the wallet with a Tor daemon via the loopback IP (eg, 127.0.0.1:9050),
  then use `--untrusted-daemon` unless it is your own hidden service.
 Example command line to start electroneumd through Tor:
      DNS_PUBLIC=tcp torsocks electroneumd --p2p-bind-ip 127.0.0.1 --no-igd

 ### Using Tor on Tails

 TAILS ships with a very restrictive set of firewall rules. Therefore, you need
 to add a rule to allow this connection too, in addition to telling torsocks to
 allow inbound connections. Full example:

     sudo iptables -I OUTPUT 2 -p tcp -d 127.0.0.1 -m tcp --dport 26968 -j ACCEPT
     DNS_PUBLIC=tcp torsocks ./electroneumd --p2p-bind-ip 127.0.0.1 --no-igd --rpc-bind-ip 127.0.0.1 \
         --data-dir /home/amnesia/Persistent/your/directory/to/the/blockchain
