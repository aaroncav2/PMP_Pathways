# PMP Pathways – Android app (Capacitor + AdMob)
1. Create a free GitHub repo, upload everything in this folder (keep the .github folder).
2. Actions tab -> "Build Android (APK + AAB)" -> Run workflow -> download `debug-apk` artifact and install it.
3. For Google Play: run "Create upload keystore" once, add 4 repo secrets (KEYSTORE_BASE64, KEYSTORE_PASSWORD, KEY_ALIAS=upload, KEY_PASSWORD), re-run build, download `release-for-play-store` (.aab).
4. Replace test ad IDs in www/admob.config.json with your real AdMob IDs and set "testMode": false before publishing.
5. Change appId in capacitor.config.json (e.g. com.yourname.pmppathways) BEFORE your first Play upload – it can never change afterwards.
