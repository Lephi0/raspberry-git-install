# raspberry-git-install
Commands to install latest git and git-lfs on a Raspberry Pi OS.

## Instuctions for latest Git (2.36.1 - time of writing)
1. sudo apt update
2. sudo apt install make libssl-dev libghc-zlib-dev libcurl4-gnutls-dev libexpat1-dev gettext unzip -y
4. wget https://github.com/git/git/archive/refs/tags/v2.36.1.tar.gz *
5. sudo unzip {version}
6. cd git-{version}
7. sudo make prefix=/usr/local all
8. sudo make prefix=/usr/local install
9. git --version

**source can be found at https://github.com/git/git*

## Instuctions for latest Git LFS (3.2.0 - time of writing)
1. curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
2. sudo apt-get install git-lfs
3. git lfs install (initialize git LFS globally)
4. git-lfs --version

### Sources
- https://www.linuxcapable.com/how-to-install-configure-git-on-debian-11/ (install git from source)
- https://github.com/git/git/releases/tag/v2.36.1 (git repository)
- https://github.com/git-lfs/git-lfs/wiki/Installation#source (git-lfs wiki)
