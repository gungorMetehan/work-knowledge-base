# LimeSurvey Anketlerinde Üst Başlıkla Birlikte Soru Sorma

Bazen anketlerde yöneltilen maddeler (sorular) bir üst başlığa (boyuta, faktöre, vb.) sahip olabilir. Bu durumda hem ankette görünsün diye hem de veriyi analiz edecek kişiye bir hatırlatma olması amacıyla bu üst başlıkların da sorular ile birlikte görüntülenmesi istenebilir.
Bu aslında yaygın bir durum da değildir. LimeSurvey bunu bir soru türü olarak da sunmuyor. Ancak basit bir sembol ile bu yapılabilir. Bu farklı soru türlerinde kullanılabilmektedir. Ancak genellikle **Diziler** başlığı altındaki soru türleri için uygundur.

1) İlgili madde (soru) için **Soru türü** kısmından **Diziler** arasından **Dizi** seçilir.

<img width="896" height="685" alt="dizi1" src="https://github.com/user-attachments/assets/266fc1d5-b2b7-4953-8460-e088f10830fe" />

2) Sorunun gövdesi, **Alt sorular** ve **Yanıt Seçenekleri** girildikten sonra, **Alt sorular**'ın girişinde basit bir işlem yapılmalıdır. Burada madde (soru) kökü ile istenen üst başlık arasına `|` sembolü yerleştirildiğinde LimeSurvey bunu bir ayırma aracı olarak görür ve satırdaki maddeyi tam buradan ikiye bölerek yazılı olan iki tarafı aynı satırda farklı sütunlarda gösterir.

<img width="1405" height="747" alt="dizi2" src="https://github.com/user-attachments/assets/8bd85d3c-9293-4896-90bb-890e410dda1b" />

3) **Kaydet** düğmesi tıklandıktan sonra aşağıdaki görünüm elde edilecektir.

<img width="1281" height="398" alt="dizi3" src="https://github.com/user-attachments/assets/1768941f-893b-486c-946d-fb724ddabff6" />
