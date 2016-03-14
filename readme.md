# BitShares Wallet
<img src="http://i.imgur.com/9RtNJuy.png" width="200" align="right">
BitShares Wallet a beautiful, simple, minimalist UI/UX to the BitShares 2.0 blockchain. This v1.0 will allow the user to send and receive Bitshares and Smartcoins (BTS, bitEUR, bitUSD, BTSATM, etc) with their Android, iPhone or Windows mobile device in portrait or landscape modes. 

[The app on Google Play Market](https://play.google.com/store/apps/details?id=de.bitsharesmunich.wallet "")

Send any amount.. anywhere.. for just a few cents.. and in only 3 seconds!
 
* Works with all Smartcoin enabled Point Of Sale (POS) systems at merchants worldwide 
* Absolute Security; BitShares blockchain based, End-to-End Encryption, BrainKey, multi-signature account permissions, auto-encrypted Backups, auto-close, auto-timeout and PIN verifications
* No Bluetooth, NFC, merchant wireless service or special hardware is required 
* Use QR Codes to Send locally (uses your phone’s camera to scan their QR Code)
* Use QR Codes to Receive locally (displays your QR Code so your friend can scan it) 
* Receive eReceipts automatically via merchant QR codes
* 10,000+ transactions per second (TPS) which is more than Visa and Mastercard combined! 
* Send and Receive Smartcoins (bitUSD, bitEUR, bitCNY, bitBTC, bitSILVER, etc)
* Send and Receive User Issued Assets (UIAs) - (OPENPOS, OBITS, OPENBTC, COFFEE, etc) 
* Supports a large Memo field with sending payments (for personal notes or notes to the recipient)
* Share the BitShares Wallet app with friends and get reward$
* Choose friendly account names; No more long cryptic addresses or numbers
* Totally Open-Source Software (OSS) and verifiable on Github
* Contacts can be organized by BitShares account address or nickname label. Notes and Avatars are supported too!
* Quickly and Easily share your payment address via email, chat, wireless, social media and telephone
* Monitor all Balances and Transactions in real-time; UI/UX never needs a refresh
* Now in 22 languages! 


## Building
### Prerequisites
1. Go to project root directory 
2. `cd dev`
3. `unpack node_modules_bsw.zip`, so that node_modules directory appears in `dev` directory 
4. `cd app/dl/`
5. `npm install`
6. `cd ../../..` 
7. `npm install cordova -g`
8. Install Android SDK
9. `cordova platform add android`

### Web build
1. Go to project root directory 
2. `cd dev`
3. `npm run build`
4. `set port = 5000` (optional) 
5. `http-server` 
6. Remove cookies, localstorage and web databases for localhost to clear applicaton settings (optional) 
7. Open [localhost:5000](http://localhost:5000)

### Android build
1. Go to project root directory
2. `cd dev`
3. `npm run buildprod`
4. `cd ..`
5. If any changes of external resources (css, images etc) occured since last build, manually copy these folders from `dev\app\assets\` to `www\assets` 
6. `cordova build android --debug`
7. Resulting .apk file is in `platforms\android\build\outputs\apk`
