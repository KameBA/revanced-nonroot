# Credit

Code APKmirror: [revanced-build-template](https://github.com/n0k0m3/revanced-build-template)

Code Uptodown: [revanced-magisk-module](https://github.com/j-hc/revanced-magisk-module)

# Note

🚫 I don't allow someone with a github name's Fioren to download and use my new code.  He/she was used my code but said: "I was created" and "my code"

<div align="center">

[![](https://visitcount.itsvg.in/api?id=luxysiv&label=Visitors&color=0&icon=0&pretty=true)](https://visitcount.itsvg.in)
  
</div>
  
# How to use

✅ Fork this repository 

✅ Enable github actions

✅ Config your patches in folder 

[Revanced](https://github.com/revanced/revanced-patches/releases)

[Revanced Extended](https://github.com/inotia00/revanced-patches/releases)

✅ In [build-rv.sh](./src/build-rv.sh) [build-rve.sh](./src/build-rve.sh) 

✒️ Change apk source to down : APKmirror or Uptodown 

✒️ Add keyword to patch others app 

✅ Run github actions and wait

✅ Take apk in releases

# Add new app or new source to patch

1️⃣ Download source you need

➡ Use : dl_gh "user" "repo" tag" 

➡ (user = revanced,inotia00,kazimmt,kidatai31...) 

➡ (repo = revanced-patches revanced-cli revanced-integrations) You can use j-hc/revanced-cli to --riplib)

➡ (tag = latest or tags/v.... if you need specific patch version)

2️⃣ Patch key words (skip if you no need in/exclude-patches) 

➡ In folder patches creat new file app-to-patches begin by --exclude or --include 

➡ Create patch to include/exclude. Patches can be separated by a space or a newline. Like:

`--exclude patch1 patch2 patch3...`

`--include 
patch4 `

`patch5 `

`patch6...`

still be OK

➡ Use : get_patches_key "app-to-paches"

3️⃣ Get version apk supported 

➡ Use: get_ver "app_name" (Check in [version.info](./src/version.info) (Only revanced/inotia00 source)

➡ Skip this if not found or use get_ver "patch_name" "pkg_name" for different revanced/inotia00 source

➡ Use version="version" to set specific version 

4️⃣ Get apk

➡ In new code I will input all app link revanced supported. Find them(app_name) in [apkmirror.info](./src/apkmirror.info) and [uptodown.info](./src/uptodown.info)

➡ Use : 

get_apkmirror "app_name" for universal app like :YouTube,Twitch...
         
get_apkmirror "app_name" "arch" for arch app like : YouTube Music ,Messenger...

get_uptodown "app_name"

5️⃣ Patch app

➡ Use: patch "app_name" "name-you-like" "arch"

➡ (app_name: above) (name-you-like: Example YouTube-Extended-v$version)

➡ (arch: arm64-v8a,armeabi-v7a,x86,x86_64 and arm) Split apk if you need. Note: blank is same original input APK. Need use j-hc/cli to split Revanced, Revanced Extended still use inotia00/cli

# Problem 

Some apk download not exactly or not supported. Use between APKMirror and Uptodown

# Download mMicroG patched hide-icon from inotia00 patch/source 

<div align="center">

[![Release](https://img.shields.io/github/v/release/inotia00/mMicroG?label=mMicroG)](https://github.com/luxysiv/revanced-nonroot/releases/latest/download/mMicroG.apk)

👆 to download mMicroG

Necessary for non-root users. Install first
  
</div>

# About
This repository can patch YouTube/YouTube Music from revanced/inotia00 source

