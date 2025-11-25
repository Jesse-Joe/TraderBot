# TraderBot Mobile App

## Wat je nodig hebt

### Voor iOS (App Store):
1. **Mac met Xcode** (gratis in Mac App Store)
2. **Apple Developer Account** - €99/jaar op https://developer.apple.com
3. **iPhone/iPad** voor testen

### Voor Android (Play Store):
1. **Android Studio** (gratis) - https://developer.android.com/studio
2. **Google Play Developer Account** - €25 eenmalig
3. **Android telefoon** voor testen

---

## iOS Build Stappen

### Op je Mac:
```bash
# 1. Open terminal en ga naar project folder
cd /pad/naar/mobile-app

# 2. Installeer dependencies
npm install

# 3. Open Xcode project
npx cap open ios
```

### In Xcode:
1. Selecteer je **Team** (Apple Developer Account) in Signing & Capabilities
2. Verander **Bundle Identifier** naar iets unieks: `com.jouwbedrijf.traderbot`
3. Selecteer je iPhone als target device
4. Klik **Build** (Cmd + B) om te testen
5. Klik **Archive** voor App Store upload

### App Store Connect:
1. Ga naar https://appstoreconnect.apple.com
2. Maak nieuwe app aan
3. Upload via Xcode Organizer
4. Vul alle metadata in (screenshots, beschrijving, etc.)
5. Submit for Review

---

## Android Build Stappen

### Op Windows/Mac/Linux:
```bash
# 1. Open Android Studio
npx cap open android

# 2. Of build APK via command line:
cd android
./gradlew assembleDebug
# APK staat in: android/app/build/outputs/apk/debug/
```

### Play Store:
1. Ga naar https://play.google.com/console
2. Maak nieuwe app aan
3. Upload AAB bestand (niet APK)
4. Vul store listing in
5. Submit for Review

---

## Tips voor Apple Review

Apple keurt soms apps af die alleen een website wrappen. Tips:

1. **Voeg native features toe** - Push notifications zijn al toegevoegd
2. **Offline functionaliteit** - Toon cached data als offline
3. **Goede beschrijving** - Leg uit wat de app doet, niet dat het een website is
4. **Privacy Policy** - Vereist! Host op je website
5. **Geen "beta" of "test"** in de naam

---

## App Store Beschrijving (voorbeeld)

**Naam:** TraderBot - Crypto Trading

**Subtitle:** AI-Powered Trading Dashboard

**Beschrijving:**
TraderBot is een geavanceerde crypto trading dashboard waarmee je real-time je portfolio kunt volgen en automatische trades kunt monitoren.

Features:
- Real-time portfolio tracking
- Live prijzen van 100+ cryptocurrencies
- Push notificaties bij trades
- Gedetailleerde trade geschiedenis
- AI-powered trading signals
- Veilige login met encryptie

**Keywords:** crypto, trading, bitcoin, portfolio, tracker, investment

---

## Support

Bij vragen: jesse13joe@gmail.com
