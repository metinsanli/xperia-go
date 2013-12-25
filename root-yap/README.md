#### Android 4.1.2'de nasıl root yapılır?

* İlk önce gereken dosyalar cihaza gönderilir.

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
