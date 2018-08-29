# [steemwallet.app](https://steemwallet.app)
##### [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

[![steemwallet.app](https://steemwallet.app/images/social_fb.jpg)](https://steemwallet.app)

##### steemwallet is a fast, secure and open source wallet for the Steem blockchain, available for iOS and Android.

# Key features
  - Monitor any / multiple account's balances from the Steem blockchain
  - Create, sign and broadcast transfer transactions (send steem & sbd) (optional)
  - AES 256 encrypted storage for keys should you want to sign transfer operations (send steem & sbd)
  - QR code reader for easy importing of keys and sending to others
  - QR code generator for easy proposing your wallet address for others to send to
  - Optional use of Touch ID / Face ID for retrieving your passphrase
  - Forced creation of a difficult passphrase including cracktime hints, should you want to use the AES 256 encrypted storage.

# Build instructions
  - Download & install Appcelerator CLI (you need nodejs for that): https://wiki.appcelerator.org/display/guides2/Appcelerator+CLI+Getting+Started
  - Have the sdk's for Android and/or IOS on your device
  - Git clone this repo
  - `appc run -p (ios|android)`


# This app uses the following libraries / software
  - Build on [Axway Titanium Appcelerator](https://github.com/appcelerator/titanium_mobile) for crossplatform native compiled apps
  - Dsteem for steem key related functions: https://github.com/steemit/dsteem
  - Node buffer implementation, used for head-block prefix calcs: https://github.com/feross/buffer
  - Client side qr code generator: https://github.com/siciarek/javascript-qrcode
  - For time manipulations: https://github.com/moment/moment
  - AES encryption for wallet encryption: https://github.com/benbahrenburg/Ti.SlowAES
  - ZXCVBN password strength checker library: https://github.com/dropbox/zxcvbn
  - Identity module for integration with biometry: https://github.com/appcelerator-modules/titanium-identity/
  - Steem's Bad Actors List from: https://github.com/steemit/condenser/blob/master/src/app/utils/BadActorList.js
  - Detecting crossplatform resume / pause of app: https://github.com/dieskim/Appcelerator.Hyperloop.appPauseResume
  - QR code scanner from: https://github.com/appcelerator-modules/ti.barcode

### Feature requests, pull-requests

I specifically envision keeping the app lightweight. I certainly don't intend to compete with other great apps out there such as the eSteem app or for example Steepshot.

If you want to help, and want the app in your native language, feel free to help translate!
please explore the app thoroughly and check the [app/i18n/en/strings.xml](app/i18n/en/strings.xml) translation file, make a copy and translate all the texts. Whenever the %1$s or %2$s (etc etc) is used in that file it is the place of a variable, which should be quite obvious. (E.g. strings like: *Can't find account "%1$s"* - would obviously have the account name filled in at %1$s)  

#### Translations already done

| language 	| github user 	| steem user                                    	|
|----------	|-------------	|-----------------------------------------------	|
| DE       	| @pharesim   	| [pharesim](https://steemit.com/@pharesim)     	|
| ES       	| @tashidelek 	| [tashidelek](https://steemit.com/@tashidelek) 	|
| FR       	| @helo     	  | [helo](https://steemit.com/@helo)             	|

Cheers, [@roelandp](https://steemit.com/@roelandp)
