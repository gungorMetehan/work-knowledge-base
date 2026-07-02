# Power BI'daki Gauge Chart'larda Girilen Değere Göre Rengin Değiştirilmesi

Gauge chart'larda bilindiği üzere girilen değere göre bir çeşit ilerleme yüzdesi verilebiliyor. Hatta **Target** kutucuğuna bir değer girilerek bir hedef değer de gösterilebiliyor. Eğer, alınan skora / girilen değere göre ilgili kişinin ilerleme yüzdesini gösteren bar'ın renginin değişmesi isteniyorsa aşağıdaki yol izlenmelidir.

1) Sadece **Visualizations** sekmesindeki **Format Visual**'ın alt menüsündeki **Visual** menüsündeki **Gauge axis** altındaki **Min**, **Max**, **Target**, **Fill color** ve **Target color** değerlerine giriş yapıldığında aşağıdaki gibi bir chart elde edilmektedir.

<img width="462" height="332" alt="gauge1" src="https://github.com/user-attachments/assets/709656cd-3959-48ac-b7aa-b0ddae8e622c" />

2) Yukarıdaki örnek chart için şu şekilde giriş yapılmıştır. Yalnızca 0, 100, 85 değerleri girilmiş ve iki farklı renk seçilmiştir. Biri bar'ın rengini, diğeri de hedefin rengini - çizgi şeklinde - göstermektedir.

<img width="761" height="765" alt="gauge2" src="https://github.com/user-attachments/assets/f4bf11b7-be3e-4973-b8c0-ab1bda3c1cc9" />

3) Burada **Fill color** seçeneğinde seçilen rengin hemen sağında bir **fx** sembolü yer almaktadır. Bu sembol tıklandığında **Fill color - Colors** başlıklı bir pencere açılacaktır. İşte bu kısımdan, kurallarımızı belirleyebiliriz.
Öncelikle **Format style** açılır menüsünden **Rules** seçilmelidir. Ardından kurallar **+ New rule** düğmesi tıklanarak yapılabilir. Bu örnekte yalnızca 0, 75, 75, 90, 90 ve 100 değerleri girilip ilgili aralıklar için üç farklı seçim yapılmıştır. Diğer alanlar otomatik olarak gelmektedir.

<img width="1271" height="719" alt="gauge3" src="https://github.com/user-attachments/assets/e76a7e25-0fbf-4db0-9b25-070990d78f7d" />

4) Tüm ayarlar yapıldıktan ve **OK** düğmesine tıklandıktan sonra aşağıdaki görsel elde edilecektir.

<img width="375" height="283" alt="gauge4" src="https://github.com/user-attachments/assets/95990755-b620-4388-a38e-ce60554cccba" />

Görüldüğü üzere bar'ın rengi değişmiştir. Çünkü ilgili kişiye ait girilen değer olan 80, 75'ten büyük ve 90'dan küçüktür. Ayrıca hedef değer olarak girilen 85 hala gauge chart üzerinde görüntülenebilmektedir.
