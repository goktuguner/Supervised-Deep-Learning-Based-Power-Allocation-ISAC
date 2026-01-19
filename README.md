# Supervised-Deep-Learning-Based-Power-Allocation-ISAC
# Bitirme Projesi - Kaynak Kod Paketi

Bu paket, bitirme raporunda anlatılan veri hazırlama, model karşılaştırma, performans değerlendirme ve simülasyon adımlarının Python implementasyonlarını içerir.

İÇERİK (DOSYALAR):
- Data Preparation.py: Veri okuma/temizleme, gerekli dönüşümler ve modelleme için veri setinin hazırlanması.
- Grid Search vs Traditional Way.py: Grid search yaklaşımı ile geleneksel (manuel/klasik) yaklaşımın karşılaştırılması.
- Model Comparison.py: Modellerin eğitimi ve temel karşılaştırma pipeline’ı.
- Model Comparison Performance.py: Performans metriklerinin hesaplanması, karşılaştırma ve (varsa) görselleştirmeler.
- Uzaklaşan Simülasyon.py: Simülasyon senaryosu ve sonuçların üretilmesi.

GEREKSİNİMLER:
- Python 3.9+ (önerilen: 3.10+)
- Gerekli kütüphaneler proje dosyalarında import edilen paketlerdir (ör. numpy, pandas, scikit-learn, matplotlib vb.).
- Eğer requirements.txt yoksa temel kurulum için örnek: pip install numpy pandas scikit-learn matplotlib

KURULUM:
1) ZIP içeriğini bir klasöre çıkarın.
2) Terminal/Command Prompt ile klasöre girin.
3) (Opsiyonel ama önerilir) Sanal ortam oluşturun:
   - Windows: python -m venv venv  ->  venv\Scripts\activate
   - macOS/Linux: python3 -m venv venv  ->  source venv/bin/activate
4) Gerekli paketleri kurun:
   - pip install -r requirements.txt (varsa)
   - yoksa: pip install numpy pandas scikit-learn matplotlib

ÇALIŞTIRMA SIRASI (ÖNERİLEN):
1) Veri hazırlama:
   python "Data Preparation.py"
2) Model karşılaştırma (eğitim ve temel sonuçlar):
   python "Model Comparison.py"
3) Performans analizi / metrikler:
   python "Model Comparison Performance.py"
4) Grid Search vs Traditional Way karşılaştırması:
   python "Grid Search vs Traditional Way.py"
5) Simülasyon:
   python "Uzaklaşan Simülasyon.py"
Not: Bazı dosyalar aynı veriyi kullandığı için önce Data Preparation.py çalıştırılması önerilir.

ÇIKTILAR:
- Çıktı dosyaları (Excel/CSV/figür) kod içinde belirtilen klasörlere kaydedilir.
- Eğer kodlar aynı klasöre çıktı üretiyorsa, çalıştırdığınız dizinde oluşacaktır.
- Çıktı yolu değiştirmek isterseniz ilgili .py dosyalarında output/save/export bölümlerindeki path’i güncelleyin.

SIK KARŞILAŞILAN SORUNLAR:
- FileNotFoundError (dosya yolu hatası): Veri dosyası/klasör yolu kod içinde farklı bir dizini işaret ediyor olabilir. Kod içindeki path’leri kendi bilgisayarınızdaki konuma göre güncelleyin.
- ModuleNotFoundError (eksik kütüphane): Hata mesajındaki paketi kurun: pip install <paket_adi>

NOTLAR:
- Bu paket, bitirme raporunu desteklemek için hazırlanmıştır.
- Kodlar modüler olarak ayrılmıştır; rapordaki akışa göre çalıştırma sırası yukarıdaki gibidir.
