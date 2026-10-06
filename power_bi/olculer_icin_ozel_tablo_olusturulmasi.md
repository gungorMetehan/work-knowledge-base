# Power BI'da Ölçüler İçin Özel Tablo Oluşturulması

Power BI'da yeni bir ölçü (measure) oluşturulduğunda, hangi tablonun altında çalışılmakta ise oluşturulan ölçü de o tablonun altında yer alıyor. Ancak ölçüler hangi tablo altında olursa olsun aynı şekilde çalışan yapılar. Çoğu zaman da tek bir tablodan beslenerek oluşturulmuş olmak zorunda değiller.
Bu nedenle, oluşturulan bir ölçünün sanki tek bir tablonun içindeki bir elemanmış gibi durması yerine sadece ölçülere özel bir tablo oluşturularak, tüm ölçülerin bunun altına alınması daha mantıklı olabilir. Bu Data alanında daha şık bir görüntünün yanı sıra daha düzenli bir yapı da sağlar. Aşağıda, yeni ölçülerin oluşturularak tamamen kendilerine özel bir tablonun / klasörün altına alınması görseller ile birlikte açıklanmıştır.

1) Öncelikle yeni ölçü oluşturulmalıdır. Yeni ölçü Power BI'da pek çok yerden oluşturulabilir. Buradaki örnekte *memnuniyet* isimli tablo ile çalışılırken menüdeki **Modeling** sekmesi tıklanarak **New Measure** seçeneği seçilmiştir. Ardından kodlar yazılarak **Enter** tuşuna basılmıştır.
Bu durumda, kodlarda bir sorun yok ise yeni ölçü, doğrudan hangi tablo üzerinde kalındı ise o tablonun altına oluşturulmuş olacaktır. Bu nedenle **Memnuniyet Seviyesi** ölçüsü **memnuniyet** tablosunun altındadır.

<img width="1912" height="992" alt="yeniolcu1" src="https://github.com/user-attachments/assets/c5313804-cd2d-4ba6-9d6c-9a037561d9f9" />

2) Oluşturulmuş olan ölçüyü, bir klasörün / tablonun altına alabilmek için içi boş bir tablo oluşturulmalıdır. Bunun için menüdeki **Home** sekmesinden **Enter Data** seçilir. Bu aslında, sıfırdan veri girişi yapmak için kullanılan bir kısımdır.
**Enter Data** denildiğinde ekrana bir **Create Table** penceresi açılacaktır. Bu pencerenin içinde hiçbir işlem yapmadan doğrudan ölçülerimize özel oluşturacağımız tablonun adını girerek **Load** tıklanır. Bu örnekte tablonun adının **Olculer** olması sağlanmıştır.

<img width="1914" height="998" alt="yeniolcu2" src="https://github.com/user-attachments/assets/99c40b44-33f3-40d8-a284-b8df9baea9b5" />

3) Tablo oluşturulduğunda **Data** penceresinde en altta içi boş **Olculer** tablosu oluşacaktır. Bu tablonun hemen solundaki sembol de bunun bir tablo olduğunu göstermektedir.

<img width="443" height="437" alt="yeniolcu3" src="https://github.com/user-attachments/assets/d94c04c4-b654-4c12-85f6-a558912847ae" />

4) **Olculer** isimli tablonun içine / altına almak istediğimiz ölçümüzün (measure) üzerine gelip tıkladıktan sonra otomatik olarak **Measure Tools** açılır. Burada ölçü ile ilgili çeşitli ayarlamalar yapılmaktadır. Buradaki **Home table** kısmında yeni ölçünün istenilen bir tablonun altına alınabildiği görüntülenebilir.
Burada artık yeni oluşturulan **Olculer** tablosu da yer almaktadır.

<img width="1917" height="977" alt="yeniolcu4" src="https://github.com/user-attachments/assets/c1596d05-3f87-42aa-91b8-7582e1a7e2d6" />

5) İlgili işlem gerçekleştirildiğinde, yeni ölçünün **Olculer** tablosunun altına geçtiği görüntülenebilecektir.

<img width="189" height="391" alt="yeniolcu5" src="https://github.com/user-attachments/assets/05905e3a-903a-4e95-9bd0-1298fcbc96d7" />

6) **Olculer** tablosunun altında bir de **Column1** isimli bir sütunun varlığı görünmektedir. Bu, en başta tablo oluştururken mecburi olarak oluşan sütun. Bir ölçü olmadığı ve ölçüler ile ilgili tablonun altında bulunması gerekmediği için yanındaki ... işaretine tıklayarak **Delete from model** denebilir.

<img width="182" height="732" alt="yeniolcu6" src="https://github.com/user-attachments/assets/d962ee18-ddce-48f8-b3a6-a33f7b8a7415" />

7) Bu gereksiz sütun silindiğinde eş zamanlı olarak bir şey gerçekleşir: Sadece ölçülere özgü hazırlanan boş tablonun yanındaki sembol değişir. Artık bir tablo sembolü yerine, bir hesap makinesi sembolü belirir burada. Hatta bu hesap makinesi sembolü de üretilmiş bir ölçünün solundaki hesap makinesi sembolünden farklıdır.
Kısacası, bundan sonra .pbix dosyasında hazırlanacak olan tüm ölçüler bu yeni tablonun / klasörün altında aynı şekilde alınabilir.

<img width="181" height="353" alt="yeniolcu7" src="https://github.com/user-attachments/assets/5488d6ad-9040-4150-a4d1-0b5ead2a6426" />
