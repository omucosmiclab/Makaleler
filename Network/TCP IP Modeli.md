# TCP/IP

## TCP/IP’nin Tarihçesi
 
İnternetin tarihsel ve teknik standartları TCP/IP referans modelidir. Bu model Birleşik Devletler savunma bölümü tarafından üretilmiş bir modeldir. Tasarlanışının nedeni ise nükleer savaş dâhil her türlü şartta sürekli ayakta durabilen bir ağ yapısının istenmesiydi. Birleşik Devletler savunma bölümü, dünya üzerinde bulunan bakır kablo, mikrodalga, optik kablo ve uydu hattı kullanan farklı iletişim medyaları ile her şartta haberleşmeyi sağlayabilmek istiyordu. Bu şartlar TCP/IP modelinin tasarısını oldukça güçleştirdi.
 
TCP/IP protokol grubu, 1970’lerin ortasında, Stanford Üniversitesi ve Bolt Beranek ve Newman (BB&N) tarafından geliştirilmiştir. Geliştirme, DoD’in DARPA bölümü tarafından desteklenmiştir. DARPA, ARPANET adı verilen ve devlet kuruluşları, üniversiteler ve araştırma kurumlarını paket anahtarlamalı ağlarla birbirine bağlama projesi üzerinde çalışmıştır. TCP/IP protokol grubu bu amaca yönelik olarak geliştirilmiştir.
 
1978-1979’larda TCP/IP protokol grubunun büyük bir kısmı tamamlanmış ve DARPA, 1980’lerde Internet protokolünü ARPANET birimlerine yüklemeye ve kullanmaya başlamıştır. 1983 yılının Ocak ayında, DARPA, ARPANET’ e bağlanan tüm ağların internet kullanmasını zorunlu tutmuştur. İnternetin büyümesi ve kullanımı ile, ARPANET, küçük paket anahtarlamalı ağlardan, noktadan-noktaya telefon bağlantılarla hibrit ağlara dönüşmüştür. ARPANET terimi kullanılmaya devam etmektedir ve DoD’nin araştırma ve geliştirme amacı ile internetin bir parçası olarak uygulanmaktadır. IAB adındaki bir organizasyon, şu anda internet araştırmalarını organize etmektedir. IAB, DARPA tarafından kurulan ve internet araştırmalarını teşvik etmeye yönelik bir kuruluştur. Her IAB grubu, internet konularının bir parçası üzerinde çalışır. Bu çalışmaların sonuçları, çoğunlukla internetin işlevsel bir parçası hâline gelir.
 
Şu anda internet üzerinde çalışan birçok protokol ve uygulama, RFC adı verilen bir dizi makale ile belgelenir. RFC kitaplığının bakımı ve jüriliği yapma görevi, Menio Park, California’da bulunan SRI Network Information Center (NIC) tarafından yürütülür. İnternet protokolünü konu alan her dokümanda, Unix BSD ve internet protokol birleşmesinin önemi vurgulanır. 1982’de, Unix BSD işletim sistemi üniversitelerin bilgisayar bölümlerinde çok popüler olan bir işletim sistemiydi. Ağ standardı olarak interneti kabul etmiştir. Unix BSD/internet birleşimi, her ikisinin de popülaritesini arttırmış ve bu durum günümüze kadar devam etmiştir. Amerika Birleşik Devletleri, kendisinin denetimi altında bulunan internet protokolü parçasının OSI referans modeli ile uyumlu olması için GOSIP  ile değiştirilmesini istemiştir. Buna rağmen TCP/IP’nin ticari kullanımı büyüyerek devam etmiştir.

## TCP/IP Nedir?
Açılımı Transmission Control Protocol/Internet Protokol olan TCP/IP internetin temel protollerini içeren bir pakettir. TCP/IP protokolü diye adlandırmak çok doğru değildir. Çünkü TCP/IP çok sayıda protokol ve yardımcı programlardan oluşan bir protokol kümesidir. TCP kısmı veri transfrerinde önemli noklataları belirtirken IP kısmı taşıma yolunu bulmayı belirtir; en çok kullanılan iki protokolün ismi verilmiştir.

Bir bilgisayar ağında kullanılan protokol ne olursa olsun, aslında bilgisayarlar fiziksel adresleri ile birbirlerini tanır ve iletişimde bulunurlar. Bu fiziksel adres ağ kartı veya ağa bağlanmayı sağlayan herhangi bir donanımın içinde hiçbir şekilde değiştirilmesi mümkün olmayan 48 bit uzunluğundaki bir numaradır. TCP/IP protokolünde diğer bilgisayarlardan farklı olarak her bilgisayar bir IP numarası alır. İnternet’te bulunan her bilgisayarın kendine ait bir IP numarası vardır ve sadece ona aittir. IPv4 adresleri 32 bit uzunluğundadır ve kolay okunabilmeleri için 8 bitlik 4 gruba ayrılmışlardır. İnternet üzerinde veri alışverişi yapan alıcı ve göndericiyi tanımlamaktadırlar.

TCP/IP, OSİ modeli* gibi katmanlardan oluşur diyebiliriz. Temel olarak 4 katmanda 15’ten fazla protokol vardır. Veriler bu katmanlar arasında sırasıyla paketlenerek gönderilir, alıcıda ise paketlemenin tersi sırayla teker teker açılarak veri ulaştırılmış olur.

## TCP/IP Katmanları

### Uygulama Katmanı:
En üst seviye katmandır. Bu katmanda gönderilecek veri tipi ve veriyi işleyen uygulamalar bulunur. TFTP,FTP,SMTP;SNMP protokollerini barındırır.

### Taşıma katmanı:
Bu katmanda verinin nasıl gönderileceği belirlenir. Veri güvenliği, hata kontrolü gibi işlemler yapılır. TCP ve UDP bu katmandadır.

### Ağ katmanı: 
IP katmanı olarak da adlandırılan bu katman da verilerin gideceği adres veriye eklenir yani veri bu katmandan gönderilir ve yönlendirilir. IPv4 ün gelecekte yetersiz kalma durumuna karşı IPv6 sistemine geçmek için çalışmalar başlatılmıştır.IPv4 32 bit iken IPv6 ile 128 bitlik adresler kullanılacak. Bu sayede daha fazla cihaza IP adresi atanabilecek. IP, ICMP, ARP, RARP, DHCP, BOOTP protokollerini barındırır.

### Fiziksel katman:
Bu katman verinin hangi yolla gönderileceği belirlenir. İletişim ortamının özelliklerini, haberleşme hızını ve kodlama şemasını belirler. Ethernet, Wi-Fi, Token Ring, ATM gibi protokoller bu katmanda çalışır.


*OSI Modeli için https://github.com/omucosmiclab/Makaleler/blob/master/Network/OSI%20Modeli.md ziyaret edebilirsiniz


***Binnaz DEMİRÇEVİREN




