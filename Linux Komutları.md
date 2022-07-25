Linux Komutları

ls : komutu bulunduğunuz dizindeki dosyaları görmenizi sağlar.
* -l : Klasörleri liste biçiminde ayrıntıları ile birlikte gösterir.
* -s : Dosyaların boyutunu bayt cinsinden gösterir.
* -a : Gizli olan tüm dosya ve klasörleri gösterir

clear : komutu ekrandaki yazıları siler.


cd : komutu bulunduğunuz dizinden başka bir dizine geçmeye yarar
NOT: Eğer üst dizine çıkmak istiyorsanız cd ..


mkdir : komutu klasör oluşturmaya yarar.


touch : komutu, dizin belirtmediğiniz sürece bulunduğunuz dizinde dosya oluşturmaya yarar.


ln : komutu, bir dosyayı veya bir klasörü başka bir yere linklemeye/kısayol oluşturmaya yarar. Parametre verilmediğinde hard-link yapılır (Not: klasörler hard-link yapılamaz)
* -s : Sembolik olarak linkler. Genelde kullanılan parametre budur.
* -f : Linklemeye zorlar (force).



readlink : komutu, linklenmiş dosyaların tam konumunu ve nasıl linklendiğini gösterir.
* Not: hardlink ile linklenmiş dosyaları göstermez.



cat, more ve less : komutları genelde kendisine verilen dosyaların içeriğini okumaya yarar.



echo : komutu, kendisine yazdığınız şeyin ekrana basılmasını sağlar.
* -e : Kaçış dizilerini aktifleştirir.



cp : komutu dosya kopyalamaya yarar. Genelde birlikte kullanılan argümanlar:
* -r : Klasör kopyalar.
* -f : Kopyalamaya zorlar.
* -v : Bir klasör kopyalanırken hangi dosyaların kopyalandığının çıktısını verir.
* -i : üstüne yazmadan önce sorar.



rm : komutu verdiğiniz adresteki dosyayı silmeye yarar. Genelde birlikte kullanılan argümanlar:
* -r : Klasör siler.
* -f : Silmeye zorlar.
* -v : Birden fazla dosya silerken her dosya sildikten sonra şu dosyayı sildim diye bilgi verir.
* -i : Her silme işleminden önce silmeye emin misiniz diye sorar.



vim : bir metin düzenleyicidir 

kaydetmek ve çıkmak için tuş kombinasyonları vardır. (:q = Çıkış | :wq = Kaydederek çıkış | :q! = Kaydetmeden çıkış)



chmod : komutu dosyaların yetkilerini ayarlamaya yarar.
* +x : Dosyayı çalıştırılabilme iznini verir.
* -x : Dosyadan çalıştırılabilme iznini kaldırır. NOT: chmod'un nasıl kullanıldığı ile ilgili daha fazla bilgiye google'a chmod cheat sheet yazarak ulaşabilirsiniz.



awk kullanımı cok genıstır ondan dolayı https://ceaksan.com/tr/awk-komutu boyle bır kaynak bırakıyorum
