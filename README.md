# OMU Cosmic Lab | Ondokuz Mayıs Üniversitesi Siber Güvenlik ve Kriptoloji Laboratuvarı

Bilgi güvenliği ve kriptoloji alanına ilgi duyan insanların faydalanması için oluşturulmuş olan bu depo, makaleleri elinden geldiğince sade bir şekilde yazan gönüllü bir ekip tarafından sürekli güncellenmektedir.

Ekibe katılmak ve projeye katkı sağlamak için aşağıdaki adımları uygulayabilirsiniz.

Projeyi bilgisayarınıza indirmek:
    
    $ git clone https://github.com/omucosmiclab/Makaleler/ cosmiclab

_Depoyu varsayılan olarak Makaleler klasörüne indirecektir. Fakat son parametre olarak 'cosmiclab' yazdığımız için bulunduğunuz dizinde 'cosmiclab' isimli klasöre indirecektir. İsmi kendinize göre düzenleyebilirsiniz._

    $ cd cosmiclab
_Dizine gidip düzenleme yapabilirsiniz. Düzenleme için kullanabileceğiniz onlarca metin editörü bulunmaktadır. VS Code, Atom vs. bunlardan bir kaçıdır. Klasörü metin editörüyle açtıktan sonra size ait klasörü düzenleyin._

Kriptoloji üzerine simetrik algoritmalar ile ilgili bir makale yazacağınızı düşünürsek, Kriptoloji klasörünün altında 'Simetrik Algoritmalar.md' adında bir dosya yaratmalıyız. Daha sonra dosyanın içine araştırmalarımızdan edindiğimiz bilgileri ekleyebiliriz. 

> Önemli not: Bu bilgileri eklerken Markdown formatına uygun olmasına dikkat ediniz. Markdown formatı için [link](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)e tıklayabilirsiniz.


Dosyanızı düzenledikten sonra:

    $ git status

Çıktısında, dosyanızın düzenlenmiş olduğunu görebilirsiniz.

    $ git add .

Komutunu kullanarak düzenlenmiş dosyalarınızı git'in stage area dediği alana ekleyebilirsiniz ve değişikliği kaydetmek için de (commit atmak)

    $ git commit -m "Simetrik algoritmalar makalesi düzenlendi"

şeklinde commit atabilirsiniz. Burada dikkat etmeniz gereken nokta, -m parametresi ile commit yani yaptığınız değişiklik için bir mesaj, açıklama giriyor olmanız. Bu açıklama yaptığınız değişiklik hakkında diğer insanların bilgilenmesi açısından çok önemli.

Commit attığınızda, değişikliği yerel projede yapmış oluyorsunuz. Son adım olarak da:

    $ git push origin master

komutu ile yaptığınız değişiklikleri Github deposuna yani buraya atabilirsiniz.

> Ufak bir not: Eğer büyük bir değişiklik yapacaksanız, -alışkanlık olarak da kullanabilirsiniz- sizin ara verdiğiniz vakitlerde projeye başka insanların katkıda bulunmuş ve bu değişiklikleri Github'a atmış olabileceklerini düşünün. Çalışmaya başlamadan önce işleri sağlama almak için uzak sunucudan deponun en güncel hâlini çekin ve ondan sonra çalışmalara başlayın.

Uzak sunucudan (Github'dan) projenin son hâlini çekmek için:

    $ git pull

komutunu kullanabilirsiniz.

İyi çalışmalar!