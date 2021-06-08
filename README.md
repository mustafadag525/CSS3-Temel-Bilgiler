
DİV KULLANIMI

![indir](https://user-images.githubusercontent.com/55752233/121259421-c5066380-c8b8-11eb-8ed9-2fa82ee2630a.png)


Div etiketi bir html belgesi içinde bir bölüm belirtmek için kullanılır.div html içinde verileri sağa,sola,yukarı,aşağı css yardımı ile hizalamaya yarar bir kutu olarak düşünülebilir. Metinler ,resimler ve videolar div içinde yerleştirilir.

Daha hızlı sayfa yükleme zamanları : Site div ile tasarlandığında daha az kod teşkil ettiğinden siteler daha hızlı yüklenir. Daha Düşük Barındırma ücretleri : Daha az yüklenme zamanı barındırma ücretleri ve bant genişliğinin az kullanılması demektir ve bunun sonucu barındırma hizmeti aldığımız şirkete daha az ödeme yaparız. Verimlilik : İçerik düzeni stilleri ayrılmış olduğundan, yeniden tasarlama CSS ile çok kolay. Güncelleme için CSS dosyası ve değişiklikleri çok kolaydır. Daha iyi SEO için Daha az kod olması ve kodlama yapısının tablolu yapıya göre daha düzenli olması arama motorlarının indekslemesi için bir avantajdır. Arama motorları(google,yandex...) div ile düzenlenmiş sitelere öncelik verir. Düzenleri ve tasarım gelişmişliği : CSS, HTML tablolara göre tasarımda özgürlük sunmaktadır. Tablolar katı, esnek olmayan, ve ızgara tabanlı iken, CSS tabanlı tasarımlar akışkan, esnek ve genişletilebilir. Takım çalışmalarına daha uygundur : Web sitesi önyüzü ve arka planı ayrımı yapılır. Arayüz geliştirici ve programcı arasında daha kolay ve güzel iletişim sağlanır. iş bölümü olduğu için işler hızlı yürür. Tekrar tasarlama daha ucuzdur farklı tasarımların adapte edilmesi kolaydır. Geleceğe dönük bir yapıdır : HTML5 ile birlikte gelen yeni etiketler ve HTML5’in yapısı div ile kodlamanın devamı niteliğindedir






ID Nedir?

ID ingilizce "Identity" kelimesinin kısaltılmışıdır ve Türkçe "Kimlik" anlamına gelmektedir. Tek bir varlığı tanımlar. Örneğin; hepimizin bir kimlik numarası vardır ve hiçbiri aynı değildir. HTML'de ID, tek bir element için kullanılır. Genellikle header, footer, navbar, sidebar gibi tekrar etmeyen alanları tanımlamak için kullanılır. Her sayfada ortak olarak kullanılan ID olabilir (header, footer, ...) ancak tek sayfada aynı isimde birden fazla ID olmamalıdır. Çünkü hem W3C kurallarına uymaz hem de Javascript kullanacağımız zaman aynı isimde ID varsa karışıklığa yol açar.

document.getElementById("id")
 

Ayrıca bir elemente ID tanımladık varsayalım, aynı sayfanın herhangi yerinde o ID'ye link verilmişse, linke tıklandığında otomatik olarak sayfa tanımlanmış ID'ye kayacaktır. Aşağıda İçeriğe git linkine tıklandığında sayfa, ID'si content olana kayar.

<div id="content">İçerik</div>
<a href="#content">İçeriğe git</a>
 

CSS'de # (diyez) işareti ile kullanılır.

#idismi
{
    position:absolute;
    left:25px;
    top:25px;
    width:150px;
}
 

Class Nedir?

Class'larda ID'lere benzer lakin amaçları farklıdır. ID'nin aksine tek sayfa içerisinde birçok kez tanımlanabilir. Sayfa içerisinde aynı özellikleri taşıyan yerler varsa özellikle yazı stilleri gibi (örneğin; başlıkların aynı renkte ya da boyutta olduğu yerler) Class kullanılmalıdır. Class'lar ID'de olduğu gibi Javascript içinde de olabilir. CSS'de . (nokta) işareti ile kullanılır.

.menu 
{
    font-size:14px;
    color:#ff0000;
}
 

Nerede Class Nerede ID Kullanmalıyım?

Bunu örnekle açıklamak istiyorum. Varsayalım kütüphane açacağız. Öncelikle kitaplarımızı felsefe, psikoloji, polisiye ... gibi kategorilere bölmemiz gerekir ve kütüphanemizde bu kitaplara özel raflar oluşturmalıyız. İşte kitaplara özel oluşturulan bu raflara ID diyoruz. Her kitabın sayfa sayısı, yazı büyüklüğü, ebatları farklıdır. Değişik kitaplar aynı rafta toplanmıştır ve bu işleme de Class diyoruz.

HTML Kodu

<div id="sidemenu">
    <div class="menu">
        <p class="birinci_yazi">Birinci yazı</p>
        <p>İkinci yazı</p>  
        <p>Üçüncü yazı</p>  
    </div>
</div>
 

CSS Kodu

div#sidemenu
{
    position:absolute;
    left:25px;
    top:25px;
    width:150px;
}
div.menu 
{
    font-size:14px;
    color:#ff0000;
    border:2px solid #7FC07F;
}
p.birinci_yazi 
{
    font-size:24px;
    color:#ff0000;
}
