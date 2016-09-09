+++
date = "2016-04-01T11:39:53+01:00"
draft = true
title = "build and sign your android app in meteor"

+++

## Build:

```
meteor build destination/path --server=http://yourapplocation.com --mobile-settings settings.json
```

## Generate sign key:
```
keytool -genkey -alias anAlias -keyalg RSA -keysize 2048 -validity 10000
```

## Sign:

```
jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 release-unsigned.apk theAlias [-keystore smile.keystore]
```


## Compress:

```
~/Library/Android/sdk/build-tools/23.0.3/zipalign 4 release-unsigned.apk alpha-1.apk
```
