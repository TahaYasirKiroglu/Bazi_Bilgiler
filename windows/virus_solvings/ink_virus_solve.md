#### Ink Virüsü

Dönem dönem bilgisayarlarda yayılan ve bilgisayarı mahveden kısayol uzantılı virüsleri bilmeyeniniz yoktur. 
Burda virüs bilgisayara yayılmadan önce engelleme yolu anlatılacaktır.


      del *.Ink
      attrib -h -r -s /s /d *.

bir text belgesi oluşturup yukarıdaki kodları içine atın.
Daha sonra dosya uzantısını .bat olarak değiştirin.
Dosyayı flaşın içine atın ve çalıştırın.
 Dosyanın içerisinde dosyalarınız isimsiz bir klasörün içerisinde bulunacaktır.
 Son olarak isimsiz klasörün içerisindeki virüs dosyalarını silerek dosyalarınız kurtarabilirsiniz.

Ayrıca doğrudan cmd üzerinden de bu işlem geçekleştirilebilir.

Diyelimki flash belleğiniz F:\ sürücüsünde

      F:
      del *.Ink
      attrib -h -r -s /s /d *.
      
Daha sonra arayüz üzerinden boş isimli klasörün içindekii virüs dosyaları silinerek virüsün yayılması engellenir.
