## Ağ Cihazları

1. **Repeater**

	Bir portuna gelen sinyali, çok zayıflatmadan ya da bozmadan iletebileceği maksimum uzaklığa kadar aynı ağ üzerinde yineleyerek diğer portuna aktarır. Unutulmaması gereken nokta, repeater yaptığı işin, yani sinyali zayıflattığının farkındadır. Eğer sinyal üzerinde bir bozma yaparsa sinyali bit cinsinden kaydeder ve orijinal gücünde yeniden üretir. 2 portludur.  

	Yaptığı iş ek bir kontrol gerektirmediğinden OSI'ın birinci katmanında bulunur.

2. **Hub**

	Temelde bir repeater türündendir. Ancak birden fazla porta sahiptir ve kendisine bağlı cihazlara paylaşım yolu sunar. Tüm cihazlar bu yolu kullanır. En aptal ağ cihazıdır. Böyle söylenmesinin sebebi, kendisine gelen verinin hangi adrese gideceğinin kontrolünü yapamamasından ve veriyi tüm portlara göndermesinden kaynaklıdır. (Bu noktada kontrolü cihaz yapar, eğer veri kendisine gelmişse kabul eder.) Tek bir veri gönderiminde tüm portlar meşgul olacağından aynı anda birden fazla iletim gerçekleştiremez, diğer iletimler için yolun boşalmasını bekler. Onunla birlikte cihazlar da bekleyeceği için performans düşer, ağ trafiği yoğunlaşır.  

	Sadece veri taşıyıp herhangi bir kontrol yapmadığı için OSI'ın birinci katmanında bulunur.


3. **Switch**
	
	Temel mantığı hub gibi paylaşım yolu sunmaktır. Tek farkı **anahtarlama*** yapmasıdır. Anahtarlama sayesinde iki cihaz haberleşirken diğerleri de kendi aralarında haberleşebilir. Yani ağın boşalmasını beklemeden, ağı ortak kullanabilirler.  

	*Anahtarlama tam olarak nedir? Bir veri gönderildiğinde switch veriyi gönderen cihazın MAC adresini ve verinin gönderildiği kapıyı(portu) adres tablosuna kaydeder. Bir sonraki gönderimde adres tablosundaki bilgiler incelenir ve MAC adresinin bağlı olduğu kapı tespit edilir. Eğer henüz böyle bir kayıt bulunmuyorsa veri, gönderen kapı hariç tüm kapılara gönderilir ve hedef kapı bulunduğunda tabloya kaydedilir.  

	Switch, MAC adresleri ile kontrol yaptığından OSI'ın ikinci katmanında bulunur.

4. **NIC (Network Interface Card / Ağ Arabirim Kartı)**

	Bilgisayarın ağa bağlanmasını, bir başka bilgisayar ile ağ kurmasını sağlayan karttır. MAC adresi ile de desteklendiğinden ağdaki bilgisayarların OSI'ın birinci ve ikinci katmanına ait aygıtlarmış gibi iletişim kurmalarına imkan sağlar. Aynı zamanda protokol kontrol yazılımına da sahiptir. 

3. **Bridge**

	Hub ve Switch yardımıyla aynı ağdaki bilgisayarları birbirleri ile haberleştirebiliyorduk. Ancak bunları kullanarak iki farklı ağın birbirleri ile haberleşmesini mümkün kılamayız. Bu işlevi gerçekleştirmek için kullanılabilecek cihazlardan birisi bridge idir. Sinyal yelpazesini genişletebilen bir repeater gibi de düşünülebilir.  

	En az iki, bağımsız, aynı protokolü kullanan ağları birbirine bağlayarak sanki tek bir ağ imiş gibi davranmalarını sağlar. Aynı bridge'e bağlanan farklı ağlardaki cihazlar birbirine veri göndermek isterse bridge verileri inceler ve adreslerini kontrol eder. Adres, karşı ağda bulunuyorsa üzerinden geçmesine izin verir. İşte faydalı olduğu noktası burasıdır. Eğer gönderilecek verinin adresi, bridge'e bağlı diğer ağlardan birinde değilse, yani kendi bulunduğu ağ içerisinde ise trafiğe katılmaz. Böylece performans kazandırmış olur.  

	İnceleme işleminde MAC adreslerine göre filtreleme yaptığından OSI'ın ikinci katmanında bulunur.

6. **Router**

	Router, veri paketlerini switch benzeri bir anahtarlama yöntemi ile yönlendiren ağ cihazıdır. Ancak bu anahtarlamayı bilgisayarların MAC adreslerine göre değil, IP adreslerine göre yapar. Peki bu noktada bridge'den farkı nedir? Router, çok büyük-karmaşık ağları birbirine bağlayabilir, trafiği sınırlandırabilir ve veriyi aktarırken seçilecek en iyi yola karar verebilir. Aynı zamanda bridge gibi iki ağı birbirine bağlamak için aynı protokolü kullanmaları şartına gerek duymaz. Ancak ağların benzer teknolojileri kullanmalarını bekler.  

	IP adresleriyle işlem yaptığından OSI'ın üçüncü katmanında bulunur.

7. **Gateway**

	Router ve bridge gibi iki farklı ağı birbirine bağlayarak trafiğin düzenlenmesinde görev alır. Ancak onlara göre çok daha gelişmiş bir cihazdır. Farklı protıkolleri kullanan ağların yanında farklı teknolojileri kullanan ağlarında birbirleriyle haberleşmesini sağlar. Bunu kendi içerisinde birtakım dönüşümler ile gerçekleştirir.  

	Peki bu farklı teknoloji dediğimiz şey tam olarak nedir? Örneğin; ATM teknolojisine sahip bir ağ ile Ethernet teknolojisine sahip bir ağ, gateway sayesinde haberleşebilir.  

	Dönüşümleri yaparken IP adreslerini kullandığı için OSI'ın üçüncü katmanında yer alır.

8. **Modem**

	Modemler, gatewayler gibi kendi içlerinde dönüşüm yapmaktadırlar. Bilgisayardan gelen dijital sinyalleri, ev telefonlarının analog sinyallerine çevirir (Veri gönderirken bu işlemi yaparken veri alma sırasında tersi işlem yapar.) ve bu sayede bilgisayar internete çıkabilir. Unutulmaması gereken nokta, evimize bir modem bağlandığında 1 adet IP adresi verilir. Yani modem ile yalnızca tek bir cihaz internete çıkabilir. Birden fazla cihazı internete çıkartmak için, yönlendirme yapan diğer ağ cihazlarından destek alınır ve bu sayede verilen IP adresi bölüştürülür.

9. **Access Point**

	*TODO*

10. **Firewall**

	*TODO*
