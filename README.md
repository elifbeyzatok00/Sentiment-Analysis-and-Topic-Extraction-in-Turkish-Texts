# Sentiment Analysis and Topic Extraction in Turkish Texts
What is Natural Language Processing (NLP) & NLP Project Example

## Table of Contents 🗒️

1. [Doğal Dil İşleme Nedir? (What is Natural Language Processing - NLP)](#)
  - [NLP'nin Temel Bileşenleri (Basic Components of NLP)](#)
  - [NLP'nin Kullanım Alanları (Areas of Use of NLP)](#)
2. [NLP Proje Örneği (NLP Project Example)](#)
  - [Türkçe Metinlerde Duygu Analizi ve Konu Çıkarımı (Sentiment Analysis and Topic Inference in Turkish Texts)](#)
      * [Adımlar (Steps)](#)
      * [Araçlar ve Kütüphaneler (Tools and Libraries)](#)
      * [Sonuçlar ve Öneriler (Results and Recommendations)](#)
      * [Örnek Referans Makale (Sample Reference Paper)](#)
  - [Proje Kodları (Project Codes)](#)
      * [0. Proje Detayları (Project Details)](#)
      * [1. Veri Ön İsleme (Data Pre-Processing)](#)
      * [2. Öznitelik Çıkarımı (Feature Extraction)](#)
      * [3. Model Oluştur (Create Model)](#)
---
## Doğal Dil İşleme Nedir? (What is Natural Language Processing - NLP)
Doğal Dil İşleme (Natural Language Processing - NLP), bilgisayarların insan dilini anlaması, yorumlaması ve üretmesi için geliştirilen yöntem ve teknikleri kapsayan bir alandır. NLP, dilbilim, bilgisayar bilimi ve yapay zeka alanlarının kesişiminde yer alır ve insanların yazılı veya sözlü dilini analiz ederek çeşitli uygulamalarda kullanmayı amaçlar.

![image](https://github.com/elifbeyzatok00/Natural-Language-Processing/assets/102792446/dc99c22c-025a-403f-b47c-a3d0e844da55)

### NLP'nin Temel Bileşenleri (Basic Components of NLP)

1. **Metin Önişleme (Text Preprocessing)**
   - **Tokenization (Kelime Ayrıştırma):** Metni kelimelere veya cümlelere bölme.
   - **Stemming ve Lemmatization:** Kelimeleri kök veya temel formlarına indirgeyerek standartlaştırma.
   - **Stop Word Removal (Yaygın Kelimelerin Kaldırılması):** Anlam açısından düşük değerli kelimeleri metinden çıkarma.
   - **Normalization (Normalizasyon):** Metindeki büyük harfleri küçük harfe çevirme, noktalama işaretlerini kaldırma vb. işlemler.

2. **Dil Modellemesi (Language Modeling)**
   - Dil modelleri, bir dildeki kelime dizilimlerini ve olasılıklarını öğrenir. Bu modeller, cümle tamamlama, makine çevirisi ve metin üretimi gibi uygulamalarda kullanılır. N-gram modelleri ve modern derin öğrenme tabanlı modeller (örneğin, GPT, BERT) bu alanda yaygındır.

3. **Sentiment Analizi (Duygu Analizi)**
   - Metinlerdeki duygusal tonun (olumlu, olumsuz, tarafsız) belirlenmesi. Bu, müşteri geri bildirimleri, sosyal medya analizleri gibi alanlarda kullanılır.

4. **Ad Öbekleri ve İsim Varlığı Tanıma (Named Entity Recognition - NER)**
   - Metindeki özel adların (örneğin, kişi isimleri, yer adları, organizasyonlar) tanımlanması ve sınıflandırılması.

5. **Parçacık Etiketleme (Part-of-Speech Tagging)**
   - Kelimelerin dil bilgisel kategorilerine (isim, fiil, sıfat vb.) göre etiketlenmesi.

6. **Makine Çevirisi (Machine Translation)**
   - Metinlerin bir dilden başka bir dile otomatik olarak çevrilmesi. Google Translate gibi hizmetler bu teknolojiyi kullanır.

7. **Özetleme (Summarization)**
   - Uzun metinlerin ana noktalarını belirleyerek kısa özetler oluşturma. İki tür özetleme yöntemi vardır: Ekstraktif (metindeki cümleleri seçme) ve abstraktif (metni yeniden formüle etme).

8. **Metin Sınıflandırma (Text Classification)**
   - Metinleri belirli kategorilere ayırma. Spam tespiti, konu sınıflandırması gibi uygulamalar bu alana girer.

![image](https://github.com/elifbeyzatok00/Natural-Language-Processing/assets/102792446/12cdce1e-2b5c-4b8a-910a-7dc6926bb39a)

### NLP'nin Kullanım Alanları (Areas of Use of NLP)

- **Arama Motorları:** Kullanıcı sorgularını anlama ve ilgili sonuçları getirme.
- **Sosyal Medya Analizi:** Kullanıcıların duygu durumlarını ve trendleri analiz etme.
- **Otomatik Yanıt Sistemleri:** Chatbotlar ve sanal asistanlar.
- **Dil Öğrenme Uygulamaları:** Dil öğretme ve çeviri uygulamaları.
- **Müşteri Hizmetleri:** Otomatik müşteri destek sistemleri.

---

## 🧪NLP Proje Örneği (NLP Project Example)

# Türkçe Metinlerde Duygu Analizi ve Konu Çıkarımı (Sentiment Analysis and Topic Extraction in Turkish Texts)

![image](https://github.com/elifbeyzatok00/Natural-Language-Processing/assets/102792446/2b3dcce2-9264-4722-8172-4e2a18727e97)

## Proje Açıklaması (Project Description)
Bu proje, Türkçe metinleri işleyerek duygu analizi yapmak ve metinlerdeki ana konuları çıkarmak amacıyla geliştirilmiştir. Proje, özellikle sosyal medya paylaşımları, müşteri yorumları ve haber metinleri gibi çeşitli Türkçe içerikli metinlerde uygulanabilir.

## Veri Seti (Dataset)
- **Örnek Veri Seti (Sample Dataset):** [Turkish Sentiment Analysis Dataset](https://huggingface.co/datasets/winvoker/turkish-sentiment-analysis-dataset)
- **Veri Seti Tanımı (Dataset Description):** Türkçe metinlerin sınıflandırılması için oluşturulmuş bir veri setidir. Bu veri seti, olumlu, olumsuz ve nötr etiketlerle belirtilmiş metinleri içerir. Duygu analizi modellerinin eğitiminde ve değerlendirilmesinde kullanılabilir.

## Adımlar (Steps)

### 1. Veri Toplama (Data Collection)
Türkçe içerikli metin verilerini toplamak için çeşitli yöntemler kullanılabilir:
- **Web Scraping Araçları (Web Scraping Tools):** BeautifulSoup, Scrapy
- **Sosyal Medya API'leri (Social Media APIs):** Twitter API, Facebook API
- **Anketler ve Formlar (Surveys and Forms)**

### 2. Veri Ön İşleme (Data Preprocessing)
Metin verilerini analiz edebilmek için aşağıdaki ön işleme adımları uygulanmalıdır:
- **Metin Normalizasyonu (Text Normalization):** Büyük-küçük harf dönüşümü gibi işlemler.
- **Gereksiz Karakterlerin Kaldırılması (Removing Unnecessary Characters):** Noktalama işaretleri ve özel karakterlerin temizlenmesi.
- **Tokenizasyon (Tokenization):** Metin verilerini kelimelere veya cümlelere ayırma.
- **Stop Words (Durma Kelimeleri) Kaldırma (Removing Stop Words):** Analiz için anlamsız olan kelimeleri çıkarma.
- **Stemming ve Lemmatization:** Kelimeleri kök veya temel hallerine indirme.
- **N-gram Oluşturma (Creating N-grams):** Kelime gruplarını ve dizilerini oluşturma.

### 3. Özellik Çıkarma (Feature Extraction)
Metin verilerini sayısal vektörlerle temsil etmek için aşağıdaki yöntemler kullanılabilir:
- **TF-IDF (Term Frequency-Inverse Document Frequency)**
- **Word Embeddings (Kelime Gömme):** Word2Vec, GloVe
- **Bag of Words (BoW)**
- **Word Frequencies (Kelime Sıklıkları)**

### 4. Metin Sınıflandırma Algoritması Tasarımı (Text Classification Algorithm Design)
Metin sınıflandırma için yaygın kullanılan algoritmalar:
- **SVM (Support Vector Machine)**
- **KNN (k-Nearest Neighbors)**
- **Evrişimli Sinir Ağları (Convolutional Neural Networks - CNN)**
- **Transformer Models (BERT, GPT)**

### 5. Duygu Analizi (Sentiment Analysis)
Türkçe metinlerdeki duyguları (olumlu, olumsuz, nötr) belirlemek için duygu analizi yapılabilir.

### 6. Görselleştirme (Visualization)
Analiz sonuçlarını görselleştirmek için kullanılabilecek yöntemler:
- **Confusion Matrix (Karmaşıklık Matrisi)**
- **Precision-Recall Curve (Hassasiyet-Duyarlılık Eğrisi)**
- **ROC Curve (Receiver Operating Characteristic Eğrisi)**
- **Class Distribution Visualization (Sınıf Dağılımı Görselleştirme)**
- **Word Clouds (Kelime Bulutları)**

## Araçlar ve Kütüphaneler (Tools and Libraries)
- **Ön İşleme (Preprocessing):** NLTK, TextBlob
- **Özellik Çıkarma (Feature Extraction):** Gensim, Scikit-learn
- **Model Eğitimi (Model Training):** TensorFlow, Keras, PyTorch
- **Görselleştirme (Visualization):** Matplotlib, Seaborn

## Sonuçlar ve Öneriler (Results and Recommendations)
Bu proje, Türkçe metinleri analiz ederek duygu ve konu çıkarımları yaparak Türkçe içerikli verilerden anlamlı bilgiler elde edilmesini sağlar. Analiz sonuçlarından çıkarılan bilgiler değerlendirilerek işletmeler veya araştırmacılar için öneriler sunulabilir.

## Örnek Referans Makale (Sample Reference Paper)
- **A Comprehensive Analysis of Static Word Embeddings for Turkish** (Sarıtaş ve diğ. 2023)


## 👩🏻‍💻Proje Kodları (Project Codes)

 0. Proje Detayları (Project Details) -> [`NLP-PROJECT.docx`](https://github.com/elifbeyzatok00/Natural-Language-Processing/blob/main/0-NLP-PROJECT.docx)

 1. Veri Ön İsleme (Data Pre-Processing) -> [`Veri On Isleme.ipynb`](https://github.com/elifbeyzatok00/Natural-Language-Processing/blob/main/1-Veri%20On%20Isleme.ipynb)

 2. Öznitelik Çıkarımı (Feature Extraction) -> [`OznitelikCikarimi.ipynb`](https://github.com/elifbeyzatok00/Natural-Language-Processing/blob/main/2-OznitelikCikarimi.ipynb)

 3. Model Oluştur (Create Model) -> [`Model.ipynb`](https://github.com/elifbeyzatok00/Natural-Language-Processing/blob/main/3-Model.ipynb)
