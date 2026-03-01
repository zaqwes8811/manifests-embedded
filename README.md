# Install Google Repo

```
# Google Repo from stock repos has some troubles, better install like it

mkdir ~/bin/

curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo

```

# Openwrt on RPI4

```
mkdir ~/owrt_rpi4 && cd ~/owrt_rpi4
~/bin/repo init -u https://github.com/hedge-in-fog/manifests-embedded.git -b main -m owrt_rpi4.xml
repo sync -j `nproc`
```

# Soft router

```
mkdir ~/soft_router && cd ~/soft_router
~/bin/repo init -u https://github.com/hedge-in-fog/manifests-embedded.git -b main -m soft_router.xml
repo sync -j `nproc`
```

# EOL CV

```
mkdir ~/eol_cv && cd ~/eol_cv
~/bin/repo init -u https://github.com/hedge-in-fog/manifests-embedded.git -b main -m eol_cv.xml
repo sync -j `nproc`
```