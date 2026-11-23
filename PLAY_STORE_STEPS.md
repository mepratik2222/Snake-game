# Play Store वर Snake Game टाकण्याचे टप्पे (फक्त मोबाईल वापरून)

## 1. गेम इंटरनेटवर ठेवा (मोफत, HTTPS लिंक लागते)
1. github.com वर मोफत account बनवा (मोबाईल browser, "Desktop site" चालू करा).
2. नवीन repository बनवा, नाव: `snake-game`, Public.
3. या zip मधील सर्व फाइल्स (index.html, manifest.webmanifest, sw.js, privacy.html आणि icons फोल्डर) Upload करा.
4. Settings > Pages > Branch: main > Save. 1-2 मिनिटांनी लिंक मिळेल:
   `https://तुमचे-नाव.github.io/snake-game/`
5. privacy.html मधील `YOUR-EMAIL@example.com` तुमच्या खऱ्या email ने बदला (GitHub वर file उघडून Edit).
   Privacy Policy लिंक: `.../snake-game/privacy.html`

## 2. Android package (.aab) बनवा
1. pwabuilder.com उघडा, तुमची लिंक टाका > Start.
2. "Package for stores" > Android > Google Play.
3. Package ID: `com.तुमचेनाव.snakegame` (हे नंतर बदलता येत नाही).
4. Generate. मिळालेली zip मध्ये `.aab` file आणि `signing.keystore` + password असतात.
   **ही keystore आणि password कायमची सुरक्षित ठेवा** (Google Drive/email). हरवली तर app update करता येत नाही.
5. Zip मधील `assetlinks.json` ची मजकूर GitHub repo मध्ये `.well-known/assetlinks.json` म्हणून ठेवा (नाहीतर app मध्ये वर address bar दिसते).

## 3. Play Console
1. play.google.com/console > developer account बनवा, एकदाची फी (सुमारे $25), ओळख पडताळणी.
2. Create app > Game > Free.
3. Store listing: listing.txt मधील मजकूर वापरा. Icon 512x512: icons/icon-512.png.
   Feature graphic (1024x500) आणि कमीत कमी 2 screenshots तुम्हाला स्वतः काढावे लागतील (फोनवर गेम खेळताना screenshot).
4. App content: Privacy policy लिंक, Ads = No, Target audience = 13+ (किंवा सर्वांसाठी), Data safety = "No data collected", Content rating प्रश्नावली (हिंसा नाही).
5. Testing > Closed testing > नवीन release > `.aab` upload.
   नवीन personal account असेल तर 12 testers (Gmail ids) जोडा, त्यांनी opt-in करून 14 दिवस अॅप ठेवला पाहिजे.
6. 14 दिवसांनंतर Dashboard > "Apply for production" > प्रश्नांची उत्तरे > Google review.
