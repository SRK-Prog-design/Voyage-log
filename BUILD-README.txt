NSSL Voyage Log - real Android app (APK)
=========================================
This folder is a complete Android app project. Two ways to get the APK file:

A) Easiest - build online with GitHub (free, no software to install)
   1. Create a free account at github.com and make a new repository.
   2. Upload ALL files of this folder to it. If the hidden folder ".github" is skipped by the web upload,
      click Add file > Create new file, name it  .github/workflows/build-apk.yml  and paste the text from BUILD-APK-workflow.txt.
   3. Open the Actions tab > "Build APK" > Run workflow. Wait about 3 minutes.
   4. Open the finished run, download "NSSL-Voyage-Log-apk", unzip it to get app-debug.apk.
   5. Copy app-debug.apk to your phone and tap it. Allow "install unknown apps" when asked. The ship icon "Voyage Log" appears in your app drawer.

B) Android Studio on a PC
   1. Install Android Studio, choose File > Open and select this folder.
   2. (Optional, for offline PDF) download https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js
      and save it as app/src/main/assets/jspdf.umd.min.js
   3. Build > Build APK(s). The file is in app/build/outputs/apk/debug/app-debug.apk

Notes
- Backups, CSV and PDF files are saved in Downloads/NSSL Voyage Log.
- Data is stored on the phone. For automatic phone <-> PC sync follow FIREBASE-SETUP.txt (free Firebase database), then enter the URL and code in Data > Auto sync.
- Not yet compiled or tested on a phone - if the build shows an error, send me the message and I will fix it.
