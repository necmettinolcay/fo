#   Danışmansız Öğrenme

.fx: first

Abdullah Yaprak `110-----`

Necmettin Olcay Özer `11060296`


Mart 2015

---

##  Danışmansız Öğrenme

-   Sistemin öğrenmesine yardımcı olacak bir öğretmen yok

-   Ağa sadece girdi değerleri verilir

-   Ağın ulaşması gereken hedef çıktılar verilmez.

-   Girişe verilen örnekten elde edilen çıkış bilgisine göre ağ sınıflandırma kurallarını kendi kendine geliştirir

##  Danışmansız Öğrenme

-   Sınıflandırma problemlerinde yaygın olarak kullanılır

-   Sistemin öğrenmesi bittikten sonra çıktıların ne anlama geldiğini gösteren etiketlendirmenin kullanıcı tarafından yapılması gerekmektedir

##  Danışmansız Öğrenme

![](media/fil.jpg)

##  Danışmansız Öğrenme

-   Sistemin doğru çıkış hakkında bilgisi yok

-   Girişlere göre kendi kendini örnekler

-   Ağ bağlantı ağırlıklarını aynı desenler oluşturmak üzere ayarlar

##  Danışmansız Öğrenme

-   Bu öğrenmede gizli sinirler görev yaparlar

-   Dışardan herhangi bir yardım alınmaz

-   Kendini örgütlemek için bir yol bulmak zorundadır.

-   Yani ağ __yaparak__ öğrenmek zorundadır


##  Danışmansız Öğrenme

Danışmansız öğrenme ile

-   SOM(Self Organizing Map) 

-   ART(Adaptive Resonance Theory)

ağları geliştirilmiştir

##  Yarışmacı Öğrenme

-   Amaç n boyutlu bir vektörü bir vektörler setine haritalamaktır

-   Yani bir vektörün belirli bir sayıda vektör ile gösterimi amaçlanmaktadır

-   Öğrenme ile de girdi vektörünün hangi vektör seti tarafından temsil edildiğinin öğrenilmesi kastedilmektedir

-   Genel olarak sınıflandırma problemlerinde kullanılır

##  Yarişmacı Öğrenme


![](media/cmptv.png)


##  Yarışmacı Öğrenme

-   Eğitim sırasında girdilerin sınıflara ayrılması en yakın komşuluk kuralına göre gerçekleştirilir.

-  Girdi vektörü ile referans vektörleri arasındaki en kısa mesafe aranmaktadır

-  Girdi vektörü kendisine en yakın mesafede bulunan vektör grubuna aittir

-  Ağın ağırlıkları değiştirilerek girdileri doğru sınıflara ayıracak referans vektörler belirlenmektedir.

##  Yarişmacı Öğrenme

-  Girdi katmanı ile yarışma katmanı tam bağlantılıdır

-  Girdi katmanı ile yarışma katmanı arasındaki ağırlıklar değiştirilir

-  İstenilen duruma göre çıkışla ilgili işlemler yapılır

##  Yarışmacı Öğrenme

-  Öğrenme kuralı yarışma katmanındaki her proses elemanının bir biriyle yarışması ilkesine dayanır

-  Yarışma girdi vektörü ile ağırlık vektörleri(referans vektör) arasındaki öklid mesafesinin hesaplanmasına dayanır

-  Ağırlık vektörü girdi vektörüne en yakın olan proses elemanı yarışmayı yazanır

##  Yarışmacı Öğrenme


-  i. proses elemanının mesafesi aşağıdaki gibi hesaplanır

![](media/euclid.gif)

-  Girdi vektörü X

-  Referans (Ağırlık) vektörü A

-  Aralarındaki mesafe d

##  Yarişmacı Öğrenme

-  Bütün mesafeler hesaplandıktan sonra en yakın olan kazanandır

-  `Ağırlıklar öğrenme kuralına göre değiştirilir`

-  Ağırlıklar girdi vektörüne biraz daha yaklaştırılır

![](media/weight.gif)

-  Veya uzaklaştırılır

![](media/weight2.gif)
   
##  Özörgütlemeli Harita Ağı

-   SOM(Self-organizing map)

-   Kohonen tarafından geliştirilmiştir

-   Genellikle sınıflandırma yapmak için kullanılır

-  `Girdi vektörlerini ve girdi vektörlerinin dağılımını` öğrenebilme yetenekleri yüksektir

##  Özörgütlemeli Harita Ağı

-   Yarışmacı öğrenimle eğitilir 

-   Girdi ve çıktı olmak üzer 2 katmandan oluşur

-   Çıktı katmanı 2 boyutlu düzlemi göstermektedir

-   Proses elemanları bu düzlem üzerine dağılmış vektörleri gösterirler

![](media/som1.png)
##  Özörgütlemeli Hatita Ağı

-   SOM ağları yarışmayı kazanma ve kazanan elemanın 1 diğer elamanların 0 değerini alması ilkesine dayanır.

-   Bir girdi verildiğinde çıktı uzayında yarışmayı kazanan ve onun etrafındaki komşuların ağırlıkları değiştirilir

![](media/som2.jpg)

##  Özörgütlemeli Harita Ağı

Algoritma
:   Özgörgütlemeli haritalama algoritması

    -   0-) Ağırlık katsayılarına ilk deger ata

    -   Topolojik komşuluk parametrelerini belirle

    -   Öğrenme katsayısını belirle


##  Özörgütlemeli Harita Ağı

Algoritma
:   Özörgütlemeli haritalama algoritması

    -   1-)Bitiş şartı yanlışken adım 2-8 tekrarlanır
    
    -   2-) Her bir x giriş vektörü için adım 3-5 tekrarlanır

    -   3-) Her bir i,j için oklid uzaklık değerlerini hesapla

    -   4-) Hesaplanan bu uzaklık değerlerinden en küçüğünü bul
    
##  Özörgütlemeli Harita Ağı

Algoritma
:   Özörgütlemeli haritalama algoritması

    -   5-) Bulunan bu proses elemanının ve komşularının ağırlıklarını güncelle
    -   6-) Öğrenm kaysayısını güncelle
   
    -   7-) Topolojik komşuluk parametresini azalt
   
    -   8-) Bitiş şartını kontol et

##  Özörgütlemeli Harita Ağı

Algoritma
:   Özörgütlemeli haritalama algoritması

    -   7-) Topolojik komşuluk parametresini azalt
   
    -   8-) Bitiş şartını kontol et
