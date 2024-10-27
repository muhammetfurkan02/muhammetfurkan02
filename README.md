Ubuntu Sistem Gereksinimleri ve Kurulum Rehberi
Ubuntu’yu kurmadan önce dikkat etmeniz gereken bazı önemli noktalar vardır:

Depolama Alanı: Cihazınızda en az 25 GB boş alan bulundurmanız önerilir. Ancak minimal bir kurulum yapmak istiyorsanız, 5 GB yeterli olacaktır.
Harici Depolama: Kurmak istediğiniz Ubuntu sürümünü içeren bir harici depolama (Flash bellek, SSD, HDD) gereklidir.
Veri Yedekleme: Olası bir aksilik durumuna karşı verilerinizin yedeğini almayı unutmayın.
Minimal Sistem Gereksinimleri:
2 GHz çift çekirdekli işlemci
4 GiB RAM (sistem belleği)
50 GB sabit disk alanı (minimal kurulum için 8.6 GB yeterlidir)
İnternet erişimi
Kurulum Hazırlıkları
Sistemi kurmadan önce gerekli tüm hazırlıkları yaptığınızdan emin olun. Ardından Ubuntu’nun resmi web sitesine giderek yükleme işlemine başlayabilirsiniz: Ubuntu İndirme Sayfası (Benim indirdiğim sürüm Ubuntu 24.04.1).
![image](https://github.com/user-attachments/assets/25bb1670-4deb-4db6-89fe-1fa03f5dace9)

1. Görüntüyü İndirme
Ubuntu web sitesini açın ve masaüstü sürüm görüntüsünü indirin.

2. USB’ye Görüntüyü Yazma
Görüntüyü indirdikten sonra, bu dosyayı bir harici depolama birimine (örneğin, USB) yazmanız gerekecek. Windows üzerinde bunu yapmak için Rufus gibi bir yardımcı program kullanabilirsiniz.

3. BIOS Ayarları
Eğer bilgisayarınız USB belleği doğrudan başlatmıyorsa, BIOS ekranına girmeniz gerekecek. Bilgisayarınızı kapatın ve tekrar açarken BIOS’a girmek için genellikle F12, F2, F10 veya Escape tuşlarına basın. BIOS ekranında, önyükleme aygıtı önceliğini USB sürücünüzü birinci sıraya yerleştirerek ayarlayın. Ardından ayarları kaydedip çıkın.
![image](https://github.com/user-attachments/assets/98fa7d74-a2f1-4efe-8d01-4c0a3e79bc22)

Ubuntu 24.04.1’i Yükleme
BIOS ayarlarını yaptıktan sonra bilgisayarınızı yeniden başlatın. Bu sefer USB bellekten başlayacak ve işletim sistemini kurmaya başlayacaksınız.
![image](https://github.com/user-attachments/assets/206f17ec-4cb2-4428-85d4-bedfbd3a8a6c)

1. Dil Seçimi
Bilgisayarınızı yeniden başlattığınızda, dil seçim ekranıyla karşılaşacaksınız. İsterseniz bu ekranı atlayabilir veya istediğiniz dili seçebilirsiniz.
![image](https://github.com/user-attachments/assets/f6f68f44-6722-447a-9924-e629865bd910)

2. Sistem Yükleyicisini Başlatma
Açılan ekranda "Ubuntu’yu Yükle" seçeneğini seçin. Yükleyici başlayacaktır.

3. Klavye Düzeni
Kurulum sırasında klavye düzenini değiştirmek isterseniz, bunu Alt+Shift veya Win+Space ile yapabilirsiniz. Varsayılan olarak İngilizce gösterilecektir, ancak farklı bir düzen seçebilirsiniz.
![image](https://github.com/user-attachments/assets/3d5e7c99-908a-4de1-9fee-79f1c0cde937)

4. Yazılım Seçenekleri
Başlangıçta hangi uygulamaları yüklemek istediğinizi belirleyeceksiniz. İki seçenek var:

Normal Kurulum: Varsayılan yardımcı programlar, uygulamalar ve oyunlar ile birlikte gelir.
Minimal Kurulum: Daha az depolama alanı kaplar ve yalnızca ihtiyaç duyduğunuz bileşenleri yükler.
Kurulum sırasında güncellemeleri indirip üçüncü taraf yazılımları yüklemek için gerekli kutucukları işaretleyin. İnternete bağlı olmanız önerilir, böylece en son güncellemeleri alabilirsiniz.
![image](https://github.com/user-attachments/assets/e3fcf054-19a0-4a30-a2f2-53bf9aad3eb1)

5. Disk Bölümlendirmesi
Ubuntu’yu başka bir işletim sistemiyle birlikte mi yoksa mevcut işletim sisteminizi silip onun yerine mi kurmak istediğinizi seçin. Windows kuruluysa, yükleyicinin otomatik olarak bölümlendirmeyi yapmasına izin verebilirsiniz.
![image](https://github.com/user-attachments/assets/f0eed3c1-3e42-435f-bc3b-3d4456f0f622)

6. Yeni Bölüm Oluşturma
Tüm boş alanı tek bir bölüm olarak seçebilir veya farklı bölümler oluşturabilirsiniz. Genellikle Linux’ta üç bölüm oluşturulması önerilir:

/boot: Önyükleyici için
/: İşletim sistemi için
/home: Kullanıcı dosyaları için
7. Önyükleyici ve Kök Bölümü Oluşturma
Önyükleyici için 300 MB'lık bir bölüm oluşturun ve dosya türünü Ext2 olarak ayarlayın. Kök bölümü için ise 50 GB veya daha fazla alan ayırarak dosya türünü Ext4 olarak seçin.
![image](https://github.com/user-attachments/assets/3a319185-0c76-4313-b8e3-858ae06d312b)

8. Kullanıcı Oluşturma
Adınızı girin ve bilgisayar adı ile kullanıcı adınızı belirleyin. Ardından güçlü bir şifre oluşturun.
![image](https://github.com/user-attachments/assets/706b099c-3360-419d-b198-4a8178250e77)

9. Kurulumun Tamamlanması
Kurulum aşamaları tamamlandığında, makineniz birkaç dakika içinde kurulumu gerçekleştirecektir. Kurulum tamamlandığında bilgisayarınızı yeniden başlatmanız istenecek. Harici disk veya USB belleği istediğiniz zaman çıkarabilirsiniz.
![image](https://github.com/user-attachments/assets/ae7ed6c3-d5df-4eee-bba4-32983fb29868)

Sonuç
Bir Linux işletim sistemi olan Ubuntu’yu başarıyla kurdunuz! Diğer Ubuntu sürümlerini de benzer adımlarla kurabilirsiniz. Ubuntu’nun keyfini çıkarın!

