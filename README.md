Otel Yönetim Sistemi
=======================

Bu proje, STAJ döneminde öğrenme ve pratik amaçlı geliştirilmiş basit bir 
Otel Yönetim Sistemi uygulamasıdır.

Uygulama, Python (Tkinter) ile grafik arayüzlü bir masaüstü yazılımı olarak 
geliştirilmiş ve Firebird veritabanı kullanılarak verilerin kalıcı hale 
getirilmesi sağlanmıştır.


Özellikler
-------------

- Oda Yönetimi
  * Yeni oda ekleme
  * Oda durumlarını (Boş, Dolu, Rezerve, Temizlikte) takip etme
  * Oda boşaltma & temizlik süreci

- Kişi Yönetimi
  * Yeni kişi ekleme (Ad, Soyad, Telefon, Cinsiyet)
  * Kişileri listeleme

- Rezervasyon Yönetimi
  * Odaya kişi atama (çoklu kişi desteği)
  * Giriş & çıkış tarihleri ile rezervasyon oluşturma
  * Tarih çakışmalarını kontrol etme

- Takip & Bildirim
  * Rezervasyon süresi dolduğunda uyarı verme
  * Çıkış sonrası odayı otomatik "Temizlikte" durumuna alma
  * Temizlik sonrası odayı tekrar "Boş" yapma

- Detaylı Bilgi Ekranı
  * Oda, kişi, kat, durum ve tarih filtreleri
  * Oda ve kişi bazlı arama


Kullanılan Teknolojiler
---------------------------

- Python 3
- Tkinter → GUI (masaüstü arayüz)
- Firebird → Veritabanı
- fdb → Python Firebird bağlantı kütüphanesi
- threading → Arka plan rezervasyon kontrolü


Kurulum
----------

1. Bu projeyi bilgisayarınıza klonlayın:
   git clone https://github.com/Cngzsafa/otel-yonetim-sistemi.git

2. Gerekli Python kütüphanelerini yükleyin:
   pip install fdb

3. Firebird veritabanınızda "OTEL.FDB" dosyasını oluşturun.
   Kodda varsayılan bağlantı bilgileri:
   dsn="localhost:C:/Users/""/Desktop/VERITABANI/OTEL.FDB"
   user="sysdba"
   password="masterkey"

4. Uygulamayı çalıştırın:
   python otel_app.py


Not
------

Bu proje STAJ döneminde öğrenme amaçlı geliştirilmiştir. 
Gerçek otel yönetim sistemleri için daha kapsamlı, güvenlikli ve ölçeklenebilir çözümler tercih edilmelidir.
