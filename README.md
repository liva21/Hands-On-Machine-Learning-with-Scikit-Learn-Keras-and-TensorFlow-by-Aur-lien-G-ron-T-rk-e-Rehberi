# 📚 Hands-On Machine Learning — Türkçe Rehber

**Aurélien Géron**'ın *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* kitabının tüm bölümlerini Türkçe açıklamalarla anlattığım bir rehber.

> Terimler İngilizce kalmaya devam ediyor — amaç teknik terminolojiye yabancılaşmadan, Türkçe düşünerek öğrenmek.

---

## 🎯 Bu Repo Neden Var?

Kitabı okurken "kodu anlıyorum ama *neden* böyle yazıldığını tam kavrayamıyorum" hissini çok yaşadım. Her bir kod satırının ne yaptığını, hangi matematiksel fikrin arkasında yattığını ve alternatiflerine göre neden bu yolun seçildiğini anlamak istiyordum. Bunun için her bölümü baştan sona geçip kodların içine Türkçe açıklamalar yazdım.

Bu notebook'lar:
- Orijinal kodun **hiçbir satırını değiştirmiyor** — sadece üstüne `#` yorumları ve açıklayıcı markdown hücreler ekliyor
- Her fonksiyon, her parametre, her matematiksel kavram açıklanıyor
- Bölüm başlarında konunun teorik altyapısını anlatan Türkçe özetler var
- Sıfırdan başlayanlar için de, kitabı daha önce okumuş olup pekiştirmek isteyenler için de uygun

---

## 📂 İçerik

```
📁 repo/
├── 01_the_machine_learning_landscape_TURKCE.ipynb
├── 02_end_to_end_machine_learning_project_TURKCE.ipynb
├── 03_classification_TURKCE.ipynb
├── 04_training_models_TURKCE.ipynb
├── 05_support_vector_machines_TURKCE.ipynb
├── 06_decision_trees_TURKCE.ipynb
├── 07_ensemble_learning_and_random_forests_TURKCE.ipynb
├── 08_dimensionality_reduction_TURKCE.ipynb
├── 09_unsupervised_learning_TURKCE.ipynb
├── 10_neural_nets_with_keras_TURKCE.ipynb
├── 11_training_deep_neural_networks_TURKCE.ipynb
├── 12_custom_models_and_training_with_tensorflow_TURKCE.ipynb
├── 13_loading_and_preprocessing_data_TURKCE.ipynb
├── 14_deep_computer_vision_with_cnns_TURKCE.ipynb
├── 15_processing_sequences_using_rnns_and_cnns_TURKCE.ipynb
├── 16_nlp_with_rnns_and_attention_TURKCE.ipynb
├── 17_autoencoders_gans_and_diffusion_models_TURKCE.ipynb  (eski 18)
├── 18_reinforcement_learning_TURKCE.ipynb                  (eski 19)
└── README.md
```

---

## 🗂️ Bölüm Bazında Konu Özeti

### Bölüm 1 — The Machine Learning Landscape
Machine Learning'e giriş: supervised/unsupervised/reinforcement learning farkları, model-based vs instance-based öğrenme, overfitting/underfitting kavramları. GDP vs Yaşam Memnuniyeti örneğiyle Linear Regression ve K-Nearest Neighbors'ın Scikit-Learn API'si üzerinden karşılaştırması.

### Bölüm 2 — End-to-End Machine Learning Project
Gerçek bir projede baştan sona akış: veri indirme, keşifsel analiz (EDA), özellik mühendisliği (feature engineering), pipeline oluşturma, model seçimi, cross-validation, hyperparameter tuning ve modeli kaydetme.

### Bölüm 3 — Classification
İkili ve çok sınıflı sınıflandırma. SGDClassifier, Confusion Matrix, Precision/Recall/F1, ROC-AUC, OvO/OvR stratejileri. MNIST veri setiyle uygulamalı çalışma.

### Bölüm 4 — Training Models
Lineer Regresyon'un matematiksel temeli: Normal Equations, Gradient Descent (Batch, Stochastic, Mini-batch). Polynomial Regression, Learning Curves, Ridge/Lasso/ElasticNet regularization, Logistic Regression ve Softmax Regression.

### Bölüm 5 — Support Vector Machines (SVM)
Hard/soft margin sınıflandırma, kernel trick (polynomial, RBF), SVM regresyon. Destek vektörlerinin geometrik yorumu ve C/gamma hiperparametre etkilerinin görselleştirilmesi.

### Bölüm 6 — Decision Trees
Karar ağaçlarının yapısı, CART algoritması, Gini impurity ve entropy. Ağaç derinliği ile overfitting ilişkisi, instability sorunu ve görselleştirme.

### Bölüm 7 — Ensemble Learning and Random Forests
Voting, Bagging, Pasting, Random Forest, Extra-Trees, AdaBoost, Gradient Boosting, Stacking. Her yöntemin güçlü/zayıf tarafları ve bias-variance tradeoff bağlantısı.

### Bölüm 8 — Dimensionality Reduction
Boyut lanetini anlama. PCA, Kernel PCA, Locally Linear Embedding (LLE). Explained variance ratio, n_components seçimi ve görselleştirme teknikleri.

### Bölüm 9 — Unsupervised Learning
K-Means, DBSCAN, küme kalite metrikleri (silhouette score, inertia). Gaussian Mixture Models (GMM), anomali tespiti ve yoğunluk tahmini.

### Bölüm 10 — Neural Nets with Keras
Keras'a giriş: Sequential ve Functional API. Dense katmanlar, aktivasyon fonksiyonları, callbacks (EarlyStopping, ModelCheckpoint), TensorBoard, hyperparameter tuning (Keras Tuner).

### Bölüm 11 — Training Deep Neural Networks
Vanishing/exploding gradient problemi. Glorot/He initialization, Batch Normalization, Gradient Clipping. Optimizer'lar: SGD+momentum, RMSProp, Adam, AdaGrad. Learning rate scheduling ve regularization teknikleri (Dropout, MC Dropout, L1/L2).

### Bölüm 12 — Custom Models and Training with TensorFlow
TensorFlow'un düşük seviye API'si: tensor işlemleri, `tf.GradientTape`, custom layer/loss/metric/model. TF Functions ve autograph mekanizması.

### Bölüm 13 — Loading and Preprocessing Data
`tf.data` API ile büyük veri setleri: `Dataset.map`, `cache`, `prefetch`, `interleave`. TFRecord formatı, feature column'lar ve Keras preprocessing layer'ları.

### Bölüm 14 — Deep Computer Vision with CNNs
Konvolüsyon, pooling, stride ve padding kavramları. LeNet-5'ten ResNet'e mimari evrimi. Transfer learning, data augmentation, object detection (YOLO ailesi) ve semantic segmentation.

### Bölüm 15 — Processing Sequences with RNNs and CNNs
Zaman serisi tahmini. Vanilla RNN, LSTM, GRU. WaveNet mimarisi ile dizi modelleme ve 1D konvolüsyon.

### Bölüm 16 — NLP with RNNs and Attention
Karakter ve kelime bazlı dil modeli. Encoder-Decoder mimarisi, Attention mekanizması, Transformer ve Multi-Head Attention. Hugging Face ile pretrained model kullanımı.

### Bölüm 17 — Autoencoders, GANs and Diffusion Models
Undercomplete/Stacked/Convolutional/Recurrent Autoencoder. Denoising, Sparse, Variational (VAE) ve Discrete VAE. GAN, DCGAN. DDPM (Denoising Diffusion Probabilistic Model), DDIM ve Stable Diffusion.

### Bölüm 18 — Reinforcement Learning
Gymnasium ile CartPole ortamı. Hard-coded policy, Policy Networks, REINFORCE algoritması. Markov Chains, MDP, Q-Value Iteration, Q-Learning, Deep Q-Network (DQN), Actor-Critic ve PPO (Stable-Baselines3 ile Atari Breakout).

---

## 🛠️ Kullanılan Teknolojiler

| Kütüphane | Versiyon | Kullanım Amacı |
|-----------|----------|----------------|
| Python | ≥ 3.10 | Temel dil |
| Scikit-Learn | ≥ 1.6.1 | Klasik ML algoritmaları |
| TensorFlow / Keras | ≥ 2.x | Derin öğrenme |
| PyTorch | ≥ 2.6.0 | Derin öğrenme (bölüm 17-18) |
| NumPy | - | Sayısal işlemler |
| Pandas | - | Veri analizi |
| Matplotlib | - | Görselleştirme |
| Gymnasium | - | RL ortamları |
| Stable-Baselines3 | - | PPO, A2C vb. |

---

## 🚀 Nasıl Kullanılır?

### Yerel Ortamda

```bash
# Repoyu klonla
git clone https://github.com/liva21/Hands-On-Machine-Learning-with-Scikit-Learn-Keras-and-TensorFlow-by-Aur-lien-G-ron-T-rk-e-Rehberi.git

# Klasöre gir
cd Hands-On-Machine-Learning-...

# Jupyter Notebook'u başlat
jupyter notebook
```

### Google Colab'da

Her notebook'un en üstünde Colab ve Kaggle bağlantıları mevcuttur. Doğrudan tarayıcıda açıp çalıştırabilirsiniz — herhangi bir kurulum gerekmez.

---

## 📖 Orijinal Kaynak

Bu rehber, aşağıdaki kitabın Türkçe açıklamalı companion notebook'udur:

> **Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow**  
> Yazar: Aurélien Géron  
> Yayınevi: O'Reilly Media  
> Orijinal notebook'lar: [github.com/ageron/handson-ml3](https://github.com/ageron/handson-ml3)

Orijinal kodlar değiştirilmemiştir. Tüm haklar Aurélien Géron'a aittir. Bu repo yalnızca eğitim amaçlı Türkçe açıklama eklemektedir.

---

## 🤝 Katkı

Hata, eksik açıklama veya öneri için issue açabilir ya da pull request gönderebilirsiniz. Her türlü geri bildirime açığım.

---

## ⭐ Destek

Bu rehber işinize yaradıysa repoya **star** atarsanız sevinirim — başkalarının da bulmasına yardımcı olur.

---

<p align="center">
  Türkçe konuşan ML meraklıları için ❤️ ile hazırlandı
</p>
