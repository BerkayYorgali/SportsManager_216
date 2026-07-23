# Sports Manager

Futbol ve voleybol menajerlik oyunu (JavaFX).

---

## 🎮 Sadece oynamak istiyorum

1. **[Releases](https://github.com/BerkayYorgali/SportsManager_216/releases)** sayfasına git.
2. En son sürümdeki **`SportsManager-Setup-*.exe`** dosyasını indir.
3. Çift tıkla → kurulumu tamamla → Başlat Menüsü'nden **Sports Manager**'ı aç.

Java kurmana **gerek yok** — Java ve tüm kütüphaneler kurulumun içinde gelir.

> Windows "bilinmeyen yayıncı" uyarısı verirse: **More info → Run anyway**.
> (Uygulama dijital olarak imzalı olmadığı için normaldir.)

Kayıtların şurada tutulur: `C:\Users\<kullanıcı>\SportsManager\saves`

---

## 🛠️ Geliştirmek istiyorum

Gereksinimler: **JDK 23** ve **Maven**.

```bash
git clone https://github.com/BerkayYorgali/SportsManager_216.git
cd SportsManager_216

# Oyunu çalıştır
mvn javafx:run
```

Çalıştırılabilir tek dosya (fat jar) üretmek için:

```bash
mvn clean package -DskipTests
java -jar target/SportsManager.jar
```

---

## 📦 Yeni sürüm yayınlama (bakımcı için)

Kurulum `.exe`'si **GitHub Actions** tarafından bulutta otomatik üretilir.
Yeni bir sürüm çıkarmak için sadece bir etiket (tag) push et:

```bash
git tag v1.0
git push origin v1.0
```

Ardından [Actions](https://github.com/BerkayYorgali/SportsManager_216/actions) sekmesinde
derleme başlar; bittiğinde kurulum `.exe`'si otomatik olarak
[Releases](https://github.com/BerkayYorgali/SportsManager_216/releases) sayfasına yüklenir.

> Test için: Actions sekmesi → **Build Windows Installer** → **Run workflow** ile
> etiket push etmeden de derleme yapıp çıktıyı artifact olarak indirebilirsin.
