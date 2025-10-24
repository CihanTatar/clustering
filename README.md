Country Clustering and Data Analysis / Ülke Kümeleme ve Veri Analizi

Bu proje, ülkeleri sosyoekonomik göstergelerine göre benzer gruplara ayırmayı amaçlamaktadır. K-Means ve HDBSCAN algoritmaları kullanılarak ülkeler arasındaki benzerlikler ve farklılıklar incelenmiştir. Ayrıca veri analizi ve görselleştirme adımlarıyla ülkelerin ekonomik durumları değerlendirilmiştir.

Veri setinde yer alan kolonlar:  
country, child_mort (bebek ölüm oranı), exports (ihracat), health (sağlık harcamaları), imports (ithalat), income (kişi başı gelir), inflation (enflasyon oranı), life_expec (yaşam beklentisi), total_fer (doğurganlık oranı), gdpp (kişi başı GSYH).

Veri ön işleme aşamasında eksik değerler temizlenmiş, değişkenlerin dağılımları incelenmiş ve korelasyon analizi yapılmıştır.  
K-Means algoritması için optimum küme sayısı Elbow Method ve Silhouette Score yöntemleriyle belirlenmiştir.  
HDBSCAN uygulanarak yoğunluk tabanlı kümeleme yapılmış ve ülkeler aşağıdaki dört sınıfa ayrılmıştır:

- absolutely necessary  
- neccessary  
- In Between  
- no neccessary  

Bu sınıflar, ülkelerin ekonomik göstergelerine göre birbirine olan benzerlik derecelerini temsil etmektedir.

Kullanılan kütüphaneler: pandas, numpy, matplotlib, seaborn, scikit-learn, hdbscan

Geliştirilebilecek noktalar:  
• PCA veya t-SNE ile boyut indirgeme ve kümelerin daha net görselleştirilmesi  
• Küme sonuçlarının harita üzerinde gösterilmesi  
• Her sınıfın ortalama ekonomik göstergelerini özetleyen metriklerin oluşturulması  

Yazar: Cihan Tatar  
E-posta: tatarcihan25@hotmail.com


English Version

This project aims to cluster countries based on socioeconomic indicators using K-Means and HDBSCAN algorithms. The analysis explores relationships between countries and their economic similarities.

Dataset columns:  
country, child_mort (child mortality rate), exports, health (health expenditure), imports, income, inflation, life_expec (life expectancy), total_fer (fertility rate), gdpp (GDP per capita).

After cleaning and preprocessing the data, distributions and correlations were analyzed.  
The optimal number of clusters for K-Means was determined using the Elbow Method and Silhouette Score.  
HDBSCAN was then applied for density-based clustering, and countries were categorized into four groups:

- absolutely necessary  
- neccessary  
- In Between  
- no neccessary  

These classes represent the relative socioeconomic importance and similarity of countries within each cluster.

Libraries used: pandas, numpy, matplotlib, seaborn, scikit-learn, hdbscan

Possible improvements:  
• Apply PCA or t-SNE for clearer visualization of clusters  
• Display clustering results on a world map  
• Generate summary statistics for each class’s economic indicators  

Author: Cihan Tatar  
Email: tatarcihan25@hotmail.com
