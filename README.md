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

Bir resimden birkaç tane insan olarak algılanabilir özellik HOG özellik çıkarma algoritması ile çıkarılmaktadır. Bu özelliklerin hangisinin insan olduğunu anlamak için Support Vector Machine (SVM) kullanılmıştır. Resimdeki insan algılandıktan sonra iskeletin çıkarılması için star-skeleton yöntemi kullanılmaktadır ve çıkarılan iskeletten elde edilen bilgiler Hidden Markov Model’de kullanılarak insan hareketi belirlenmektedir. İnsan hareketi algılama işlemi aşağıdaki gibi yapılmaktadır:

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

Makalede yapılan çalışmanın amacı, RGB derinlik kamerasından alınan iskelet ve RGB bilgilerini beraber kullanarak insan hareketlerini algılamaktır. Microsoft Kinect kamerasının 

## 10. Real-Time Human Action Recognition with a Low-Cost RGB Camera and Mobile Robot Platform - [PDF](PDFs/10_Real-Time_Human_Action_Recognition_with_a_Low-Cost_RGB_Camera_and_Mobile_Robot_Platform.pdf)

https://www.mdpi.com/1424-8220/20/10/2886

