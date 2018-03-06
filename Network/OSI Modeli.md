## **OSI(OPEN SYSTEMS INTERCONNECTION) REFERANS MODELİ**

Network alanında öğrendiğimiz bilgilerin yerine oturabilmesi için OSI referans modelini iyi anlamak gerekmekte. Bu yüzden olayların başına 
dönüp "Neden böyle bir modele ihtiyaç duyulmuş?", "Kimler, ne zaman bu yapıyı oluşturmuşlar?" gibi sorulara kısaca değindikten ve tüm "Neden?" lerimizi
ortadan kaldırdıktan sonra "Nedir? ve Nasıl?" sorularımıza geçebiliriz.

OSI modelinden önce networklerin, her bir donanım firmasının kendine özgü olacak şekilde yapısı vardı. Bu networklere o kuruluşun sağladığı donanıma sahip
cihazlar bağlanabiliyorlardı. 

Yani OSI den öncesi için haberleşme demek genellikle "Aynı firmanın donanımına sahip cihazlar"ın yapabildiği bir iletişim demekti. İşte bu nokta OSI referans modeli gibi
bir yapıya ihtiyaç duyulduğu açıktı. Kısıtlı ve seçici haberleşme yapısından sıyrılıp günümüzdeki gibi dünya çapında haberleşebilme için de ISO (The International Standards Organization)
harekete geçti ve 1984 yılında OSI referans modeline son şeklini verdi. 

### **OSI Nedir?**

OSI referans modeli farklı donanımlara sahip cihazların birbirleriyle nasıl haberleşeceklerini belirten yapının bütünüdür. OSI referans modeli dünya üzerindeki tüm cihazlar için
sabit yapıdadır. Network ya da cihaza bağlı olarak farklılık göstermez, standarttır. / adet katmandan oluşur. İki cihaz haberleşirken her bir gerekli adımda(Örneğin veriyi hedefe gönderme, 
verinin görüntülenmesi, verinin işlenmesi, kimlik doğrulaması) belirli protokoller devreye girer. 7 katmanın her birinde bu protokoller rol oynar. Yani haberleşme
baştan aşağı OSI referans modeli esas alınarak protokollerin belirli rolleriyle yapılır.

### **OSI Katmanları**
	
OSI Referans Modelindeki katmanlar bu modeli oluşturan temel elemanlardır. Her bir katmanın diğer katmanlarla ilişkili görevleri bulunur. Ve her katmanda belirli protokoller görev alır. Katmanlar bireysel görevlerini de protokoller üzerinden gerçekler. OSI katmanlarında çeşitli zafiyetler bulunabilir. 

> Yazının devamında daha da içeriğe girmek kaydıyla kısaca OSI katmanlarının görevleri aşağıdaki gibidir:
	 
* Layer 7 (UYGULAMA/ APPLICATION)     = Uygulamaların, ağları kullanabilmesini sağlayan katmandır. Diğer katmanlardan farklı olarak bir başka katman için hizmet sağlamaz.

* Layer 6 (SUNUM/ PRESENTATION)       = Verinin görüntüleneceği cihazda anlaşılabilir formatta olmasını sağlar. Uygulama katmanından gelen veriyi standart bir biçimde sunar. Veri sıkıştırma,
				        veri şifreleme, veri dönüştürme gibi manipulasyonlar gerçekleştirir. Farklı uygulamalar arasında kullanılan ortak verinin anlaşılması açısından çevirmen görevi
				        görür. 

* Layer 5 (OTURUM/ SESSION)           = 2 cihaz arasında birbirleriyle haberleşecek uygulamaların arasındaki bağlantıyı başlatır, sürdürür, sonlandırır. Cihazlar arası diyalogları takip eder bu 					        diyaloglar ise session yani oturum olarak da adlandırılabilir. Her diyalog, oturum iletişimde bulunmak istenen cihazları birbirinden ayırt etmeyi sağlar.

* Layer 4 (TAŞIMA/ TRANSPORT)         = Layer3 için, Layer4'ten gelen verinin daha verimli işlenmesi için veriyi segmentlere böler; Layer4 için, Layer3'ten aldığı segmentler halindeki veriyi, 					bütünleşik yapıya dönüştürür. Yani alt ve üstündeki katmanlar arasında bir nevi köprü görevi görür.

* Layer 3 (AĞ/ NETWORK)               = Veri iletimi esnasında routerların kullanacağı ,hedef(destination) ve kaynak(source) adresleri gibi, bilgiler eklenir, veri üzerinde bazı işlemler gerçekleşir.

* Layer 2 (VERİ BAĞLANTISI/ DATA LINK)= Verinin(datanın), çerçeve(frame)ye dönüştürülerek nasıl iletileceği, anlık iletişimin kime ait olduğu ve iletimde hata unsuru olup olmadığı kontrolünü sağlar

* Layer 1 (FİZİKSEL/ PHYSICAL)        = Cihazlar arasındaki fiziksel bağlantıyı oluşturur, sürdürür, sonlandırır.

 
##### **LAYER 1/ FİZİKSEL KATMAN**

Bilgisayar için her şey 1 ve 0'dır. Gönderilecek veri de 1 ve 0 lar olarak iletilir.  Alıcı tarafta okunan sinyaller 1 ve 0 a dönüştürülürken; gönderici taraf 1 ve 0ları elektrik sinyallerine çevirip kabloya yerleştirir.

Gönderim işleminden önce nasıl(ortam, özellik) gönderileceğine karar verilmelidir
ki işte bu işlemi gerçekleştiren katman fiziksel katmandır. Kablolu bağlantı için kablo türü, kablosuz bağlantı için iletim
kanalı seçimi vb. kararlar bu katmanda verilir.  Bitler, elektrik, radyo sinyalleri, ışık gibi pek çok yolla gönderilebilir. İletimin
gerçekleşmesi açısından önemli unsur ise taşıma ortamıdır. Taşıma ortamı hem alıcı hem gönderici için aynı olmalıdır. Elektriksel yolla
iletilen veri radyo sinyalleri olarak alınırsa iletim düzgün şekilde gerçekleşemez. Taşıma ortamı iletim için tek unsur, tek şart değildir. Voltaj değeri
veri iletim hızı gibi değerlerin de uygun şekilde tanımlanması gerekir.

> PROTOKOLLER: _ISDN, DSL, fiber optik_... 


##### **LAYER 2/ VERİ BAĞLANTISI KATMANI**

Veri bağlantı katmanı 2 bölümden oluşur LLC (Logical Link Control) ve MAC (Media Access Control) genel anlamda bu iki bölümün yaptığı iş gönderilen verinin hatasız bir şekilde iletilip iletilmediği kontrolüdür. Ağ katmanından aldığı veriyi çerçeveler (data framing) ve fiziksel katmana iletir. Bir data frame incelenirse Data (Veri),  Header (Başlık), Trailer (Kuyruk) olmak üzere temel olarak 3 bölümden oluştuğu görülür. İçerikte hedef ve kaynak bilgileri, hata kodunu tutan değer CRC (Cyclic Redundancy Code ), verinin kendisi, başlangıç ve bitişi belirten özel işaret bitleri gibi yapılar vardır. 2. katmandaki çoğu işlem ağ kartı içerisinde gerçekleşir. Alınan, gönderilen data frameler için onaylama bekler. Onaylama alınmayanlar için tekrar gönderim işlemini gerçekleştirir.

LLC ve MAC bölümlerine gelecek olursa üst kısımda LLC alt kısımda MAC bölümü bulunur. LLC Layer 3 ve Layer 2 arasındaki bağlan
tıyı sağlar. Bağlantıda kullanılan protokole (UDP, TCP/IP) uygun erişim noktaları yani mantıksal portlar (Service Access Points, SAPs) oluşturur.
Böylece hedef ve kaynak cihazlar karşılıklı olarak aynı protokoller üzerinden bağlantı gerçekleştirir LLC, bunu verinin çerçeve yapısına (Destination Service Access Point - DSAP, Source Service Access Point - SSAP) ekleyerek sağlar. Bu bilgileri ekledikten sonra veriyi bir alt bölüm olan MAC'e yollar. "Onay alınmayan data frameler tekrar gönderilir"  durumu ise yine LLC'nin sorumlulukları arasındadır. 
Yine akış kontrolü (Flow Control) yani karşı tarafın alabileceği maksimum veri paketi sayısının aşılmamasını sağlayabilmek de LLC'nin görevlerindendir.

MAC bölümü ise adından da anlaşılacağı üzere veri çerçevesine hedef ve kaynak cihazların MAC adresini ekler. Bu fiziksel bağlantıda daha güvenilir iletişimler kurmayı sağlar. Çünkü her bir cihaz için eşsiz MAC adresleri mevcuttur. Yine de bu durumda layer 2 için zaafiyetler bulunmaktadır. (Bunları ayrı olarak daha detaylı incelemenizde fayda var.)
Veri iletimi sırasında bir hata meydana gelirse bunun bilgisi CRC içerisinde tutulur. Hatadan kasıt verinin iletim ortamı içerisinde bozunması olabilir, ya da gönderilen ve alınan verinin aynı olmaması durumu da olabilir.

MAC bölümü, mac adreslerinin yanında bir de işte bu CRC kodunu ekler. Gönderici tarafta veri paketini fiziksel katmana aktarırken; alıcı tarafta veriyi LLC'ye yönlendirir.

Saldırılarda MAC ve ARP ataklarının da önemli bir yeri vardır. MAC ve ARP protokollerine ve bu protokollere değinen saldırılara burada detayıyla yer verilmeyecektir.  Ancak örnek vermek gerekirse MAC Flooding, ARP Poisoning/ARP Spoofing gibi saldırılar katman 2 saldırılarındandır.

> PROTOKOLLER: _MAC, ARP, Ethernet, HDLC_...

	
##### **LAYER 3/ AĞ KATMANI**

Verinin ağ içerisindeki yönlendirimi, akış trafiği bu katmanda yönetilir. Ağ katmanında veri üzerinde bir çok manipulasyon (enkapsülasyon, dekapsülasyon, adresleme, yönlendirme) gerçekleştirilir. 
Ancak amaç verinin en kısa rotadan (routerlar aracılığıyla) alışverişinin yapılmasını sağlamak da denebilir. Ağ katmanında gönderilecek veriler paketlere bölünür; gelen veriler ise üst katmanlar için birleştirilir. 

Taşıma katmanında veriler segmentlere bölünerek ağ katmanına aktarılır. İşte bu segmentlere hedef ve kaynağın adresi (IP adresi) gibi bilgileri içeren 3. katman başlığının eklenmesi  (gönderici tarafta) ile paketler oluşturulur. Bu işleme ise enkapsülasyon denir. Dekapsülasyon ise adından anlaşılacağı üzere enkapsülasyonun tersidir yani alıcı tarafta, veri paketinden 3. katman başlığı atılır ve veri taşıma katmanına yollanır. Peki alıcı ve gönderici taraf ile olan alışverişte günümüz büyük çaplı ağları da düşünecek olursak veri nasıl yolunu buluyor? İşte veriye rotasını gösterme ve doğru adreslere ulaşmasını sağlama, Layer 3 yani ağ katmanının adresleme ve yönlendirme işlemlerinden geçmekte. Enkapsülasyon ile segmentlere hedef ve kaynağın IP adreslerinin eklendiğini söylemiştik. İşte alıcı ve gönderici taraf arasında bulunan ara cihazlar(routerlar) bu adreslere bakar ve kime ait olduğu belli olan veriyi doğru adrese ulaştırır. Bu durum adreslemedir. Ancak alıcı ve gönderici her zaman aynı yerel ağ (Local Network) içerisinde bulunmayabilir. Bu durumda devreye routerlar girmekte. Routerlar adresler yardımıyla veri alışverişinin en optimal rotadan yapılmasını sağlar ve veriyi buna göre yönlendirir.

Yukarıda segmentlere katman 3 başlığı eklendiğini belirtmiştik. Katman 3 başlığı dediğimiz yapı aslında günümüz teknolojisinde kullanılan ve yerini IPv6'ya bırakacağı öngörülen IPv4 başlığıdır.
Bu başlıkta  kaynak adres, hedef adres, yaşam süresi (time to live), protokol, fragment offset, flag (bayrak), versiyon, paket uzunluğu gibi bilgiler bulunur. Bu bilgilerin içeriğine kısaca değinmek gerekirse:
* Kaynak adres: Kaynak cihazın IP adresi
* Hedef adres: Hedef cihazın IP adresi 
* Yaşam süresi: Bir paketin yaşam süresidir. 8 bitlik bir değer taşır. Bu değer her bir routerdan geçiş için 1 azaltılır ve eğer 0 olmuşsa paket atılır. Paket herhangi bir sebepten ötürü doğru adrese ulaşamamış ise sonsuza kadar routerlar arasında dolaşması engellenmiş olur. 
* Protokol: Kullanılan protokolün numarası
* Fragment Offset: Türkçesiyle parça karşılığı denilebilir. Parçalanmış verinin doğru sırayla ulaştırılması için paketlerin sıra değeri
* Flag: İşlenen paketin veriye ait son paket olup olmamasını kontrol etmek içindir. Eğer More Fragment değeri 1 ise işlenecek başka parçalar da olduğu belirtilir. Ancak MF 0 sa ve Fragment Offset 0 dan farklıysa
parçanın son parça olduğu belirtilir. Hem MF hem Fragment Offset 0 ise bu, verinin parçalanmamış olduğunu işaret eder.
* Versiyon: IP versiyon numarasıdır 
* Paket uzunluğu: Başlık dahil verinin bulunduğu paketin boyutudur.

> PROTOKOLLER: _IP, ICMP, ARP, IPV4, IPV6, IGMP_...


##### **LAYER 4/ TAŞIMA KATMANI**

Layer 4 oturum ve uygulama katmanları için standartlaştırılmış erişim sağlar. Yani iletişim ağının özelliklerine göre herhangi bir düzenleme yapılması gerekmez. Böylece üst katmanlar teknolojik 
değişikliklerden izole edilmiş olur. Temel olarak taşıma katmanı, gönderici tarafta üst katmanlardan gelen veriyi parçalar; alıcı tarafta ise gelen veri parçalarının doğru sırayla birleştirilmesi işlemlerinden sorumludur denebilir.  Layer 4te üst katmandan gelen veriler segmentlere dönüştürülür. Segmentler ağ paketi boyutundadır. 

Taşıma katmanı veri akışının kalitesini artırma (QoS = Quality of Service), güvenilirlik, hata kontrolü, zamanında ulaştırma ya da bunun kontrolü, akış denetimi, çoklama gibi işlemler gerçekleştirir. 
Güvenilirlik durumu taşıma katmanında kullanılan protokolle alakalı bir durumdur. Örneğin TCP/IP protokolünde cihazlar arası bir denetim söz konusu iken UDP protokolünde herhangi bir denetim yapılmaz.
Taşıma işlemi, mesajın alıcı taşıma katmanına herhangi bir hata olmadan ulaşmasını sağlamak için uçtan uca gerçekleştirilir eğer hata varsa bu, mesajın yeniden iletilmesi ile düzeltilir.
Çoklama ise aynı ağ üzerinde birden fazla uygulamanın kullanılmasına izin verir. Ayrıca bazı uygulamalar paket yerine direkt baytları kabul eder bu durumda da taşıma katmanı bayt odaklı veri akışını yönetebilir.

> PROTOKOLLER: _TCP/IP, UDP, SCTP, SPX_...


##### **LAYER 5/ OTURUM KATMANI**

Her cihaz tek bir cihaz ile iletişim halindedir diye bir kural yoktur. Yani bir cihaz eş zamanlı olarak birden fazla cihazla haberleşme içinde olabilir. Aynı şekilde bir uygulama da birden fazla uygulama içerisinde olabilir. Katman mantığını anlatmaya çalışırsak; bu durumda cihazlar ve uygulamalar arası iletişimin karışmaması için her bir iletişime birer oturum(session) gözüyle bakılır. Günlük hayattan bir örnekle session mantığını anlamaya çalışalım. Siz bir konuşmacı olarak bir davete katıldınız. Bu konuşmaya bir çok davetlinin geleceğini düşünürsek her birinin
yakakartı bulunmalıdır ki siz de, davetli de o an için kiminle iletişimde olduğunuzu anlayın. Sonuçta A kişisinden almak istediğiniz bilgiyi, B kişisine sormak büyük bir karışıklığa sebebiyet verebilir. 
İşte oturumlar da buna benzer bir mantıktadır. Anlık olarak iletişimde bulunulan her bir uygulama adına bir oturum (session) oluşturulur. Böylece çok iletişimli bir ortam içerisinde büyük bir karışıklık önlenir. Çünkü her bir uygulamanın bir yakakartı gibi oturum kimliği bulunur. Oturum katmanı iki uygulama arasındaki sohbeti yönetir ve senkronize eder, sonlandırır. Eğer senkronizasyon işlemi gerçekleştirilmezse veri kayıpları, iletişimin koparılması gibi sorunlar yaşanabilir. Örneğin karşılıklı haberleşen iki uygulamadan (bunlar A ve B olsun) A, B'ye bir veri yollayacakken B uygulaması sohbeti keserse, bu durumda A uygulamasının yolladığı veri kayıp bir veri olacaktır.

> PROTOKOLLER: _NetBIOS, SAP, Named Pipes, SMB_...


##### **LAYER 6/ SUNUM KATMANI**

Sunum katmanı gönderilecek verinin uygun formatta hazırlanmasını gerçekleştirir. Böylece karşı taraftaki uygulama katmanı bu veriyi kullanabilir. Yani uygulama katmanı için çevirme, dönüştürme işlemi gerçekleştirir. Ayrıca sistemler arasında syntax farklılığı ya da sistemden kaynaklı bit uzunluğu farklılıkları vs. olabilir. Örneğin bir sistem bir harfi 8 bit ASCII olarak kaydederken bir diğeri 16 bit Unicode kullanabilir. İkisi de aynı harfi temsil etmesine rağmen format, uzunluk gibi farklılıkları olabilir. Bu durumda sunuş katmanı 8 ya da 16 bit ile değil direkt o harf ile ilgilenilmesini sağlar. Çünkü uygulamalar arası farklılıklarda tercüman gibi davranır.  

> PROTOKOLLER: _SSL, MIME, TSL, ISO 8822, ISO 8823_...


##### **LAYER 7/ UYGULAMA KATMANI**

Uygulamalar ve ağ arasındaki iletişimi gerçekleştirir Uygulamaların ağ üzerinde çalışmasını ve ağı kullanmalarını sağlar. (Örneğin bir e-mail sunucusunun ağ aracılığıyla e-postaları iletmesi) 
Son kullanıcının hizmetlerini karşılar. Uygulama katmanında iletişimi kuran uygulamanın kendisi değil bu uygulamayı sağlayan hizmettir. Dolayısıyla uygulama katmanını, uygulamalar ve kullanıcı arayüzlerine
hizmet eden üst düzey kurulum hizmeti olarak düşünmek yanlış olmaz. 

> PROTOKOLLER: _HTTP, HTTPS, DNS, FTP, TelNet, SMTP, SSH, SSL, IRC_...


_Yararlanılan Kaynaklar_

* https://studytonight.com
* http://searchnetworking.techtarget.com
* http://bidb.itu.edu.tr
* https://techopedia.com
* https://quora.com

**Burcu SÖYLEMEZ**
