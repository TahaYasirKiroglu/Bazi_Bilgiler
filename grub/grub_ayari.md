
~~~bash
 sudo gedit /etc/default/grub
~~~

yapılan ayar değişikliğinden sonra

~~~bash
sudo update-grub
~~~

Aynı zamanda grub-customizer adında grafik arayüze sahip bir programla da ayarlarınızı yapabilirsiniz.

~~~bash
# repoyu ekliyoruz. Bunun için onay vermek gerekiyo
sudo add-apt-repository ppa:danielrichter2007/grub-customizer
sudo apt-get update
sudo apt-get install grub-customizer
~~~
