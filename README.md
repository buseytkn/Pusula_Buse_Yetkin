# FİZİKSEL TIP VE REHABİLİTASYON ANALİZİ - CASE ÇALIŞMASI

** Ad Soyad:** Buse Yetkin  
** E-Posta:** ytkn.bs@gmail.com  

## Proje Hakkında  
Bu proje, fiziksel tıp ve rehabilitasyon alanına ait bir hasta veri seti üzerinde keşifsel veri analizi (EDA), veri temizleme (preprocessing) ve feature engineering adımlarını kapsamaktadır.  
Amaç, verilen veri setini modellemeye uygun hale getirmektir.

## Proje Dosya Yapısı
data_analysis.ipynb # EDA (Keşifsel Veri Analizi) notebook  
preprocessing.ipynb # Veri temizleme ve ön işleme notebook  
belge.md # Ayrıntılı analiz raporu  
figures/ # Analiz sırasında üretilen grafiklerin bir kısmı  
├── age_hist.png  
├── kronik_cinsiyet.png  
├── ...  
talent_academy_case_dt_2025.xlsx # Orijinal veri seti

## Analiz ve Uygulanan Adımlar
- **EDA (Keşifsel Veri Analizi)**  
  - Yaş dağılımı, cinsiyet farkları, kronik hastalık ve alerji dağılımları incelendi.  
  - Eksik değerler ve yazım hataları tespit edildi.  
  - Hasta bazlı tanı ve tedavi sayılarına dair özet istatistikler çıkarıldı.  

- **Preprocessing (Veri Temizleme ve Ön İşleme)**  
  - Eksik değerler dolduruldu (mode, KNNImputer, hasta bazlı doldurma).  
  - Kategorik değişkenler OneHotEncoder ve LabelEncoder ile kodlandı.  
  - Sayısal değişkenler için StandardScaler ve MinMaxScaler uygulandı.  
  - Yazım hataları düzeltildi ve gereksiz değerler temizlendi.  

- **Feature Engineering (Özellik Mühendisliği)**  
  - Toplam_Tani: Hasta başına benzersiz tanı sayısı.  
  - Toplam_Tedavi: Hasta başına benzersiz tedavi sayısı.

## Nasıl Çalıştırılır?

1. Bu projeyi bilgisayarına indir:  
   - GitHub sayfasından **Code → Download ZIP** diyerek indirebilirsin.  
   - Veya terminal üzerinden:  
     ```bash
     git clone https://github.com/<kullanici_adi>/pusula_buse_yetkin.git
     ```

2. Python 3.10+ ortamında gerekli kütüphaneleri yükle:  
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
3. Çalıştırmak için:

data_analysis.ipynb notebook’unu açarak EDA adımlarını çalıştırabilirsin.

preprocessing.ipynb notebook’unu açarak veri temizleme ve ön işleme adımlarını çalıştırabilirsin.

Görseller figures/ klasöründe hazırdır.

Ayrıntılı rapor için belge.md dosyasını inceleyebilirsin.
