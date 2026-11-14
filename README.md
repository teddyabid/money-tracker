# Money Tracker APK

## Way 1: GitHub diye (computer-e Android Studio lagbe na)
1. github.com-e free account e notun repository banao (jemon money-tracker).
2. Ei folder-er shob file (www, .github, package.json, capacitor.config.json, .gitignore) upload koro.
   (Web-e "Add file" -> "Upload files" diye .github folder shoho dite hobe.)
3. Repository-r "Actions" tab -> "Build APK" -> build shesh hole (4-6 min) niche "Artifacts" theke
   money-tracker-apk download koro. Zip khulle app-debug.apk paabe.
4. APK phone-e pathao, tap kore install koro (Install unknown apps allow korte hobe).

## Way 2: Nijer computer-e
Node 18+, Java 17 ar Android Studio (SDK shoho) lagbe.
    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk

## App change korte chaile
www/index.html edit koro, tarpor build abar chalao.
