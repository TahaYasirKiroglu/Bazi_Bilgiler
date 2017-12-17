## ubuntu bats sorun çözümü

bats, ubuntuda kullanılırken bazı hatalar veriyor. 
Yaptığım incelemeler sonucunda /usr/lib/bats/bats-exec-test içerisindeki
`trap` built fonksiyonunun yanlış parametrelerle çalıştırıldığını gördüm ve parametreleri büyük harflerle
yamak gerektiğini düşündüm ve bunu gerçekleştirdiğimde çalıştığını gördüm.

Bendeki bats programı 0.4.0 srümünde. Düzeltilmiş kodlar bats-exec-test şeklinde veriliştir.
