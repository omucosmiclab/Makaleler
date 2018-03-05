## Ağ Cihazları

1. **Hub**

	Temelde kendisine bağlı cihazlara paylaşım yolu sunar ve tüm cihazlar bu yolu kullanır. En basit, aynı zamanda en aptal ağ cihazıdır. Böyle söylenmesinin sebebi, kendisine gelen verinin hangi adrese gideceğinin kontrolünü yapamamasından ve veriyi tüm portlara göndermesinden kaynaklıdır. (Bu noktada kontrolü cihaz yapar, eğer veri kendisine gelmişse kabul eder.) Tek bir veri gönderiminde tüm portlar meşgul olacağından aynı anda birden fazla iletim gerçekleştiremez, diğer iletimler için yolun boşalmasını bekler. Onunla birlikte cihazlar da bekleyeceği için performans düşer, ağ trafiği yoğunlaşır.  

	Sadece veri taşıyıp herhangi bir kontrol yapmadığı için OSI'ın birinci katmanında bulunur.

2. **Switch**
	
	Temel mantığı hub gibi paylaşım yolu sunmaktır. Tek farkı **anahtarlama*** yapmasıdır. Anahtarlama sayesinde iki cihaz haberleşirken diğerleri de kendi aralarında haberleşebilir. Yani ağın boşalmasını beklemeden, ağı ortak kullanabilirler.  

	*Anahtarlama tam olarak nedir? Bir veri gönderildiğinde switch veriyi gönderen cihazın MAC adresini ve verinin gönderildiği kapıyı(portu) adres tablosuna kaydeder. Bir sonraki gönderimde adres tablosundaki bilgiler incelenir ve MAC adresinin bağlı olduğu kapı tespit edilir. Eğer henüz böyle bir kayıt bulunmuyorsa veri, gönderen kapı hariç tüm kapılara gönderilir ve hedef kapı bulunduğunda tabloya kaydedilir.  

	Switch, MAC adresleri ile kontrol yaptığından OSI'ın ikinci katmanında bulunur.

3. **Bridge**

	En az iki, bağımsız, aynı protokolü kullanan ağları birbirine bağlayarak sanki tek bir ağ imiş gibi davranmalarını sağlar. Aynı bridge'e bağlanan farklı ağlardaki cihazlar birbirine veri göndermek isterse bridge verileri inceler ve adreslerini kontrol eder. Adres, karşı ağda bulunuyorsa üzerinden geçmesine izin verir. İşte faydalı olduğu noktası burasıdır. Eğer gönderilecek verinin adresi, bridge'e bağlı diğer ağlardan birinde değilse, yani kendi bulunduğu ağ içerisinde ise trafiğe katılmaz. Böylece performans kazandırmış olur.

4. **Router**

	*TODO*

5. **Gateway**

	*TODO*

6. **Repeater**

	*TODO*

7. **Firewall**

	*TODO*

8. **NIC (Network Interface Card / Ağ Arabirim Kartı)**

	*TODO*

9. **Modem**

	*TODO*
