# 📱 RotaBrowser Mobile (Özgün Mobil Kiosk Çekirdeği)

**RotaBrowser Mobile**, web tabanlı uygulamalarınızı (CRM, ERP, Otomasyon Panelleri, Saha Sistemleri) standart bir web sitesi gibi değil, sanki **yerel (native) bir Android uygulamasıymış** gibi çalıştırmanızı sağlayan **özelleştirilebilir (White-Label)** bir mobil kiosk ve tarayıcı altyapısıdır.

## 💡 Neden RotaBrowser Mobile?

Geliştirdiğiniz web projelerini mobil cihazlarda müşterilerinize sunarken standart bir Chrome veya Safari sekmesi kullanmak kurumsal algıyı düşürebilir, kullanıcıların başka sekmelere kaçmasına neden olabilir. 

RotaBrowser Mobile; dışarıdan gelen URL çubuğunu, gereksiz tarayıcı butonlarını ve mobil karmaşayı gizleyerek kullanıcıyı tamamen **sizin belirlediğiniz rotada** tutar. Müşterileriniz sadece tek bir `.apk` dosyasını kurar ve doğrudan sizin uygulamanıza giriş yapar.

## 🚀 Temel Özellikler

* **Kurumsal Kimlik (White-Label):** Uygulama adı, başlangıç URL'si ve "Hakkında" ekranındaki şirket bilgileri doğrudan uygulamanın içindeki tercih ekranından anında değiştirilebilir.
* **Tam Kiosk Modu (Hard-Kiosk):** Sistem yöneticisi "Tercihler" menüsünden üst barı, sekmeleri ve yönlendirme butonlarını kapattığı an uygulama tam bir kiosk'a dönüşür.
* **Şifreli Arayüz Güvenliği:** Uygulamanın ayarlar menüsü yönetici şifresi ile korunur. Ayarlar kilitlendiğinde son kullanıcılar adres satırını göremez, dışarı çıkamaz.
* **Gerçek Çoklu Sekme (Multi-Tab):** Mobil cihazları yormayan, arkada oturumları koruyan sekme altyapısı ve hızlı erişim için "Kartlı Yeni Sekme / Favoriler" arayüzü.
* **İzole Veri Yapısı:** Uygulama içindeki çerezler (cookies), şifreler ve tarama geçmişi Android'in yerel tarayıcılarına sızmaz. Veriler cihaz hafızasında güvenle tutulur.
* **Gelişmiş Modüller:** * Geri sayım sayacı ile **Otomatik Yenileme**.
  * Siteleri PC formatında açmak için **Masaüstü Görünümü** (User-Agent spoofing).
  * Menü gizlendiğinde hayat kurtaran **Hayalet Menü (Floating Action Button)**.

## 🛠 Teknolojiler

* **Dil:** C#
* **Arayüz:** .NET MAUI (Multi-platform App UI)
* **Web Motoru:** Android WebKit (Yerleşik Mobil WebView)
* **Framework:** .NET 9.0

## 📦 Kurulum ve Kullanım (Son Kullanıcılar İçin)

1. `Releases` sekmesinden en güncel **`.apk`** dosyasını Android cihazınıza indirin ve kurun.
2. Uygulamayı açın ve sağ üstteki hamburger menüye (`☰`) tıklayarak **Tercihler** sekmesine girin.
3. `Ana Sayfa` URL'nizi, uygulamanızın adını ve Hakkında metnini kendinize göre düzenleyin.
4. Alt kısımdan gizlemek istediğiniz arayüz elemanlarını (Örn: URL Çubuğu, Sekmeler) kapatın.
5. Bir yönetici şifresi belirleyip kaydedin. Uygulama anında sizin özel Kiosk'unuza dönüşecektir.

## 🎨 Geliştiriciler İçin (İkon Değiştirme)

Uygulamayı kendi şirketinizin amblemiyle (.apk ikonu) müşterilerinize sunmak isterseniz:
1. Kaynak kodunu Visual Studio'da açın.
2. `Resources/AppIcon/appicon.png` dosyasını kendi şirket logonuz ile değiştirin (Kare format önerilir).
3. Dosyaya sağ tıklayıp "Build Action" seçeneğini `MauiIcon` yapın.
4. Projeyi Release modunda derleyerek kendi markanıza özel (White-Label) imzalı APK'nızı oluşturun.

---
*Bu proje, kapalı devre web sistemlerini profesyonel bir mobil deneyimle sunmak isteyen şirketler ve geliştiriciler için tasarlanmıştır.*
