
#  Fake News Detection with Machine Learning

Bu proje, sahte haberleri tespit edebilmek amacıyla gözetimli öğrenme yöntemlerini kullanarak gerçekleştirilmiştir. Metin verileri üzerinde TF-IDF tabanlı öznitelik çıkarımı ve makine öğrenmesi modelleri ile sınıflandırma işlemi yapılmıştır.

##  Veri Seti

Veri seti Kaggle üzerinden temin edilmiştir:  
[Fake News Detection Dataset – Mahdi Mashayekhi](https://www.kaggle.com/datasets/mahdimashayekhi/fake-news-detection-dataset)

- **Etiketler:** `FAKE` ve `REAL`
- **Sınıf Dağılımı:** %50 sahte, %50 gerçek haber (dengeli)

##  Problem Tanımı

Amaç, haber metinlerine bakarak bir haberin **sahte mi yoksa gerçek mi olduğunu tahmin etmektir.**  
Doğruluk (accuracy), kesinlik (precision), duyarlılık (recall) ve F1 skoru gibi metriklerle model performansı değerlendirilmiştir.

##  Kullanılan Yöntemler

- **Veri Ön İşleme**
  - Küçük harfe çevirme
  - Noktalama işaretlerinin temizlenmesi
  - Stop words temizliği
- **Öznitelik Çıkarımı**
  - `TF-IDF` (unigram ve bigram)
- **Sınıflandırma Modelleri**
  - Logistic Regression (başlıca model)
- **Değerlendirme Metrikleri**
  - Accuracy
  - Precision
  - Recall
  - F1 Score

##  Sonuçlar

Model sonuçları aşağıdaki gibidir:

| Metrik     | Değer     |
|------------|-----------|
| Accuracy   | 0.5175    |
| Precision  | 0.5244    |
| Recall     | 0.5244    |
| F1 Score   | 0.5244    |

Veri setindeki etiketlerin dengeli olması nedeniyle %50’nin üzerindeki her başarı modeli anlamlı kılar, ancak sonuçlar sınıflar arası ayrımın zor olduğunu göstermektedir. Bu da daha gelişmiş yöntemlere geçilmesi gerektiğini ortaya koymaktadır.

##  İyileştirme Önerileri

- BERT, Word2Vec gibi bağlamsal metin temsil yöntemleri kullanılabilir
- Derin öğrenme modelleri (LSTM, transformer tabanlı modeller) ile geliştirme yapılabilir
- Hata yapan örneklerin analizi yapılarak daha özelleşmiş modeller geliştirilebilir

##  Kaynaklar

- [Kaggle Notebook](https://www.kaggle.com/code/sametkusdemir/fake-news-detection)
- [Veri Seti](https://www.kaggle.com/datasets/mahdimashayekhi/fake-news-detection-dataset)

---


- [@sametkusdemir](https://www.kaggle.com/sametkusdemir)
