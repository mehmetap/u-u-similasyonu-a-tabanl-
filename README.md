# Uçuş Kontrol Paneli Simülasyonu

HTML, CSS ve JavaScript ile tarayıcı içinde çalışan eğitim demosu.
Üretilen değerler sentetiktir; gerçek uçuş kontrolü veya telemetri bağlantısı yoktur.

## Çalıştırma

```sh
python -m http.server 8000
```

`http://localhost:8000/preview.html` adresini açın.

| Dosya | İşlev |
|---|---|
| `preview.html` | Yerel kurallı asistan ve isteğe bağlı proxy desteği olan genişletilmiş demo |
| `tb2_kontrol_paneli_system.html` | Yerel senaryo cevaplarını gösteren önceki panel |
| `kodlar.txt` | Mevcut kaynak notları |
| `air kontrol sistem pdf.pdf` | Mevcut proje belgesi |

Panel senaryoları, gösterge güncellemeleri ve PID gösterimi içerir.
Yerel asistan bir dil modeli değildir. `preview.html` içindeki `AI_RUNTIME`
proxy ayarı ancak sizin sağladığınız bir backend ile çalışır; başarısız HTTP
isteklerinde yerel yanıta döner. Tarayıcıya servis anahtarı eklemeyin.
Eski paneldeki kimlik doğrulamasız harici API çağrısı kaldırıldı.
Gösterilen senaryo metinleri gerçek uçuş prosedürü olarak kullanılmaz.
