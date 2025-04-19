# ft_transcendence

42 İstanbul'un bitirme projesi olarak geliştirilen, Django backend ve Pure JavaScript frontend kullanılarak oluşturulmuş bir Pong oyunu platformu.

## 🎮 Proje Hakkında

ft_transcendence, klasik Pong oyununu modern web teknolojileri ile yeniden yorumlayan bir multiplayer oyun platformudur. Proje, gerçek zamanlı oyun deneyimi, kullanıcı yönetimi ve sosyal özellikler sunmaktadır.

## 💻 Teknolojiler

### Backend
- Python 3.x
- Django
- Django Channels (WebSocket)
- PostgreSQL
- Django REST Framework

### Frontend
- Pure JavaScript
- HTML5 Canvas
- CSS3
- WebSocket API

### Authentication
- OAuth 2.0 (42 intra)
- JWT

## 🛠️ Kurulum

### Gereksinimler
- Python 3.8 veya üzeri
- PostgreSQL
- Node.js (geliştirme için)
- Redis (WebSocket için)

### Yerel Geliştirme Ortamı
1. Projeyi klonlayın:
```bash
git clone https://github.com/[kullanıcı-adı]/ft_transcendence.git
cd ft_transcendence
```

2. Python sanal ortamı oluşturun ve aktif edin:
```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
# veya
.\venv\Scripts\activate  # Windows
```

3. Bağımlılıkları yükleyin:
```bash
pip install -r requirements.txt
```

4. Veritabanını oluşturun:
```bash
python manage.py migrate
```

5. Geliştirme sunucusunu başlatın:
```bash
python manage.py runserver
```

## 📝 Özellikler

### Oyun
- [x] Gerçek zamanlı Pong oyunu
- [x] Çoklu oyuncu desteği
- [x] Özelleştirilebilir oyun ayarları
- [x] Skor takibi ve liderlik tablosu

### Kullanıcı Sistemi
- [x] 42 OAuth entegrasyonu
- [x] Kullanıcı profilleri
- [x] Avatar yükleme
- [x] İki faktörlü doğrulama (2FA)

### Sosyal Özellikler
- [x] Arkadaş sistemi
- [x] Gerçek zamanlı sohbet
- [x] Oyun davetleri
- [x] Kullanıcı durumu takibi

### Turnuva Sistemi
- [x] Turnuva oluşturma
- [x] Otomatik eşleştirme
- [x] Turnuva ağacı görüntüleme
- [x] Ödül sistemi

## 🎯 42 Proje Gereksinimleri

### Zorunlu Kısım
- [x] SPA (Single Page Application)
- [x] Kullanıcı hesap yönetimi
- [x] Gerçek zamanlı çoklu oyuncu Pong oyunu
- [x] Sohbet sistemi
- [x] Kullanıcı yetkilendirme ve güvenlik

### Bonus Özellikler
- [x] Farklı oyun modları
- [x] Turnuva sistemi
- [x] Özelleştirilebilir oyun ayarları
- [x] Gelişmiş kullanıcı istatistikleri

## 🔒 Güvenlik Özellikleri

- JWT tabanlı kimlik doğrulama
- CSRF koruması
- XSS önleme
- Rate limiting
- İki faktörlü doğrulama (2FA)
- Güvenli WebSocket bağlantıları

## 🚀 Deployment

1. Ortam değişkenlerini ayarlayın:
```bash
cp .env.example .env
# .env dosyasını düzenleyin
```

2. Veritabanını hazırlayın:
```bash
python manage.py migrate
python manage.py collectstatic
```

3. Production sunucusunu başlatın:
```bash
gunicorn config.wsgi:application
```

## 📈 Performans ve Ölçeklendirme

- Redis önbelleği
- WebSocket bağlantı havuzu
- Asenkron görev işleme
- Statik dosya CDN desteği

## 🐛 Hata Ayıklama

Yaygın hataların çözümleri:
- WebSocket bağlantı sorunları
- Veritabanı migrasyon hataları
- OAuth yapılandırma sorunları
- Oyun senkronizasyon problemleri

## 👥 Katkıda Bulunanlar

Bu proje 42 İstanbul öğrencileri tarafından geliştirilmiştir:
backend : My dear teammate Berke, www.github.com/clas0512.
frontend & game : github.com/aruzgar aerbosna intra id: ekarali, rdeyirme
My tasks are dev&ops docker systems on this project. 

## 📝 Lisans

Bu proje [MIT](LICENSE) lisansı altında lisanslanmıştır.

---

⭐️ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!


