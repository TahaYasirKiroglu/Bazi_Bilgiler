# PDF Slice

Ubuntu'da pdf bölümlemek için `pdftk` adında bir paketten yararlanıyoruz.

~~~bash
sudo apt-get install pdftk
~~~
diyerek programı kuruyoruz. Onay isterse onay veriyoruz. 70MB civarında bir
boyutu var.

Programı kurduktan sonra bölmek istediğimiz yeri şu şekilde belirtiyoruz:

Diyelimki elimizde `full-pdf.pdf` adında bir dosyamız var. Biz bu dosyanın
12 ile 15. sayfaları arasını bölmek istiyoruz. Ve bu böldüğümüz sayfaları içeren
 pdf'in adınında `12-15arasi.pdf` olmasını istiyoruz.
Terminalde `full-pdf.pdf` 'in konuma geldikten sonra şu komutla bölümlemeyi
yapabiliyoruz:

~~~bash
pdftk full-pdf.pdf cat 12-15 output 12-15arasi.pdf
~~~
