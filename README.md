**Çalışma Konusu:**
**WhatsApp Cloud API ile Mesaj Teslimat Takibi ve Analizi**
**Amaç:**
Webhook event’lerini kullanarak gönderilen mesajların teslimat ve okuma durumlarını takip eden, MongoDB üzerinde verileri analiz eden ve basit bir gösterim sunan bir sistem geliştirmeni istiyorum. Hem API’yi daha iyi tanımış olacaksın, hem de gerçek projeye katkı sağlayabilecek parçalar üreteceksin.
---
**1. Gün – API İncelemesi ve Planlama**

* WhatsApp Cloud API dökümantasyonuna göz at.
* `message status` event’lerini detaylı incele: `sent`, `delivered`, `read`, `failed`.
* Webhook mantığını, event’lerin ne zaman ve nasıl geldiğini anlamaya çalış.

**2. Gün – Webhook Listener ve Veri Kaydı**

* Basit bir Node.js tabanlı webhook listener oluştur.
* Gelen event’leri MongoDB’ye loglayan bir yapı kur.
* Event payload’larını düzgün ve anlamlı bir şekilde sakla.

**3. Gün – Analiz Fonksiyonları**

* Kullanıcı bazlı mesaj analizi yapan bir MongoDB query’si yaz.
* Son 100 mesaj için: kaç tanesi iletilmiş, kaç tanesi okunmamış vs.
* Oranları basit bir JSON çıktısı ile döndür.

**4. Gün – Görselleştirme ve Gösterim**

* Basit bir dashboard ya da API response ile analiz sonuçlarını sun.
* Her kullanıcı için okuma / teslim oranlarını göster.
* İsteğe bağlı: tarih filtresi, kullanıcı filtresi ekle.

**5. Gün – İleri Düzey Filtreleme ve Raporlama**

* 24 saat içinde iletilemeyen mesajları listeleyen bir endpoint yaz.
* Aynı kullanıcıya başarısız gönderimlerin raporunu çıkar.
* Opsiyonel: Tekrar gönderim için öneri listesi oluştur.

**6. Gün – Temizlik ve Dokümantasyon**

* Kodlarını temizle, yorum satırları ekle.
* Projenin nasıl çalıştığını anlatan kısa bir README yaz.

**7. Gün – Sunum ve Değerlendirme**

* Yaptığın işi kısa bir sunumla anlat.
* Sistem nasıl çalışıyor, neler öğrendin, hangi zorluklarla karşılaştın?
* Ekstra fikirlerin veya önerilerin varsa belirt.
