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

grep : komutu çıktısını alabildiğin bir komutun içinden belli bir kelime veya cümlenin olduğu satırları almaya/işlemeye yarar.

* -v : Belirlenen kelimeyi içeren satırları almamaya yarar
* -E : Birden çok kelime kullanmaya yarar
* -i : Büyük küçük harf kuralını es geçer
* -ne : Satır numaralarını gösterir
* -A(SAYI) : Belirlenen kelimenin altından SAYI kadar satır alır (After)
* -B(SAYI) : Belirlenen kelimenin üstünden SAYI kadar satır alır (Before) 

cut: komutu, herhangi bir komutun çıktısındaki değeri kırpmaya yarar. "|" ile birlikte kullanılabilir.

* -d : Ayraç olarak hangi karakterin kullanacağını belirler.
* -f : Ayracın başından başlayarak seçim yapmaya yarar. En sona "-" eklerseniz satırın sonuna kadar alır.

tr : komutu yine aynı grep, awk, sed gibi bir çıktı ve dosya işleme aracıdır. Özel olarak isteğe göre seçilen biçimleri işleme özelliği vardır.

* -d : Belirli biçim veya karakter ile eşleşen karakterleri siler.
* -c : Belirli biçim veya karakter ile eşleşmeyen karakterler üzerinde işlem yapar.
* -s : Belirli biçim veya karakter birden fazla tekrar ediyorsa tekrar sayısını 1'e düşürür. Kendisine ikinci bir parametre verilirse, belirli karakter yerine belirtilen karakteri yerleştirir. 

sed : komutu, belirli çıktılarda herhangi bir kelimeyi veya cümleyi düzeltmeye yarayan komuttur.

-i : Bu parametreyi dosya seçerek kullandığınızda dosyada düzenleme yapar. "|" işleci ile kullandığınızda herhangi bir değişiklik yapmaz. Değişiklik sadece çıktıya yansır.
/ : sed komutunda ayıraç olarak kullanılır, dilerseniz _ gibi farklı karakterleri kullanabilirsiniz.
g,1,2 : g ile tüm değerleri, sayılar ile baştan bir kaç değeri değiştirebilirsiniz.
; : Bu işareti sed içerisinde kullanmak, alt satıra geçmek ile eşdeğerdir

awk kullanımı cok genıstır ondan dolayı https://ceaksan.com/tr/awk-komutu boyle bır kaynak bırakıyorum
