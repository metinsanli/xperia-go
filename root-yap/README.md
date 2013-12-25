#### Android 4.1.2'de nasıl root yapılır? (Windows için)

* Gereken dosyaları içeren [meTooR.zip](https://github.com/metinsanli/xperia-go/raw/master/root-yap/meTooR.zip) indirlip klasörüyle çıkartılır.

* Komut Satırı (cmd) meTooR klasöründe açılır.

* Gereken dosyalar cihaza gönderilir.

**adb push doomed2 /data/local/tmp/.**

**adb push run_root_shell /data/local/tmp/.**

**adb push busybox /data/local/tmp/.**

**adb push su /data/local/tmp/.**


* Gönderilen dosyalara tam erişim yetkisi verilir.

**adb shell chmod 777 /data/local/tmp/doomed2**

**adb shell chmod 777 /data/local/tmp/busybox**

**adb shell chmod 777 /data/local/tmp/run_root_shell**


* Betik çalıştırılır.

**adb shell /data/local/tmp/run_root_shell**

* Tamamdır. İsteğe bağlı; Google Play Marketten ücretsiz [Superuser](https://play.google.com/store/apps/details?id=com.koushikdutta.superuser) uygulaması yüklenerek uygulamalar için root yetkisi kontrollü olarak verilebilir.
