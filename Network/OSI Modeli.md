## **OSI(OPEN SYSTEMS INTERCONNECTION) REFERANS MODELİ**

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

	Yazının devamında daha da içeriğe girmek kaydıyla kısaca OSI katmanlarının görevleri aşağıdaki gibidir:
	 
	* Layer 7 (UYGULAMA/ APPLICATION) = 
	* Layer 6 (SUNUM/ PRESENTATION)   =
	* Layer 5 (OTURUM/ SESSION)       =
	* Layer 4 (TAŞIMA/ TRANSPORT)     =
	* Layer 3 (AĞ/ NETWORK)           =
	* Layer 2 (VERİ İLETİM/ DATA LINK)=
	* Layer 1 (FİZİKSEL/ PHYSICAL)    =
	
