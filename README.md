# DiziPal Erişim Tarayıcısı

**Sürüm:** 1.0  
**Geliştirici:** [Uğur ARIKAN]  
**Platform:** Windows  
**Gereksinimler:** Yok (Python kurulumu gerektirmez)

## Yazılımın Amacı

Bu yazılım, belirli aralıklardaki DiziPal adreslerini kontrol ederek güncel ve çalışan bir URL bulmanıza yardımcı olur. DiziPal, zaman zaman alan adı değişiklikleri yaptığı için erişimi zorlaşmaktadır. Yazılımımız, belirlediğiniz aralıkta mevcut URL’leri tarayarak erişilebilir olanları otomatik olarak tespit eder, çalışan adresi ekranınıza getirir ve tarayıcınızda otomatik olarak açar.

## Özellikler

- **Otomatik URL Denetimi**: Belirlenen URL aralığındaki adresleri tek tek test ederek çalışan adresi bulur.
- **Aralık Güncellemesi**: Çalışan bir adres bulduğunda, bir sonraki kullanımda taramaya devam edilecek aralığı otomatik olarak günceller.
- **Kolay Kullanım**: Yazılımı başlatmak için sadece `.exe` dosyasını çift tıklamanız yeterli.
- **Renkli Çıktı**: Çalışan ve çalışmayan adresler renkli olarak gösterilir (Yeşil: Çalışıyor, Kırmızı: Çalışmıyor).

## Kullanım Talimatları

1. **Yazılımı Başlatma**:
   - `DiziPal_Erisim_Tarayicisi.exe` dosyasını çift tıklayarak çalıştırın.
   
2. **URL Tarama**:
   - Program, önceden belirlenen `config.txt` dosyasındaki aralıktan başlayarak URL'leri kontrol edecektir.
   - Çalışır durumda bir adres bulunursa bu adres ekranda yeşil renkte görünecek ve tarayıcınızda açılacaktır.

3. **Başlangıç ve Bitiş Aralığını Ayarlama**:
   - Program, en son taranan aralığı `config.txt` dosyasına kaydeder. Son geçerli adres bulunduğunda, bir sonraki çalıştırmada buradan devam edilir.
   - Başlangıç aralığını sıfırlamak veya farklı bir aralıkta arama yapmak için `config.txt` dosyasını açın ve yeni aralıkları girin (örneğin, `800,820`).

## Dosyalar

- **DiziPal_Erisim_Tarayicisi.exe**: Yazılımın çalıştırılabilir dosyası.
- **config.txt**: Programın başlangıç ve bitiş aralığını kaydettiği dosya. Gerektiğinde bu dosyadaki değerleri güncelleyebilirsiniz.

## Sık Sorulan Sorular

1. **Yazılımı çalıştırdığımda tarayıcıda açılan URL yanlış gözüküyor, ww1 ile başlıyor.**
   - Program, `www` ile başlayan adresleri arar. Eğer farklı bir sunucuya yönlendirme yapılırsa, doğru adrese bağlanmak için DiziPal’in güncel URL’sini belirlediğiniz aralıkla güncelleyin ve yeniden tarama yapın.

2. **Taramada herhangi bir sonuç bulamıyor, ne yapmalıyım?**
   - `config.txt` dosyasındaki aralığı genişletin ve tekrar çalıştırın. Örneğin, `800, 850` olarak güncelleyebilirsiniz.

3. **Programı tekrar çalıştırdığımda daha önce bulunduğum yerden devam eder mi?**
   - Evet, program son başarılı URL aralığını `config.txt` dosyasına kaydeder ve sonraki çalıştırmalarda buradan devam eder.

## Notlar ve Destek

Bu yazılım DiziPal gibi erişimi değişken olan sitelere ulaşımı kolaylaştırmak amacıyla geliştirilmiştir. Destek ve güncellemeler için [ugurarkn@gmail.com].
