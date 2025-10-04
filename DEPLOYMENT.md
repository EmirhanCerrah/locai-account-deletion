# 🚀 GitHub Pages'e Yayınlama Rehberi

## Adım 1: GitHub'da Repository Oluştur

1. GitHub'a giriş yap: https://github.com
2. Sağ üstten **"New repository"** butonuna tıkla
3. Repository bilgilerini doldur:
   - **Repository name:** `locai-account-deletion`
   - **Description:** "Account deletion page for LOCAI Travel App"
   - **Public** seçeneğini işaretle (GitHub Pages için gerekli)
   - **README** ekleme (zaten var)
4. **"Create repository"** butonuna tıkla

---

## Adım 2: Kodu GitHub'a Yükle

Terminal'de şu komutları çalıştır:

```bash
# Dizine git
cd locai-account-deletion

# GitHub remote ekle (kendi kullanıcı adınla değiştir)
git remote add origin https://github.com/KULLANICI_ADIN/locai-account-deletion.git

# Main branch'e push et
git branch -M main
git push -u origin main
```

**ÖNEMLİ:** `KULLANICI_ADIN` kısmını kendi GitHub kullanıcı adınla değiştir!

---

## Adım 3: GitHub Pages'i Aktif Et

1. GitHub repository sayfasına git
2. Üstten **"Settings"** (⚙️) sekmesine tıkla
3. Sol menüden **"Pages"** seçeneğine tıkla
4. **"Source"** kısmında:
   - **Branch:** `main` seç
   - **Folder:** `/ (root)` seç
5. **"Save"** butonuna tıkla
6. Sayfa yenilendikten sonra üstte yeşil bir kutu çıkacak:
   ```
   ✅ Your site is live at https://KULLANICI_ADIN.github.io/locai-account-deletion/
   ```

---

## Adım 4: Sayfayı Test Et

1. Tarayıcında bu URL'yi aç:
   ```
   https://KULLANICI_ADIN.github.io/locai-account-deletion/
   ```

2. Sayfa düzgün yüklendiyse ✅
3. Mobil görünümü test et (F12 → mobil mod)

---

## Adım 5: Google Play Console'a URL Ekle

1. Google Play Console'a giriş yap
2. Uygulamanı seç
3. **"Policy"** → **"App content"** → **"Data safety"** bölümüne git
4. **"Manage"** butonuna tıkla
5. **"Data types"** kısmında **"Account"** bilgilerini kontrol et
6. **"Data deletion"** seçeneğinde:
   - ✅ **"Users can request that their data be deleted"**
   - **URL:** `https://KULLANICI_ADIN.github.io/locai-account-deletion/`
7. **"Save"** butonuna tıkla

---

## 📝 E-posta Adresi Güncelleme

`index.html` dosyasında şu satırları kendi e-posta adresinle değiştir:

```html
<!-- Satır 113 civarı -->
<p><strong>E-posta:</strong> support@locai.app</p>

<!-- Satır 133 civarı -->
<p style="margin-top: 10px;">Herhangi bir sorunuz için: support@locai.app</p>
```

Değiştirdikten sonra:
```bash
git add index.html
git commit -m "Update support email"
git push
```

GitHub Pages otomatik olarak güncellenecek (2-3 dakika sürebilir).

---

## 🔧 Özelleştirme

### Logo Eklemek İsterseniz:

`index.html`'in başına logo ekle:

```html
<h1>
    <img src="logo.png" alt="LOCAI" style="height: 40px; vertical-align: middle;">
    LOCAI - Hesap Silme
</h1>
```

Logo dosyasını da yükle:
```bash
# logo.png dosyasını dizine kopyala
git add logo.png
git commit -m "Add logo"
git push
```

---

## ✅ Kontrol Listesi

- [ ] GitHub repository oluşturuldu
- [ ] Kod GitHub'a yüklendi
- [ ] GitHub Pages aktif edildi
- [ ] Sayfa test edildi ve çalışıyor
- [ ] E-posta adresleri güncellendi
- [ ] Google Play Console'a URL eklendi
- [ ] Mobil görünüm test edildi

---

## 🆘 Sorun Giderme

### Sayfa 404 Hatası Veriyor

- GitHub Pages'in aktif olduğunu kontrol et
- `main` branch ve `/ (root)` folder seçili olmalı
- 5-10 dakika bekle (ilk yayında sürebilir)

### Güncellemeler Görünmüyor

- GitHub'da commit'in yapıldığını kontrol et
- GitHub Pages'in "Actions" sekmesinden deployment durumunu kontrol et
- Tarayıcı cache'ini temizle (Ctrl+Shift+R)

### URL Çalışmıyor

- Repository public olmalı (Settings → Danger Zone → Change visibility)
- Repository adının doğru olduğunu kontrol et

---

## 📞 Yardım

Herhangi bir sorun yaşarsan:
1. GitHub Issues: Repository sayfasında "Issues" sekmesi
2. GitHub Docs: https://docs.github.com/pages

---

© 2025 LOCAI Travel App

