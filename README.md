# credit_risk_prediction
Giriş
Bu proje, banka müşterilerinin kredi riskini tahmin etmek için makine öğrenimi modelleri kullanmaktadır. Almanya'daki kredi verilerini içeren German Credit Risk veri seti kullanılmıştır.

Projede aşağıdaki adımlar izlenmiştir:

Veri ön işleme ve keşifçi veri analizi

Özellik mühendisliği

Çeşitli sınıflandırma algoritmalarının uygulanması

Model performanslarının karşılaştırılması

Metrikler
Denenen modeller ve elde edilen sonuçlar:

Model	Accuracy	Precision	Recall	F1-Score
Lojistik Regresyon	0.78	0.82	0.71	0.76
Karar Ağaçları	0.82	0.84	0.79	0.81
Rastgele Orman	0.85	0.87	0.82	0.84
XGBoost	0.86	0.88	0.83	0.85
En iyi performansı XGBoost modeli göstermiştir. Özellikle recall metriği, kötü kredi risklerini tespit etmedeki başarısı nedeniyle bu projede önemli bir metriktir.

Ekler
Projeye aşağıdaki ek çalışmalar yapılmıştır:

Streamlit ile Deployment: UI/app.py dosyasında basit bir web arayüzü oluşturulmuştur.

bash
streamlit run UI/app.py
GPU Hızlandırma: Rastgele Orman ve XGBoost modelleri CUML kütüphanesi ile GPU'da çalıştırılarak %70'e varan hız artışı sağlanmıştır.

Sonuç ve Gelecek Çalışmalar
Bu projede, müşterilerin kredi riskini makul bir doğrulukla tahmin edebilen bir model geliştirilmiştir. Gelecekte yapılabilecek iyileştirmeler:

Dinamik Veri Toplama: Gerçek zamanlı müşteri verileri ile modelin sürekli güncellenmesi

Explainable AI: Model kararlarının şeffaflığını artırmak için SHAP/LIME gibi yöntemlerin eklenmesi

Daha Büyük Veri Seti: Daha fazla örnek içeren uluslararası veri setleriyle modelin genelleme yeteneğinin artırılması

Mobil Uygulama: Banka çalışanları için kullanıcı dostu bir mobil arayüz geliştirilmesi

Linkler
Kaggle Notebook: Karar Ağaçları ve Özellik Seçimi

Kaggle Notebook: GPU ile Makine Öğrenimi

Veri Seti: German Credit Risk
