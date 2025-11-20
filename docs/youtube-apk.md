# Youtube.apk mit Revanced patchen

## Schritte

*   Revanced CLI von https://github.com/revanced/revanced-cli herunterladen
*   Youtube apk von https://www.apkmirror.com/apk/google-inc/youtube/youtube-20-14-43-release/youtube-20-14-43-2-android-apk-download/ herunterladen
*   Revanced Patches von https://github.com/ReVanced/revanced-patches herunterladen
*   Patchen:  
    `java -jar .\revanced-cli-5.0.1-all.jar patch .\youtube_20.14.43.apk -p .\patches-5.46.0.rvp -o revanced-youtube.apk`
*   Cusom Icon erstellen

*   .png erstellen und mit https://icon.kitchen/ für die diversen Auflösungen ic\_launcher.png generieren lassen
*   gepatchtes .apk entpacken (Voraussetzung apktool)  
    `java -jar .\apktool_2.12.1.jar d .\my-youtube.apk -o yt-src`
*   Eventuell in yt-src\\AndroidManifest.xml im application Element das icon Attribut auf ic\_launcher ändern.
*   in yt-src\\res\\mipmap\* die Icons durch die von icon.kitchen ersetzen
*   Neu Builden  
    `java -jar .\apktool_2.12.1.jar b yt-src -o youtube-revanced-custom.apk`
*   apk signieren (Voraussetzung uber-apk-signer)  
    `java -jar .\uber-apk-signer-1.3.0.jar --apks .\youtube-revanced-custom.apk`

*   youtube-revanced-custom.apk installieren
*   GmsCore (alternative zu Goolge Play Services) von https://rvx.to/de/gmscore/ herunterladen und installieren