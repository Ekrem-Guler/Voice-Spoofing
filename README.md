
# 🎙️ Voice Spoofing (Ses Sahtekarlığı) Analizi ve Tespiti

**Voice Spoofing**, ses sentezleme (TTS), ses dönüştürme (Voice Conversion) veya tekrar oynatma (Replay) saldırıları gibi yöntemlerle oluşturulan sahte (deepfake) sesleri tespit etmeyi veya incelemeyi amaçlayan bir makine öğrenmesi/derin öğrenme projesidir.

## 📖 Proje Hakkında

Günümüzde ses klonlama teknolojilerinin gelişmesiyle birlikte, ses tabanlı biyometrik sistemlerin güvenliği risk altına girmiştir. Bu proje, gerçek insan sesi ile sentetik veya manipüle edilmiş sesleri birbirinden ayırmak için geliştirilmiş model mimarilerini ve özellik çıkarım yöntemlerini içerir.

## ✨ Özellikler

- **Gelişmiş Özellik Çıkarımı (Feature Extraction):** MFCC, Mel-Spektrogram ve LFCC gibi teknikler.
- **Model Mimarileri:** CNN, RNN veya Transformer tabanlı derin öğrenme modelleri ile sahte ses sınıflandırması.
- **Hızlı Tahmin (Inference):** Eğitilmiş modelleri kullanarak yeni ses dosyalarını analiz etme betikleri.
- **Veri Görselleştirme:** Gerçek ve sahte seslerin özelliklerini grafiksel olarak karşılaştıran araçlar.

## 🗂️ Veri Seti
Projede temel alınabilecek veri seti, literatürde standart olarak kabul edilen **ASVspoof** (Automatic Speaker Verification Spoofing and Countermeasures Challenge) veya benzeri bir veri setidir. 
*(Projeye entegre edilen kendi veri setinizi veya veri işleme adımlarını bu bölümde detaylandırabilirsiniz).*

## 🚀 Kurulum (Installation)

Projeyi yerel bilgisayarınızda çalıştırmak için aşağıdaki adımları takip edin:

1. **Depoyu Klonlayın:**
   ```bash
   git clone https://github.com/Ekrem-Guler/Voice-Spoofing.git
   cd Voice-Spoofing
   ```

2. **Gerekli Kütüphaneleri Yükleyin:**
   Sanal bir ortam (virtual environment) oluşturup gereksinimleri yüklemeniz önerilir:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

## 🛠️ Kullanım (Usage)

*(Projedeki gerçek dosya adlarına göre aşağıdaki komutları güncelleyebilirsiniz)*

**Modeli Eğitmek:**
```bash
python train.py --epochs 50 --batch_size 32
```

**Bir Ses Dosyasını Test Etmek (Inference):**
```bash
python predict.py --audio sample.wav
```
*(Tahmin sonucu olarak sesin `GERÇEK (Bona Fide)` veya `SAHTE (Spoofed)` olma ihtimali ekrana yazdırılacaktır.)*

## 🤝 Katkıda Bulunma
Katkılarınızı bekliyoruz! Hata bildirmek, yeni bir özellik önermek veya iyileştirme yapmak isterseniz lütfen bir **Issue** açın veya **Pull Request** gönderin.

1. Bu depoyu fork'layın.
2. Yeni bir dal (branch) oluşturun (`git checkout -b feature/yeniOzellik`).
3. Değişikliklerinizi commit edin (`git commit -m 'Yeni özellik eklendi'`).
4. Dalınıza push yapın (`git push origin feature/yeniOzellik`).
5. Bir Pull Request oluşturun.
 

## 👤 İletişim
**Geliştirici:** [Ekrem-Guler](https://github.com/Ekrem-Guler)
