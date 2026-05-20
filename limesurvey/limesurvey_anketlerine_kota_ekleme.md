# LimeSurvey Anketlerine Kota Ekleme

LimeSurvey’de bir anket / form hazırlanırken bazen bazı maddeler (sorular) için kota gerekebilmektedir. 
İş dünyasından birkaç örnek: Bir eğitime belirli sayıda katılımcı başvurabilsin istendiğinde, Bir pozisyona sadece belirli sayıda çalışan başvurabilsin istendiğinde, Bir eğitim programının her grubuna eşit ve belirli sayıda katılımcı başvurabilsin istendiğinde.
Yukarıda bahsi geçen kurgular için LimeSurvey’in ‘Kotalar’ kısmından yararlanılabilir. Bunun için:

1)	Anketin / formun soruları hazırlanır.
2)	Kota konusunda sorun çıkmaması adına ilgili sorunun ‘tek yanıtlı’ bir madde türünde olması gerekmektedir. Aksi halde kota sistemi doğru işlemeyecektir. Benim önerim: **Liste (radyo)**.
3)	Şu sıra takip edilir: **Yapı > Soru Ekle > Soru türü > Bir seçimli sorular > Liste (radyo) > Genel ayarlar > Zorunlu (Açık)**
4)	Soru gövdesi ve seçenekleri hazırlandıktan sonra kaydedilir.
5)	**Anket menüsü > Kotalar**
6)	**Kota ekle > Kota adı** (Bir isim veriniz), **Sınır** (İlgili yanıtı kaç kişi verebilir en fazla nümerik olarak yazınız) ve **Kota iletisi** (Kontenjan dolduğunda yanıtlayıcı hangi metni görsün istiyorsanız onu giriniz. Aksi halde sistemde otomatik bir ileti mevcuttur) alanları doldurulur.
7)	Bu işlemler yapıldığında **Anket menüsü > Kotalar** yolunun altında artık bir kutucuk belirmiş olacaktır. Burada Yanıt ekle denmelidir. Ardından ilgili soru ve ilgili seçenek seçilmelidir.
8)	Bu aşamada ilk yanıt seçildikten sonra devam edilmemeli. Aynı sorunun diğer yanıtı için tekrar **Yanıt ekle** denerek yeni bir kota oluşturulmalıdır. Örneğin 4 farklı grup, liste (radyo) sorunun altında seçilebiliyorsa, 4 farklı kota olmalıdır. Her bir grubun da 2 katılımcı hakkı olduğunu varsayalım. Bu durumda anketi ilk 8 kişinin yanıtlaması gerekmektedir. İşte bu kurgu için 4 kere aynı soruya ikişer kişilik kota eklenmelidir.
9)	Kotaların eklenme işi bittikten sonra tüm kotaların solunda yer alan kutucuklar işaretlenmeli, ardından **Seçilmiş kotalar… > Etkinleştir** denmelidir.
10)	**Önemli:** Katılımcıların anketi birden fazla yanıtlayamaması önemlidir genelde bu kurguda. Bu nedenle son olarak **Yayınlama ve erişim** kısmından **Çift katılımları önlemek için tanımlama bilgileri kullanılsın > Açık** seçilmelidir.

Aşağıdaki örnek şunu göstermektedir:
Bir anket / form hazırlanmış. Kişilerden katılacakları grupları seçmeleri istenmiştir. Tek bir soruda 4 gruptan yalnızca bir tanesinin seçilmesi mümkündür (Görüntüde yalnızca iki farklı seçenek görülmektedir). **Sınır** yani kota olarak her grup için 2 seçilmiştir. Veriler toplanmıştır ve ilk iki grup dolmuştur. Çünkü **Tamamlandı** sütununun altında yine 2 yazmaktadır.

<img width="1885" height="843" alt="limesurvey_kotalar" src="https://github.com/user-attachments/assets/436c8730-6652-4d7c-a51c-88318ccbbd8c" />

Verilerin toplanması sırasında bir sorun ile karşılaşıldığı durumda, **Yanıtlar** kısmından mükerrer satırlar silindiğinde, silinen satır kadar kotanın hatalı şekilde dolmasının önüne geçilmiş olacaktır.
