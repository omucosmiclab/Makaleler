## **UNIX TARİHÇESİ VE ÖNEMİ**

1960'lı yıllarda bilgisayarlar tek kullanıcı ve tek program olarak çalışmaktaydı. Bilim adamları birçok kullanıcının aynı anda bilgisayarları kullanabilesi üzerine düşünmeye başlarlar.(timesharing)

1965'te **MULTICS**(MULtiplexed Information and Computing Service) adını verdikleri projeleriyle düşüncelerini gerçekleştirmek üzere çalışmalara başladılar. MIT, AT&T Bell Laboratuvarları ve GE(General Electric)'nin birlikte çalıştıkları bu projeyle UNIX'in temelleri atılmıştır.

1969'da AT&T Bell Laboratuvarları MULTICS'ten çekilmiştir. Bell çalışanlarının birçoğu (Ken Thompson, Dennis Ritchie, Douglas McIlroy ve J.F Ossanna) vazgeçmedi ve tekrar denemeye karar verdi. Thompson, isimsiz işletim sisteminin ilk sürümünü, bir DEC PDP-7'de **assembly dilinde** yazdı. UNIX işletim sisteminin ilk sürümü **UNICS**(Uniplexed Information and Computing System) ismiyle anılıyordu.
Programın getirdiği kolaylığı yeterli bulmayan, assembly dilinin evrensel olmaması yani makinadan makinaya farklılık göstermesinden dolayı daha gelişmiş bir yöntem bulmak için çalışmalarına devam ettiler.

1972 yılına gelindiğinde, Denis Ritche ve Brian Kernighan C dilini ortaya çıkardılar. 

1973'te çekirdeğinin çoğu **C** dili ile yeniden yazılarak UNIX'in 5. sürümü ortaya çıkmış oldu. Farklı bilgisayar platformlarında taşınabilirlik sağladığı, anlaşılabilir ve değiştirilebilirliği daha kolay olduğu için hızla büyüdü. Öğretim kurumları ve işletmeler tarafından kabul edilir oldu.

1974'te Unix kullanıcıları New York'ta toplandılar. **USENIX** adıyla bilinen günümüzde halen organizasyonlar yapılmakdır.  

1978 yılı Unix 7. sürümüyle gelişimini iki farklı çizgide gerçekteştirecekti: **BSD** ve **System V**.

### **BSD**

Thompson’nun Kaliforniya Üniversitesi’ne misafir öğretim üyesi olarak gitmesiyle birlikte öğrencilerin UNIX’e olan ilgisi daha da artar. İşletim sisteminin kodu üzerinde iyileştirmelere   başlanır. Öğrencilerin çalışmaları sisteme  büyük fayda sağlar.Ortaya vi editörü, Pascal derleyici, C Shell gibi önemli fonksiyonlar çıkarırlar. UNIX’in  1977’den itibaren  Berkeley Software Distribution adı altında yayımlanmaya başlanır. 

[**ARPA**](https://github.com/omucosmiclab/Makaleler/blob/master/Network/A%C4%9F%20Tarih%C3%A7esi.md)(Advanced Research Project Agency), Berkeley'in BSD (Berkeley Software Distribution) isimli projesini geliştirmek ve ARPANET'teki iletişim bozukluklarını da gidermek üzere yeni bir ağ kurmak için büyük bir sözleşme yaptılar. BSD üzerinde çalıştılar ve o kadar iyi çalıştı ki ARPA onu Arpanet araştırmaları için tercih edilen işletim sistemi olarak seçti. Unix, iletişim ağı sayesinde daha da hızla gelişti.


### **System V**

Unix'in ticari olarak devam edebileceğini düşündüğü için lisanslı hale getirdi. Değiştirilen özelliklerile daha güvenilir ve ve güçlü halidir. Birkaç yıl System V ticari olarak en çok desteklenen ürün oldu.Lisans hakkı Unix System Laboratories'e aittir. 


**BSD ve System V üzerinden türetilenler:**

BSD | System V
--- | --- 
Linux | AIX (IBM)
NextStep | IRIX (Silicon Graphics)
(NeXT) | HP-UX (HP)
Sun OS 4.x | Sun OS 5.x/Solaris (SUN)
ULTRIX (DEC) | SCO UNIXware

Günümüzde BSD halen çalışmalarına devam etmektedir. Dağıtımların hepsi Internet'ten özgürce indirilebilir.

* FreeBSD:
Kişisel bilgisayarlara odaklandı
Daha geniş kullanıcıya sahiptir.

* NetBSD:
Taşınabilirlik üzerinde duruldu.
Daha çok platformu destekler

* OpenBSD:
BSD'nin güvenliğini geliştirmeye odaklandı
 

**KAYNAKÇA**
* http://s3.eurecom.fr/~balzarot/softdev/material/0_1_unix_history.pdf
* http://e-bergi.com/y/c-ve-unix-tarihi/
* https://www.tech-worm.com/unix-nedir-unix-tarihi-gelisimi-linuxun-ortaya-cikisi/


Kübra Nur Saruhan