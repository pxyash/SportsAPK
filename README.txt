BUILD THE APK
1. Install Android Studio (free): https://developer.android.com/studio
2. File > Open > select this StreamPlayerTV folder. Wait for Gradle sync to finish.
3. Build > Build Bundle(s) / APK(s) > Build APK(s)
4. Click "locate" in the popup. The file is app/build/outputs/apk/debug/app-debug.apk

INSTALL ON ANDROID TV
- Easiest: install "Send Files to TV" on both phone and TV, send the APK, open it.
- Or: put the APK on a USB drive and open it with a TV file manager (e.g. X-plore).
- Or: enable Developer options > Network debugging, then:  adb connect TV_IP  &&  adb install app-debug.apk
- You may need to allow "Install unknown apps" for the file manager.

EDIT CHANNELS
Change app/src/main/assets/index.html (the CHANNELS list), then rebuild.

REMOTE CONTROL
Use the D-pad to move between channel buttons and OK to select. Back exits fullscreen video.
