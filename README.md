# Literatür Araştırması Raporu

## 1. Human Activity Recognition for Mobile Robot - [PDF](PDFs/1_Human_Activity_Recognition_for_Mobile_Robot.pdf)

https://www.researchgate.net/publication/322675054_Human_Activity_Recognition_for_Mobile_Robot

Makalede konvolüsyonel sinir ağları (KSA) kullanılarak bir mobil robota insan hareketlerini algılatmak amaçlanmıştır. İnsan hareketlerini algılamak için derinlik kamerası kullanmak yerine Vicon hareket algılama sistemleri kullanılmıştır. Bu nedenle makalede belirtilen çalışmada herhangi bir görüntü işleme yapılmadığı görülmektedir. Bahsedilen KSA modeli, iki adet bir bouytlu konvolüsyonel katman, bir adet max pooling katmanı, bir adet tam bağlı katman ve bir adet de Softmax katmanından oluşmaktadır. KSA burada sadece insanın yaptığı hareketi sınıflandırmak için kullanılmıştır. Hareketleri algılamak için de iki bacak, iki kol, bir kafa ve bir omuzdan alınan hareket verileri kullanılmıştır. Bununla beraber KSA modelini eğitmek için ise Vicon’un sunduğu VMCUHK veri seti kullanılmıştır. KSA modeli tahmini el sıkma, kafalama, zıplama, koşma, oturma, ve yürüme sınıfları üzerinedir. Modelin yaptığı tahminler ile çıkan F1 skor sonucu %95.70 olarak hesaplanmıştır.

## 2. Human Activity Recognition with Deep Reinforcement Learning using the Camera of a Mobile Robot - [PDF](PDFs/2_Human_Activity_Recognition_with_Deep_Reinforcement_Learning_Using_the_Camera_of_a_Mobile_Robot.pdf)

https://ieeexplore.ieee.org/abstract/document/9127376

https://sci-hub.se/10.1109/PerCom45495.2020.9127376

Makalede yapılan çalışmanın amacı Reinforcement Learning (RL) kullanarak robotlar ile insan hareketlerini algılamaktır. İnsan hareketlerini algılamak için derinlik kamerası kullanılmaktadır. Fakat söz konusu çalışma robot olduğu için çalışma iki konudan bahsetmektedir. Birincisi robotu insan hareketini algılayabilmek için robotu olabilecek en uygun lokasyona getirmektir. İkincisi ise derinlik kamerası ile insan hareketlerini algılamaktır. Bahsedilen işlemleri gerçekleştirebilmek için görüntüden insan iskeleti elde edilmelidir. Bunu başarabilmek için OpenPose isimli açık kaynak olan görüntü işleme kütüphanesi kullanılmıştır. Bu kütüphane ile yapılan çalışmalarda insan vücudu 25 eklem noktasına ayrılmaktadır. İnsan hareketlerini algılamak için kullanılan yapay sinir ağları modeli şu şekildedir:

![alt text](Images/2_1.JPG)

İnsan hareketleri yemek hazırlama, çay yapma, meyve suyu yapma, bulaşık yıkama, kitap okuma, telefon kullanma, telefonda konuşma, yemek yeme, televizyon izleme, diş fırçalama, yüz yıkama ve uyumak olacak şekilde sınıflandırılmıştır. OpenPose kütüphanesinden elde edilen veriler LSTM katmanına, 64x64 lük el görüntüleri de VGG-16 konvolüsyonel sinir ağı (KSA) katmanına verilmektedir. İkisinden de elde edilen sonuçlar birleştirilip Softmax katmanıns verildikten sonra insan hareketi olarak sınıflandırılmaktadır. Robot insanı elde edilen görüntünün ortasında tutmaya çalışmaktadır ve insana belirli bir mesafeden bakmaktadır. Robotun lokasyonu ve pozisyonu tamamen derin Q-network ile belirlenir. Bahsedilen Q-network, robotun olamsı gereken lokasyonu insan hareketi algılama sinir ağlarından elde edilen güvenilirlik skoru ile belirlemektedir. Makaledeki çalışmada robotta engellerin bulunduğu bir harita bilgisinin olduğu kabul edilmektedir.

## 3. Robotic Search and Rescue using Human Detection System - [PDF](PDFs/3_Robotic_Search_and_Rescue_Using_Human_Detection_System.pdf)

https://turcomat.org/index.php/turkbilmat/article/download/1600/1352/2983

Makalede amaç otonom bir robot yapmak değildir. Onun yerine amaç insanların giremediği enkazlara girebilecek uzaktan yönetilebilir bir arama kurtarma robotu yapmak olarak belirlenmiştir. Robot enkaz altında kalan insanları algılamak için PIR sensörü, ultrasonik sensör, gaz sensörü ve mikrodalga sensörü kullanmaktadır. PIR sensörü ile insan sıcaklıkları algılanrken mikrodalga sensörü ile de insan hareketleri algılanmaktadır. Mikrodalga sensörü sadece canlı varlıkların hareketlerini algılayabildiği için enkaz alanında insan bulmada büyük bir fark yaratmaktadır. Robota hareket komutları radyo frekansı ile gitmektedir. Robot üzerinde ayrıca bir kamera bulunmaktadır. Böylece robotu kontrol  eden operator robotu nereye göndereceğini daha iyi anlamaktadır. Robot, sensörlerden gelen bütün verileri bir Raspberry Pi üzerinde toplamaktadır. Ayrıca robotun motor kontrolleri de bu kart üzerinden gerçekleştirilmektedir.

## 4. Duruş ve Hareket Algılama Teknolojileri: Stereo, Uçuş Süresi ve Yapısal Işık Algılayıcılar - [PDF](PDFs/4_Durus_ve_Hareket_Algilama_Teknolojileri_Stereo_Ucus_Suresi_ve_Yapisal_Isik_Algilayicıiar.pdf)

https://dergipark.org.tr/tr/download/article-file/416529

Makale bir değerlendirme makalesidir. Stereo, uçus süresi (time of flight) ve yapısal ışık algılayıcılar ile yapılan duruş ve hareket algılama çalışmalarının bir kısmı incelenmiştir. Bununla beraber stereo kamera, time of flight (ToF) kameralar, yapısal ışık kameraları ve gibrit kameralar hakkında bilgi verilmiştir. Stereo kameralarda iki kamera bulunur ve bu iki kameradan alınan görüntü ile derinlik bilgisi elde etmektedir. ToF kameralar, kameradan çıkan ışınların nesneden geri dönmesi ile derinlik bilgisini hesaplamaktadır. Yapısal ışık kameraları ise kızıl ötesi ışık yayan bir teknolojidir. Kinect de bu kamera tipindedir. Kinect insan iskeletini 20 eklem noktası ile çıkarabilmektedir.Kinect v2 ise  insan iskeletini 25 eklem noktası ile çıkarabilmektedir. Makalede hibrit kamera olarak bahsedilen kameralar Leap Motion kameralardır. İnsan elini 2 kamera ve 3 kızıl ötesi ışık ile 12 eklem parçasına bölerek algılamaktadır. Fakat makalenin asıl amacı belirtilen kameralar ile eğitim, robotik, sağlık ve nesne algılama (cisim tanıma, yüz tanıma, hareket sınıflama, hareket tahmin vb.) alanlarında yapılan çalışmaları incelemektir. Eğitim alanındaki çalışmalarında öğretim amaçlı arttırılmış gerçeklik kullanılmaktadır. Robotik alanındaki çalışmalar daha çok insan hareketine göre mobil robotu hareket ettirme üzerinedir. Sağlık alanındaki çalışmalar vücut parçaları ve vücut şemasındaki bozuklukları algılama üzerinedir.

## 5. Human Activity Recognition for Domestic Robots - [PDF](PDFs/5_Human_Activity_Recognition_for_Domestic_Robots.pdf)

https://www.researchgate.net/publication/258341805_Human_Activity_Recognition_for_Domestic_Robots

https://sci-hub.se/10.1007/978-3-319-07488-7_27

Makalede yapılan çalışmanın amacı robotik teknolojileri kullanarak yaşlı insanlara yardım etmektir. Bu yardımların yapılabilmesi için de insan hareketlerinin algılanabiliyor olması gerekmektedir. Bu çalışmada insan iskeletini çıkarmak için herhangi bir işlem yapılmamaktadır. Kinect aracılığıyla insan iskeleti otomatik olarak elde edilmektedir. (Bu makaleyi çok anlamadım halbuki işin matematiğine kadar inmiş fakat pek anlayamıyorum. Eklem noktalarına ağırlık vermek için HMM based on Gaussian Mixture Model kullanılıyor. Eğitim için ise Dynamic Bayesian Networks kullanılıyor. Ama kafamda oturtamadım bir türlü. Tekrar dönüp bakacağım.)

## 6. Human Activity Recognition Using a Mobile Camera - [PDF](PDFs/6_Human_Activity_Recognition_Using_a_Mobile_Camera.pdf)

https://ieeexplore.ieee.org/abstract/document/6145923

https://sci-hub.se/10.1109/URAI.2011.6145923

Makalede yapılan çalışmanın amacı mobil robot üzerinde bulunan bir kamera ile insan hareketlerinin algılanmasıdır. Bu çalışmada insan hareketleri ayakta durmak, yürümek, oturmak, squat yapmak ve yatmak olacak şekilde sınıflandırılmıştır. İnsan hareketinin algılanabilmesi için ilk olarak insanın algılanması amaçlanmıştır. İnsan algılama algoritması aşağıdaki gibidir:

![alt text](Images/6_1.JPG)

Bir resimden birkaç tane insan olarak algılanabilir özellik Histograms of Oriented Gradients (HOG) özellik çıkarma algoritması ile çıkarılmaktadır. Bu özelliklerin hangisinin insan olduğunu anlamak için Support Vector Machine (SVM) kullanılmıştır. Resimdeki insan algılandıktan sonra iskeletin çıkarılması için star-skeleton yöntemi kullanılmaktadır ve çıkarılan iskeletten elde edilen bilgiler Hidden Markov Model’de kullanılarak insan hareketi belirlenmektedir. İnsan hareketi algılama işlemi aşağıdaki gibi yapılmaktadır:

![alt text](Images/6_2.JPG)

Bu yapılan çalışmalarla beraber insan hareketleri sınıflarını genişletmek için nesne algılma da projeye eklenmiştir. Nesne algılama ile insanın hangi nesneler ile hareketi gerçekleştirdiği belirlenmektedir. Bununla beraber insanın hareketi nerede yaptığı bilgisi de elde edilmektedir. Nesne algılama için SURF özellik çıkarma algoritması kullanılmıştır ve elde edilen özellikler için feature matching işlemi uygulanmıştır. Görüntüdeki insanı belirleme başarısı ortalama %95.33, insan hareketini belirleme başarısı ise ortalama %94.8 olarak tespit edilmiştir.

## 7. Mobile Camera Positioning to Optimize The Observability of Human Activity Recognition Tasks - [PDF](PDFs/7_Mobile_Camera_Positioning_to_Optimize_the_Observability_of_Human_Activity_Recognition_Tasks.pdf)

https://ieeexplore.ieee.org/document/1545599

https://sci-hub.se/10.1109/IROS.2005.1545599

Makalede yapılan çalışmanın amacı mobil kamerayı insan hareketlerini en iyi algılayabilecek şekilde konumlandırmaktır. Burada kameranın en iyi bulunacağı konum, görüntüdeki cismin görünüşünü en üst düzeyde çıkarırken tüm hareket yolunu gözlemleyecek şekilde belirlenmiştir. Bununla beraber kameranın cisme olabildiği kadar yakın olması gerekmektedir. Robotun olması gereken konumu belirlemek için gerekli formüller çıkarılıp Matlab ile simule edilmiştir. Makalede yapılan çalışmada tek kameralı robot (ATRV-JR) kullanılmıştır ve bu robot ileri-geri yürüyen bir insana göre kendini konumlandırmaktadır. Kameradan alınan görüntüler segmentlere ayrılmıştır ve hareket eden cismi arka plandan ayırmıştır. Segmentasyon işlemi için Gaussian Mixture Model tabanlı arka plan ayrıştırma algoritmasıyla beraber Kalman filtresi kullanılmıştır. Elde edilen görüntülerde bulunan cismin pozisyonlarına bakılarak cismin aldığı yol çıkarılmaktadır ve robotun bulunması gereken pozisyon hesaplanmaktadır. Kamera kalibrasyonu yene satranç tahtası görüntüsü yerleştirilerek yapılmıştır. Yapılan denemeler sonucunda izlenebilirlik kalitesinin %61'e kadar arttırıldığı gözlemlenmiştir.

## 8. A Depth Camera-based Human Activity Recognition via Deep Learning Recurrent Neural Network for Health and Social Care Services - [PDF](PDFs/8_A_Depth_Camera-based_Human_Activity_Recognition_via_Deep_Learning_Recurrent_Neural_Network_for_Health_and_Social_Care_Services.pdf)

https://www.sciencedirect.com/science/article/pii/S1877050916322943

Makalede yapılan çalışmanın amacı, daha önce kullanılmamış olan Recurrent Neural Network (RNN) ile insan hareketlerini algılayarak Hidden Markov Model (HMM) ve Deep Belief Network (DBN) ile çıkan sonuçları karşılaştırmaktır. Belirtilen yöntemlerde görüntü almak için derinlik kamerası kullanılmıştır. Derinlik kamerasıyla alınan görüntüde insan vücudu 14 parça ,yani 28 birleşme noktası olarak analiz edilmektedir. RNN'in optimize edilmesi için Adam optimizer kullanılmıştır. Belirtilen RNN Long Short-Term Memory ile birlikte kullanılmıştır. Çalışmada gerçekleştirilen sistem aşağıdaki gibidir:

![alt text](Images/8_1.JPG)

Yapılan denemeler sonucunda HMM ile insan hareketi algılama doğruluğu 4.48 sapma ile %92.49, DBN ile insan hareketi algılama doğruluğu 1.92 sapma ile %97.54, RNN ile insan hareketi algılama doğruluğu 0.11 sapma ile %99.55 olarak gözlemlenmiştir.

## 9. A Multimodal Approach for Human Activity Recognition Based on Skeleton and RGB Data - [PDF](PDFs/9_A_Multimodal_Approach_for_Human_Activity_Recognition_Based_on_Skeleton_and_RGB_Data.pdf)

https://www.sciencedirect.com/science/article/abs/pii/S0167865520300106

https://sci-hub.se/https://doi.org/10.1016/j.patrec.2020.01.010

Makalede yapılan çalışmanın amacı, RGB derinlik kamerasından alınan iskelet ve RGB bilgilerini beraber kullanarak insan hareketlerini algılamaktır. Microsoft Kinect kamerasının iskelet çıkarma özelliği kullanılmıştır. Fakat Kinect'ten alınan iskelet verilerinin %100 doğru olmadığı makalede belirtilmiştir. İskelet verileri Bag of Word (BoW) modeli ile kodlanmıştır. Derinlik kamerasından alınan RGB görüntü serisinin işlenebilmesi için görüntü küçültülmektedir. Görüntü resimde algılanan kişinin omuriliğine göre ortalanarak normal görüntünün %25'i olacak kadar küçültülür. Sonrasında görüntüler ortalarından yatay olarak kesilir. Bununla beraber görüntüler Sobel filtresinden geçirilir. Böylece görüntüler arasındaki farklar daha kolay algılanmaktadır. Anlatılan işlem aşağıdaki gibidir:

![alt text](Images/9_1.JPG)

Burada elde edilen görüntülere de Histograms of Oriented Gradients
(HOG) uygulanır ve elde edilen özelliklere Support Vector Machine (SVM) uygulanır. Bunlar olurken aynı zamanda BoW ile kodlanmış iskelet verisi de Random Forest Classifier'dan geçirilir. Sonrasında bu iki operasyondan elde edilen veriler birleştirilir ve yapılan insan hareketi algılanır. Bahsedilen adımlar aşağıdaki gibidir:

![alt text](Images/9_2.JPG)

## 10. Real-Time Human Action Recognition with a Low-Cost RGB Camera and Mobile Robot Platform - [PDF](PDFs/10_Real-Time_Human_Action_Recognition_with_a_Low-Cost_RGB_Camera_and_Mobile_Robot_Platform.pdf)

https://www.mdpi.com/1424-8220/20/10/2886

Makalede yapılan çalışmanın amacı, OpenPose ve 3D-baseline kütüphanelerini RGB görüntü üzerinde kullanarak elde edilen iskelet bilgisini konvolüsyonel sinir ağı (KSA) modeline vererek insan hareketi algılamaktır. Bu çalışmada elde edilen iskelet bilgisi vektörde tutulmak yerine görüntüye çevrilmiştir ve sonrasında KSA modeline verilmiştir. Yapılan çalışmanın akış şeması genel olarak aşağıdaki gibidir:

![alt text](Images/10_1.JPG)

İskelet çıkarma işleminde 17 tane eklem noktası elde edilmektedir. Bahsedilen iskeleti görüntüye çevirme işlemi iskeleti bir görüntünün üzerine basmak değildir. Bahsedilen eklem noktalarının x, y, z değerlerini görüntünün r, g, b değerlerine atamaktır. Elde edilen bu veriler aşağıdaki KSA modeline verilerek insan hareketi algılanmaktadır:

![alt text](Images/10_2.JPG)

İnsan algılama robot üzerinde bulunan tek RGB kamera ile yapılmaktadır. Burada görüntünün işlenmesi işlemi robotta bulunan NVidia Jetson Xavier kartıyla gerçekleşmektedir. Kullanılan robot ROBOTIS Turtlebot'un robotlarından biridir (Waffle olabilir). Kullanılan veri seti NTU-RGBD'dir. Bu veri setinin, bulunan en büyük Kinect V2 veri seti olduğu makalede belirtilmiştir. Fakat bu veri setinden derinlik bilgisini almak yerine sadece RGB görüntüler alınıştır. Çalışmanın başarı sonuçları accuracy 0.71, precision 0.71 ve recall 0.69 olarak ölçülmüştür. Hatırlamak gerekir ki bu çalışma gerçek zamanlı olarak çalışmıştır elde edilen görüntülerde derinlik bilgisi bulunmamaktadır. 

## 11. A Unified Approach for Patient Activity Recognition in Healthcare Using Depth Camera - [PDF](PDFs/11_A_Unified_Approach_for_Patient_Activity_Recognition_in_Healthcare_Using_Depth_Camera.pdf)

https://ieeexplore.ieee.org/abstract/document/9464951

Makalede yapılan çalışmanın amacı, yeni bir özellik seçim yöntemini insan hareketi algılama işleminde kullanmaktır. Genel olarak insan hareketi algılamanın 3 elementi vardır: segmentasyon, özellik çıkarımı ve seçimi, ve algılama. Bu çalışmada yeni özellik çıkarımı ve seçimi için geliştirilen yönteme dikkat çekilmiştir. Geliştirilen yöntem, görüntü serilerinden sınırlı özniteliklerin toplanmasına odaklanır ve sınıflarını regresyon değerlerine göre ayırt eder. Çalışmada algılanan insan hareketleri koşma, yürüme, zıplama, atlama, tek el sallama, çift el sallama, eğilme, yerinde zıplama, yana doğru hareket etme, alkışlama ve boks yapma olacak şekilde 11'e ayrılmıştır. İnsanı görüntüde segmente etmek için active contour (AC) yönteminin Chan-Vese (CV) tarafından geliştirilmiş versiyonu kullanılmak istenmiştir. Fakat bu yöntem yetersiz kaldığı için nesne farklılıklarını azaltan ve iki alan arasındaki mesafeyi artıran enerji fonksiyonlarının CV'sine Bhattacharyya mesafesinin evrimine dayalı terimleri dahil edilmiştir (Ne demek istendiğini tam anlamadım araştırılacak). Segmentasyon işleminden sonra önerilen özellik çıkarım ve seçimi işleminden elde edilen veriler ile Hidden Markov Model kullanılarak insan hareketi algılanmaktadır. Çalışmanın başarı oranı 2.7 standart sapma ile %97.3 olarak belirlenmiştir.

![alt text](Images/11_1.JPG)

## 12. A Robust Human Activity Recognition Approach Using OpenPose, Motion Features, and Deep Recurrent Neural Network - [PDF](PDFs/12_A_Robust_Human_Activity_Recognition_Approach_Using_OpenPose_Motion_Features_and_Deep_Recurrent_Neural_Network.pdf)

https://link.springer.com/chapter/10.1007/978-3-030-20205-7_25

Makalede yapılan çalışmanın amacı, RGB kamera ile OpenPose kütüphanesi kullanılarak elde edilen iskelet bilgisini Long Short-term Memory (LSTM) hücreli Recurrent Neural Network'e (RNN) vererek insan hareketlerini algılamaktır.

![alt text](Images/12_1.JPG)

Makaleye göre OpenPose kütüphanesi bir insandan 18 iskelet parçası çıkarmaktadır. Fakat bu çalışmada 14,15,16 ve 17 numaralı parçalar (kafa bölgesi) kullanılmamaktadır. Makalede yapılan çalışmada insan hareketlerini algılamak için RNN ile LSTM kullanılmıştır. Makalede RNN'in kısa süreli işlemlerde çok verimli olduğu belirtilmiştir. Fakat uzun süreli işlemler için aynı şey söylenememektedir. Bunu elimine etmek için RNN, LSTM ile beraber kullanılmıştır. Yapılan çalışmalar sonucunda LSTM'in SVM, Decision Tree ve Random Forest sınıflandırma algoritalarından daha iyi iş çıkardığı gözlemlenmiştir.

## 13 Human Activity Recognition by Using Convolutional Neural Network - [PDF](PDFs/13_Human_Activity_Recognition_by_Using_Convolutional_Neural_Network.pdf)

Makalede yapılan çalışmanın amacı, hareket algılamayı daha iyi yapacağı için termal kamera kullanarak konvolüsyonel sinir ağları (CNN) ile insan hareketlerini algılamaktır. Görüntü kameradan alındıktan sonra ilk olarak manuel olarak kesilir. Sonrasında arkaplan çıkarılır ve görüntü threshold edilir. Görüntünün daha iyi sonuç vermesi için görüntü morfolojik işlemlerde geçirilmektedir. Arka plan görüntüsü orjinal görüntüden çıkarılarak insanın olduğu kısım bulunmaktadır ve bu kısım 224x224 büyüklüğündeki bir görüntüye fit edilmektedir. Bütün görüntüler kullanılarak bir ortalama görüntü elde edilir ve bu görüntü farklı filtrelerden geçirilerek 2 farklı görüntü oluşturulur.

![alt text](Images/13_1.JPG)

Bu iki farklı görüntü ve ortalama görüntüsü birleştirilerek aşağıdaki görüntüler oluşur:

![alt text](Images/13_2.JPG)

CNN olarak VGG16-Net mimarisi kullanılmıştır ve doğruluğu %95.9 olarak tespit edilmiştir.