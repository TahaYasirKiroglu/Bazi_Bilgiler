# DPKG Silinmiş Paketlerin Yapılandırma(Config) Dosyaları

Silinmiş paketlerin yapılandırma dosyaları, programı silmemize
rağmen kalabilir ve bazı durumlarda kişisel güvenliğimizi tehlikeye atabilmektedir.
bu durumu engellemek için yapılandırma dosyalardan işimize yarayanları yedeklememiz,
işimize yaramayacak olanı da silmemiz gerekmektedir.

> Not: *apt-get remove* veya *apt remove* ile yapılan silinmelerde yapılandırma 
dosyaları kalmaktadır. Fakat *apt-get purge* veya *apt purge* ile yapılan silmelerde
yapılandırma dosyaları da silinmektedir.

Öncelikle işe yaramayan yapılandırma dosyalarını bulmamız gerekir. Bunun için

~~~bash
  dpkg --list | grep "^rc"
~~~

komutunu çalıştırabiliriz. Bu kopumutu çalıştırdığımızda bütün paket bilgilerimiz 
gösterilecektir. Daha sonra grep ile *r* ile kaldırılmış (removed), *c* ile 
yapılandırma (config) dosyası bulunan dosyalar gösterilecektir. Gelgelelim 
bu dosyaları tek tek elle mi kaldıracağız kısmına.

Yaptığım sorgudan 750 paket adı geldi. kimisi beta sürümü, kimisi de değişik 
programlardan oluşan bir sürü çöp bilgi... Açıkcası elle silecek kadar boşa
harcayacak zamanım olmadığı ve önemli yapılandırma dosyalarımı yedeklediğim için
şöyle basit bir betikle zaten elimizde olan dosyaların isimlerini
*apt purge*'e göndererek silmesini sağlayabiliyoruz.

~~~bash
  sudo apt purge `dpkg --list | grep "^rc" | awk '{ print $2; }'`
~~~
