# **OSI(OPEN SYSTEMS INTERCONNECTION) REFERANS MODELİ**

Network alanında öğrendiğimiz bilgilerin yerine oturabilmesi için OSI referans modelini iyi anlamak gerekmekte. Bu yüzden olayların başına 
dönüp "Neden böyle bir modele ihtiyaç duyulmuş?", "Kimler, ne zaman bu yapıyı oluşturmuşlar?" gibi sorulara kısaca değindikten ve tüm "Neden?" lerimizi
ortadan kaldırdıktan sonra "Nedir? ve Nasıl?" sorularımıza geçebiliriz.

OSI modelinden önce networklerin, her bir donanım firmasının kendine özgü olacak şekilde yapısı vardı. Bu networklere o kuruluşun sağladığı donanıma sahip
cihazlar bağlanabiliyorlardı. 

Yani OSI den öncesi için haberleşme demek genellikle "Aynı firmanın donanımına sahip cihazlar"ın yapabildiği bir iletişim demekti. İşte bu nokta OSI referans modeli gibi
bir yapıya ihtiyaç duyulduğu açıktı. Kısıtlı ve seçici haberleşme yapısından sıyrılıp günümüzdeki gibi dünya çapında haberleşebilme için de ISO (The International Standards Organization)
harekete geçti ve 1984 yılında OSI referans modeline son şeklini verdi. 

## **OSI Nedir?**
	 
OSI referans modeli farklı donanımlara sahip cihazların birbirleriyle nasıl haberleşeceklerini belirten yapının bütünüdür. OSI referans modeli dünya üzerindeki tüm cihazlar için
sabit yapıdadır. Network ya da cihaza bağlı olarak farklılık göstermez, standarttır. / adet katmandan oluşur. İki cihaz haberleşirken her bir gerekli adımda(Örneğin veriyi hedefe gönderme, 
verinin görüntülenmesi, verinin işlenmesi, kimlik doğrulaması) belirli protokoller devreye girer. 7 katmanın her birinde bu protokoller rol oynar. Yani haberleşme
baştan aşağı OSI referans modeli esas alınarak protokollerin belirli rolleriyle yapılır.

## **OSI Katmanları**
	
OSI Referans Modelindeki katmanlar bu modeli oluşturan temel elemanlardır. Her bir katmanın diğer katmanlarla ilişkili görevleri bulunur. Ve her katmanda belirli protokoller görev alır. Katmanlar bireysel görevlerini de protokoller üzerinden gerçekler. OSI katmanlarında çeşitli zafiyetler bulunabilir. 

> Yazının devamında daha da içeriğe girmek kaydıyla kısaca OSI katmanlarının görevleri aşağıdaki gibidir:
	 
* ...Layer 7 (UYGULAMA/ APPLICATION) = Uygulamaların, ağları kullanabilmesini sağlayan katmandır. Diğer katmanlardan farklı olarak bir başka katman için hizmet sağlamaz.

* ...Layer 6 (SUNUM/ PRESENTATION)   = Verinin görüntüleneceği cihazda anlaşılabilir formatta olmasını sağlar. Uygulama katmanından gelen veriyi standart bir biçimde sunar. Veri sıkıştırma,
				       veri şifreleme, veri dönüştürme gibi manipulasyonlar gerçekleştirir. Farklı uygulamalar arasında kullanılan ortak verinin anlaşılması açısından çevirmen görevi
				       görür. 

* ...Layer 5 (OTURUM/ SESSION)       = 2 cihaz arasında birbirleriyle haberleşecek uygulamaların arasındaki bağlantıyı başlatır, sürdürür, sonlandırır. Cihazlar arası diyalogları takip eder bu 					       diyaloglar ise session yani oturum olarak da adlandırılabilir. Her diyalog, oturum iletişimde bulunmak istenen cihazları birbirinden ayırt etmeyi sağlar.

* ...Layer 4 (TAŞIMA/ TRANSPORT)     = Layer3 için, Layer4'ten gelen verinin daha verimli işlenmesi için veriyi segmentlere böler; Layer4 için, Layer3'ten aldığı segmentler halindeki veriyi, 					       bütünleşik yapıya dönüştürür. Yani alt ve üstündeki katmanlar arasında bir nevi köprü görevi görür.

* ...Layer 3 (AĞ/ NETWORK)           = Veri iletimi esnasında routerların kullanacağı ,hedef(destination) ve kaynak(source) adresleri gibi, bilgiler eklenir, veri üzerinde bazı işlemler gerçekleşir.

* ...Layer 2 (VERİ İLETİM/ DATA LINK)= Verinin(datanın), çerçeve(frame)ye dönüştürülerek nasıl iletileceği, anlık iletişimin kime ait olduğu ve iletimde hata unsuru olup olmadığı kontrolünü sağlar

* ...Layer 1 (FİZİKSEL/ PHYSICAL)    = Cihazlar arasındaki fiziksel bağlantıyı oluşturur, sürdürür, sonlandırır.
	
