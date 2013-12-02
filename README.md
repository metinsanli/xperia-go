xperia-go
=========
Sony Xperia Go ST27i / Android 4.1.2 / 6.2.A.1.100 hakkında genel bilgi ihtiva eder.
## Neler yapılabilir.
* [Android 4.1.2 - 6.2.A.1.100 yazılımına sahip telefon nasıl root yapılır.](https://github.com/metinsanli/xperia-go/tree/master/root-yap)
* [/system/app/ klasörü altındaki uygulamaların açıklamaları](https://github.com/metinsanli/xperia-go/tree/master/apk-bilgileri)
* [Ana bellek bölümleri ve "fstab" bilgileri, "mount" parametreleri](https://github.com/metinsanli/xperia-go/tree/master/dosya-sistemi)
* [Bilinmesi Gerekenler](https://github.com/metinsanli)

## Sony Xperia Go ST27i Özellikleri
* ST-Ericsson NovaThor U8500 1GHz ARMv7 32-bit İşlemci
* 512MByte DDR2 RAM Bellek
* 7.5 GByte Dahili Hafıza (3.7 GByte'lık kısmı kullanıcıya ayrılmış)
* 3.5" 480X320 LCD Ekran
* 5 Mega Pixel Kamera
* GSM850, GSM900, GSM1800, GSM1900, UMTS900 (B8), UMTS2100 (B1)
* GPRS, EDGE, UMTS, HSDPA, HSUPA
* 802.11b, 802.11g, 802.11n, Bluetooth 3.0, USB 2.0, GPS, FM Radio, Micro SD
<img src="http://www-static.se-mc.com/blogs.dir/0/files/2012/05/xperia-go-message-life-gone-documentary.png">


## Lisans

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Bilinmesi Gerekenler

The build requires [Maven](http://maven.apache.org/download.html)
v3.1.1+ and the [Android SDK](http://developer.android.com/sdk/index.html)
to be installed in your development environment. In addition you'll need to set
the `ANDROID_HOME` environment variable to the location of your SDK:

```bash
export ANDROID_HOME=/opt/tools/android-sdk
```

After satisfying those requirements, the build is pretty simple:

* Run `mvn clean package` from the `app` directory to build the APK only
* Run `mvn clean install` from the root directory to build the app and also run
  the integration tests, this requires a connected Android device or running
  emulator

You might find that your device doesn't let you install your build if you
already have the version from the Android Market installed.  This is standard
Android security as it it won't let you directly replace an app that's been
signed with a different key.  Manually uninstall GitHub from your device and
you will then be able to install your own built version.

See [here](https://github.com/github/android/wiki/Building-From-Eclipse) for
instructions on building from [Eclipse](http://eclipse.org).

