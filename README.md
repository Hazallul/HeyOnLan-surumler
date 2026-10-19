# HeyOnLan

Evdeki bilgisayarını telefondan **açıp kapatan** ve uzaktan kumanda gibi yöneten Android uygulaması. Koltuktan kalkmadan bilgisayarı açarsın, açık unuttuysan yataktan kapatırsın, müziği durdurur, sesi kısar, fotoğrafı bilgisayara atarsın.

İki görünüm var, menüden istediğin zaman geçersin: **KATALOG** (kâğıt ve mürekkep, açık ya da koyu) ve **RUNNER** (siyah zemin, asit yeşili).

<p>
  <img src="ekran/runner-ana.png" width="260" alt="RUNNER teması: ana ekran">
  <img src="ekran/katalog-ana.png" width="260" alt="KATALOG teması: ana ekran">
  <img src="ekran/katalog-koyu.png" width="260" alt="KATALOG koyu">
</p>

## Neler yapıyor?

### Aç, kapat ve kumanda
- **Aç / kapat:** tek dokunuşla. Bilgisayarın gerçekten açık mı kapalı mı olduğunu ölçüp gösterir.
- **Güç:** yeniden başlat, uyku, istediğin süre sonra kapat, zamanlı kapatmayı iptal et.
- **Masaüstü:** kilitle, ekranı kapat, sessiz, **ses yüzdesi** (çubuğu parmağınla kaydır), **mikrofonu kapat / aç** (kapalıyken tuş belli olur), donan oyunu ya da programı **zorla kapat**.
- **Kısayollar:** dokununca bilgisayarda bir Steam oyunu, program ya da web sayfası açılır, ya da bir program kapanır. İstersen telefonun ana ekranına simge olarak eklersin.

### Bilgisayara dosya gönder
Galeride, Dosyalar'da ya da WhatsApp'ta **Paylaş**'a bas, listeden **Bilgisayara gönder**'i seç. Fotoğraf ve dosyalar bilgisayarın masaüstündeki **HeyOnLan-Depo** klasörüne düşer (klasör yoksa kendisi oluşturur). Birden fazla bilgisayarın varsa hangisine gideceğini sorar. Aynı adda dosya varsa üstüne yazmaz.

<p>
  <img src="ekran/paylas.png" width="300" alt="Bilgisayara gönder">
</p>

### Widget'lar
Dört widget var: **Tuş** (tek yuvarlak tuş), **Durum** (tuş, ad ve durum), **Hepsi** (bütün bilgisayarlar yan yana) ve **Kumanda**.

**Kumanda**'nın altındaki oka basınca widget'ın hemen altında seçtiğin işler açılır: uyku, kilitle, sessiz, oynat, mikrofon, kısayolların. Widget'ı basılı tutup büyütürsen aynı tuşlar widget'ın içinde görünür. Hangi işlerin çıkacağını uygulamada **Kısayollar** sayfasından seçersin.

<p>
  <img src="ekran/widget-listesi.png" width="330" alt="Widget listesi">
  <img src="ekran/kumanda.png" width="330" alt="Kumanda widget'ı açık">
</p>

### Panel
Telefonu yatay koyunca masada küçük bir bilgi ekranı olur: saat, çalan şarkı ve albüm kapağı, medya tuşları, işlemci, bellek, ekran kartı, sıcaklık, ağ hızı, Stream Deck gibi büyük kısayol tuşları. Düzeni parmağınla kurarsın; dört ayrı düzen arasında yana kaydırarak geçersin. Şarj olurken kendiliğinden açılabilir. Panel ya da uygulama açıkken bilgisayar çok ısınırsa telefona uyarı gelir.

<p>
  <img src="ekran/panel.png" width="100%" alt="Panel">
</p>
<p>
  <img src="ekran/panel-ayar.png" width="260" alt="Panel ayarları">
</p>

### Otomasyon
Kural: **ne zaman** ve sırayla **ne yapılacak**.
- **Saatte:** ör. hafta içi 08:30'da aç, sonra Discord'u başlat.
- **Eve gelince:** ev konumuna girip ev Wi-Fi'ına bağlanınca aç.
- **Evden çıkınca:** telefon ağdan çıkınca ve bilgisayara bir süre dokunulmayınca bilgisayar kendini uyutur ya da kapatır.
- **Şarja takınca:** ör. gece 23:00'ten sonra telefonu şarja takınca bilgisayarı kapat.

Adımların arasına bekleme koyabilirsin (ör. aç, 2 dakika bekle, oyunu başlat). Sonuç bildirimle gelir.

<p>
  <img src="ekran/otomasyon.png" width="260" alt="Otomasyon">
  <img src="ekran/kural.png" width="260" alt="Kural ekle">
</p>

### Diğerleri
- **Sesli komut:** menüden **Asistanla aç / kapat**'ı aç, sonra "Hey Google, HeyOnLan'ı aç" de. Bilgisayar kapalıysa açılır, açıksa 5 saniye geri sayıp kapanır.
- **Hızlı ayarlar kutucuğu:** bildirim panelinden tek dokunuşla aç / kapat.
- **Tasker, Home Assistant, MacroDroid:** menüden **Dış uygulamalar**'ı açınca bu uygulamalar bilgisayarı açıp uyutabilir ya da kapatabilir. Varsayılan kapalı.

<p>
  <img src="ekran/menu-tema.png" width="260" alt="Menü ve tema seçimi">
</p>

## Ne gerekiyor?

- Android 13 veya üstü bir telefon
- Windows 10 / 11 bilgisayar
- Telefon ve bilgisayar **aynı ev ağında** olmalı (misafir Wi-Fi olmaz)
- Kapalı bilgisayarı açmak için bilgisayar modeme **ethernet kablosuyla** bağlı olmalı. Wi-Fi ile bağlı bilgisayar tam kapalıyken açılamaz, uykudayken (ağ kartı destekliyorsa) açılır.

## Kurulum (5 dakika)

### 1. Telefona uygulamayı kur
1. Telefondan **[HeyOnLan.apk](https://github.com/Hazallul/HeyOnLan-surumler/releases/latest/download/HeyOnLan.apk)** dosyasını indir.
2. Dosyayı aç. "Bilinmeyen uygulamalar" uyarısı çıkarsa **Ayarlar → Bu kaynaktan izin ver** de, sonra **Yükle**.

> Play Protect "uygulamayı tanımıyor, taramaya gönder" derse **taramayı** seç; tarama bitince kurulum sürer. Google her yeni sürümü ilk kez gördüğü için bu uyarı güncellemelerde de çıkabilir, normaldir.

### 2. Bilgisayarı hazırla
1. Bilgisayardan **[HeyOnLan-Kurulum.bat](https://github.com/Hazallul/HeyOnLan-surumler/releases/latest/download/HeyOnLan-Kurulum.bat)** dosyasını indir.
2. Çift tıkla, izin sorarsa **Evet** de.
3. Pencerede bir **IP** (ör. 192.168.1.40) ve **6 haneli kod** çıkar. Pencereyi kapatma.

> Windows "bilgisayarınız korundu" derse **Ek bilgi → Yine de çalıştır**'a bas.

### 3. Eşleştir
Uygulamada **Kuruluma başla**'ya bas, IP'yi ve kodu gir, **Eşleştir**. Bu kadar.

### 4. BIOS ayarı (sadece açma için, bir kez)
Bilgisayar kapalıyken açılabilmesi için BIOS'ta **Wake on LAN** açık olmalı. Bilgisayarı açarken F2 ya da Del'e bas, "Wake on LAN", "Power On By PCI-E" ya da "Resume by LAN" benzeri ayarı **Enabled** yap. Anakarta göre adı değişir.

## Güncelleme

Yeni sürüm çıkınca uygulamanın menüsünde **YENİ SÜRÜM** yazar. **İndir**'e bas, açılan dosyayı kur. Eski uygulamanın üstüne kurulur; **silmen gerekmez, ayarların kalır.** Play Protect tarama önerirse yukarıdaki gibi taramayı seç.

Yeni özellikler bilgisayardaki kurulumun da güncel olmasını isteyebilir (uygulama "kurulum eski" der). O zaman **HeyOnLan-Kurulum.bat**'ı bilgisayarda bir kez daha çalıştırman yeterli; **yeniden eşleştirmen gerekmez.**

## Çalışmıyorsa

- **Açılmıyor:** ethernet kablosu takılı mı, BIOS'ta Wake on LAN açık mı? Telefon aynı Wi-Fi'da mı?
- **Kapanmıyor / komutlar gitmiyor:** uygulamada **Bağlantı → Test et**. Sorunu adım adım gösterir.
- **"Kurulum eski" diyor:** bat dosyasını bilgisayarda tekrar çalıştır.
- **IP değişti:** uygulama bilgisayarı ağda kendisi bulur; bulamazsa Bağlantı sayfasında test et.
- **Otomasyon geç çalışıyor:** Otomasyon sayfasındaki **Tam saat izni** ve **Pil kısıtlamasını kaldır** uyarılarına bak.

## Kurulum bilgisayarda ne yapıyor?

Bat dosyası düz metindir, Not Defteri ile açıp okuyabilirsin. Özetle:

- Windows'un kendi **OpenSSH Server**'ını açar (telefon komutları bununla gönderir).
- Bağlantıya **sadece ev ağından** izin verir, şifreyle girişi kapatır.
- Telefonun anahtarını, **sadece belirli komutları** (kapat, uyku, kilit, ses, kısayollar, dosya alma…) çalıştırabilecek şekilde ekler. Telefon bilgisayarında başka hiçbir şey yapamaz; gönderdiğin dosyalar sadece masaüstündeki **HeyOnLan-Depo** klasörüne yazılabilir.
- Wake on LAN için ağ kartı ve hızlı başlatma ayarlarını yapar.
- "Evden çıkınca" kuralı için, sen telefondan açmadıkça kapalı duran küçük bir zamanlanmış görev ekler.

---

Bu depoda sadece uygulamanın sürümleri (APK) ve bilgisayar kurulum dosyası bulunur.
