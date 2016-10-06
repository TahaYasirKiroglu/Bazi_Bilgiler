#Virtualbox için Ekran Çözünürlüğü Sorunu#

Eğerki kullandığınız sistemle beraber ubuntuyu **kurmak istemiyor** veya **kuramıyorsanız** fakat yinede ubuntuyu kullanmak
istiyorsanız sizin için en iyi seçenek sanal makina kullanmaktır.

Sanal makina kullanan kişiler, ubuntuyu normal kullanan kişilere göre bir çok problem yaşamaktadır. Bu sorunların başında **çalışma
performansı** ve ekran çözünürlüğü gelir. Her ne kadar performans sorunu çözülemesede ekran çözünürlüğü bir nebzede olsa
çözülebilmektedir. Bu bölümde virtualbox için ekran çözünürlüğü sorununu düzeltme üzerine bilgi verilecektir.


> Eğer ki ubuntunun son güncellemelerini aldığınıza emin değilseniz aşağıdaki komutları çalıştırmanız gerekmektedir. Aşağıdaki
> komutlar, komut satırına yönetici yetkisi vererek sisteminizi güncellemeye yarar.

~~~
  sudo apt-get update
  sudo apt-get upgrade
~~~

Yukarıdaki kodları çalıştırdıktan sonra aşağıdaki komutları çalıştırarak ekran çözünürlüğünü normale alabiliyoruz.

~~~
  sudo apt-get install dkms
~~~
  veya
~~~  
  sudo apt-get install virtualbox-guest-dkms
~~~

Bu kodları çalıştırdıktan sonra sanal makinayı yeniden başlatıyoruz. Sanal makina açıldığı zaman kullanıma hazır olacaktır.

> Daha detaylı bilgi için:
[Virtualbox Guestaddition](https://www.virtualbox.org/manual/ch04.html#idp46691715827040) bölümünü inceleyiniz.
