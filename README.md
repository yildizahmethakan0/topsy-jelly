# Topsy Jelly web sitesi

App Store'un istediği iki sayfa (gizlilik politikası ve destek) ile küçük bir ana sayfa. Düz HTML; derleme adımı yok.

| Dosya | Ne için |
|---|---|
| `index.html` | Ana sayfa |
| `privacy.html` | Gizlilik politikası (App Store'da zorunlu) |
| `support.html` | Destek sayfası (App Store'da zorunlu) |

## Yayınlamadan önce doldurulacak yerler

Dosyalarda köşeli parantezle işaretli:

- `[DEVELOPER NAME]` / `[GELİŞTİRİCİ ADI]` — App Store'da görünecek geliştirici adı
- `[CONTACT EMAIL]` / `[İLETİŞİM E-POSTASI]` — herkese açık olacak bir destek e-postası
- `[DATE]` / `[TARİH]` — politikanın yayın tarihi

## GitHub Pages ile yayınlama

Bu klasör oyunun kaynak kodundan ayrı, **herkese açık** kendi deposuna konur (oyunun kodunu açmak gerekmez).

1. GitHub'da herkese açık yeni bir depo oluştur, ör. `topsy-jelly`.
2. Bu klasörün içeriğini o depoya gönder:

   ```bash
   cd site
   git init -b main
   git add .
   git commit -m "Topsy Jelly sitesi"
   git remote add origin https://github.com/<kullanıcı-adı>/topsy-jelly.git
   git push -u origin main
   ```

3. Depoda Settings → Pages → "Deploy from a branch" → `main` / `/ (root)` seç ve kaydet.
4. Birkaç dakika sonra site şu adreste açılır: `https://<kullanıcı-adı>.github.io/topsy-jelly/`

App Store Connect'e girilecek adresler:

- Gizlilik politikası: `https://<kullanıcı-adı>.github.io/topsy-jelly/privacy.html`
- Destek: `https://<kullanıcı-adı>.github.io/topsy-jelly/support.html`

Uygulama yayınlanınca `index.html` içindeki yorum satırına alınmış App Store düğmesi açılıp bağlantısı yazılır.
