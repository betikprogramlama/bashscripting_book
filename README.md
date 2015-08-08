# bashscripting_book

1) Sistem Healty Checker
Sistem raporu üretip günlük mail atan, acil durumları bildiren script.

2) Network Checker
network cihazlarını kontrol eden rapor üreten script.

3) Disk Crypto
diskinizi önceden seçtiğiniz algoritmayla şifreleyen çözen script.

4) Remover - remo
Sistemden silemediğiniz klasör veya too long hatası aldığınız uygulamaları da silen sistem komutunun yazımı.

5) Twit-follower
Belirlediğiniz kullanıcı belirlediğiniz sözcüğü kullanınca size haber veren script.

- Verilen ip adres araligindaki makinalari up/down durumuna gore raporlayan multithread olarak calisan bir betik. Ayni zamanda verilen ip adres araligi icin port taramasida gerceklestirecektir. Ornek calisma opsiyonlari ise asagidaki gibi olacaktir.

 ###### ./betik -s 192.168.1.0/24 - durum taramasi
 ###### ./betik -p 80,443 192.168.1.0/24 -a - port taramasi

- Yapilandirma dosyasi icerisinde ip adres araligi, kullanici/parola bilgisi ve aranacak kelime obeklerini alarak paylasim icerisinde arayip raporlayan betik. Kisaca https://github.com/galkan/depdep yakin bir is yapacak.

###### cat config.cfg

username="user"
password="password"

keywords="password, credit card"

###### ./betik -f config.cfg 192.168.1.0/24


