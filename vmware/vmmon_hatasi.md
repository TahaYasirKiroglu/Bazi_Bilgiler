Vmware workstation 14 kullanırkan şu hatayı aldım:

> Could not open /dev/vmmon: No such file or directory.
Please make sure that the kernel module `vmmon' is loaded.
Failed to initialize monitor device.

Hatayı çözmek için modülleri yeniden yüklemek ve bazı modül ayarlarında değikliklere gitmek gerekiyordu. Uzunca süreçlerin ardından, vmware'in hali hazırda kernel değişiklikleri sırasında silinen paketler için bir komutu olduğunu fark ettim.

> sudo vmware-modconfig --console --install-all 

Aldığım hatanın sebebi kernel ayarlarında yaptığım bir kaç değiklikti. UEFI veya EFI ile ilgili hataları çözmeyebilir.
