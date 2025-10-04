# ⚡ Hızlı Başlangıç - 5 Dakikada Yayınla!

## 🎯 Gereksinimler

- GitHub hesabı (yoksa: https://github.com/join)
- Git kurulu (kontrol et: `git --version`)

---

## 📋 Adım Adım (5 Dakika)

### 1️⃣ GitHub'da Repository Oluştur (1 dk)

```
https://github.com/new
```

- **Name:** `locai-account-deletion`
- **Public** ✅
- **Create repository**

### 2️⃣ Kodu Yükle (2 dk)

Terminal'de:

```bash
cd locai-account-deletion

# Kendi GitHub kullanıcı adınla değiştir! ⚠️
git remote add origin https://github.com/KULLANICI_ADIN/locai-account-deletion.git

git branch -M main
git push -u origin main
```

### 3️⃣ GitHub Pages Aktif Et (1 dk)

1. Repository sayfasında → **Settings** ⚙️
2. Sol menü → **Pages**
3. **Branch:** `main` + `/ (root)` → **Save**
4. 2-3 dakika bekle ☕

### 4️⃣ Test Et (30 saniye)

```
https://KULLANICI_ADIN.github.io/locai-account-deletion/
```

### 5️⃣ Google Play'e Ekle (30 saniye)

Google Play Console → App content → Data safety:

```
URL: https://KULLANICI_ADIN.github.io/locai-account-deletion/
```

---

## ✅ Bitti!

Hesap silme sayfan artık canlı! 🎉

---

## 🔧 İsteğe Bağlı: E-posta Güncelle

`index.html` dosyasında `support@locai.app` yerine kendi e-postanı yaz.

```bash
# Düzenle
nano index.html  # veya herhangi bir editör

# Yükle
git add index.html
git commit -m "Update email"
git push
```

---

## 📸 Ekran Görüntüleri

### GitHub Repository Oluşturma:
![Create Repo](https://docs.github.com/assets/cb-11427/images/help/repository/repo-create.png)

### GitHub Pages Ayarı:
![Pages Settings](https://docs.github.com/assets/cb-40935/images/help/pages/select-branch-and-folder.png)

---

## 🆘 Hızlı Yardım

**❌ Sayfa 404:**
- 5 dakika bekle
- Repository **public** olmalı

**❌ Push hatası:**
- Kullanıcı adını kontrol et
- GitHub token gerekebilir

**❌ Güncellemeler görünmüyor:**
- Cache temizle (Ctrl+Shift+R)
- Actions sekmesinden deployment kontrol et

---

Daha detaylı bilgi: `DEPLOYMENT.md`

© 2025 LOCAI

