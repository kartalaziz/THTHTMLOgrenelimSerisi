# HTML Öğrenelim Serisi

# Bölüm 1
Herkese merhaba bu konumuzda W3Schools kaynağının çevirisini yapacağım. Faydalı olması dileğiyle. (Aynı zamanda ben de öğreneceğim, birlikte ilerleyeceğiz.)

## HTML nedir?
- HTML'in açılımı -> Hyper Text Markup Language
- HTML internet sitesi oluşturmak için kullanılan bir standart biçimlendirme dilidir.
- HTML bir internet sitesinin yapısını açıklar.
- HTML bir dizi öğeden oluşur.
- HTML öğeleri, tarayıcıya içeriğin nasıl görüntüleneceğini söyler.
- HTML öğeleri, "bu bir başlıktır", "bu bir paragraftır", "bu bir bağlantıdır" gibi içerik parçalarını etiketler.

## HTML Elementi(Öğesi) nedir?
Bir HTML öğesi bir başlangıç tag'i ile başlar, sonrasında bazı içeriklerle devam eder ve son olarak bitiş tag'i ile bitir.
Örnek verecek olursak: <tagismi> İçerik bla bla.... <tagismi>

HTML öğesi başlangıç tag'inden bitiş tag'ine kadar olan her şeydir:

`<h1> İlk başlığım <h1>`

`<p> ilk paragrafım <p>`

| Başlangıç tag'i  |  İçerik      |    Bitiş tag'i| 
| -------------    | ------------ | --------------|
|    ` <h1>   `    | İlk başlığım |    `    <h1> `|
|   `  <p>     `   |İlk paragrafım|    `    </p> `|
|   `  <br>    `    |     boş     |    `    boş  `|

NOT: Bazı HTML öğeleri içeriğe sahip değildir. ( `<br>` gibi). Bu öğeler boş öğeler olarak adlandırılır. Boş öğeler bitiş tag'ine sahip değildirler.

## İnternet Tarayıcıları

İnternet tarayıcılarının(Chrome, Mozilla, Opera, Brave) amacı HTML dökümanlarını okumak ve bu dökümanların çıktısını doğru şekilde verebilmektir.

Bir tarayıcı HTML etiketlerini görüntülemez, ancak bunları belgenin nasıl görüntüleneceğini belirlemek için kullanır:

Daha açıklayıcı olmasından bir örnek yapalım.

```
<html>

<head><title>Sayfanın Başlığı</title>

</head>

<body><h1>Bu ilk başlığımız</h1>

<p>Buraya içeriğimizi yazıyoruz. Merhaba THT</p>

<p>Yine içerik yazıyoruz. Ben vancoondehni ve bu HTML öğrenme amaçlı oluşturduğum konu</p>

</body>

</html> 
```

Böyle bir kod yazdık diyelim. Bu kodda bir sürü etiket(tag) var değil mi? Peki internet sitesi görünümünde bu tagler görünecek mi? Hemen bakalım:

Bir not defteri açıyorum ve bu kodları not defterine kaydediyorum. Sonrasında not defterinin ismini deneme.html olarak kaydediyorum.

![Çıktı](https://i.hizliresim.com/k0o6wtu.png)

NOT: `<body>` bölümünün içindeki içerik (yukarıdaki beyaz alan) bir tarayıcıda görüntülenecektir. `<title>` öğesinin içindeki içerik, tarayıcının başlık çubuğunda veya sayfa sekmesinde gösterilecektir.

## HTML Dökümanları

- Tüm HTML Dökümanları `<!DOCTYPE html>` ifadesi ile başlamak zorundadır.
- HTML Dökümanının kendisi `<html>` ile başlayıp `<html>` ile biter.
- HTML Dökümanında görülen kısım `<body>` ile `<body>` arasındaki kısımdır.

## `<!DOCTYPE>` Yapısı

`<!DOCTYPE>` yapısı dökümanın türünü belirtmek için kullanılır. Bu yapı tarayıcının, internet sitesini doğru şekilde çıktı vermesi için yardımcı olur.
`<!DOCTYPE>` yapısı fark duyarlılığına sahip değildir.(case sensitive değil) Büyük veya küçük harfle yazılması önemli değil demek oluyor..

`<!DOCTYPE html>`

## HTML Başlıkları

HTML başlıkları `<h1>` ile `<h6>` arasındaki değişkenlerle tanımlanır.

`<h1>` en önemli başlığı temsil ederken, `<h6>`en az değerli olan başlığı temsil eder.
Bir örnekle gösterecek olursak:

```
<html>
<body>

<h1>This is heading 1</h1>

<h2>This is heading 2</h2>

<h3>This is heading 3</h3>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/6rxnzrm.png)

## HTML Paragrafları

HTML paragrafları `<p>` ile tanımlanır.

Örneğin: `<p>Bu bir paragraftır.</p>`

## HTML Linkleri

HTML linkleri `<a>` tag'i ile tanımlanır.

Örneğin: `<a href="https://www.turkhackteam.org/">Bu bir bağlantıdır</a>`

Bu bağlantının varış yeri href eklentisi ile spesifik bir hale getirilmiştir.

## HTML Renkleri

HTML renkleri `<img>` tag'leri ile tanımlanır.

### Bir sitenin HTML Kaynak kodları nasıl görülür?

Bir HTML sitesinde, siteye sağ click ile tıklayın. "Kaynak kodu görüntüle(View source code)" kısmına tıklayın. Sonrasında kaynak kodlar açılacaktır.

## İç içe HTML Öğeleri(Nested HTML Elements)

- HTML öğeleri iç içe yazılabilir.
- Tüm HTML belgeleri iç içe HTML öğelerinden oluşur.

Nasıl yani? Daha açıklayıcı olur musun? Tabi olayım.

```
<html>
<body>

<p>This is a paragraph
<p>This is a paragraph

</body>
</html>

```

Yukarıdaki kodu inceleyelim. `<body>` ifadesinden sonra paragraflar yazdık ve sonrasında `</body>` ifadesiyle kapattık. İşte burada iç içe yazılmış ifadeler var. Buna Nested Elements yani iç içe öğeler diyoruz.

## Boş HTML Öğeleri
İçeriği boş olan HTML öğelerine boş HTML öğeleri diyoruz.

`<br>` tag'i bir satır boşluk bırakır.

`<br>` boş bir öğe olduğu için bitiş tag'ine ihtiyaç yoktur.

Örnek verecek olursak:

```
<html>
<body>
<p>Bu <br> boşluk bulunduran bir paragraftır.</p>
</body>
</html>

```
![Çıktı](https://i.hizliresim.com/hes0tsg.png)

## HTML Büyük/Küçük Harfe Duyarlı Değildir
- HTML etiketleri büyük/küçük harfe duyarlı değildir: `<P>` `<p>` ile aynı anlama gelir.

- Küçük veya büyük harfle yazmanız bir şeyi değiştirmez fakat W3C kodların küçük harfle yazılması taraftarıdır. Alışkanlık olarak küçük harfle yazmanız daha yararlı olacaktır.

## HTML Özellikleri
- HTML özellikleri, HTML öğeleri(element) hakkında ek bilgi sağlar.
- Tüm HTML öğelerinin özellikleri olabilir.
- Özellikler her zaman başlangıç etiketinde belirtilir
- Özellikler genellikle ad/değer çiftleri halinde gelir. Örneğin: name="value

### href Özelliği
`<a>` etiketi bir hyperlink'i tanımlar. href özelliği, bağlantının gittiği sayfanın URL'sini belirtir:

Örnek verecek olursak: `<a href="https://www.turkhackteam.org">TurkHackTeam'i Ziyaret Et</a>`

### src Özelliği
`<img>` etiketi, bir HTML sayfasına bir resim gömmek için kullanılır. src özelliği, görüntülenecek görüntünün yolunu belirtir:

Örnek verecek olursak: `<img src="img_girl.jpg">`

URL'yi src özelliğinde belirtmenin iki yolu vardır:

1. Mutlak URL(Absolute URL) - Başka bir web sitesinde barındırılan harici bir resme bağlantılar. 

Örnek: ` src="https://www.w3schools.com/images/img_girl.jpg" `

Notlar: Harici görseller telif hakkı kapsamında olabilir. Kullanmak için izin almazsanız, telif hakkı yasalarını ihlal ediyor olabilirsiniz. Ayrıca, harici görüntüleri kontrol edemezsiniz; aniden kaldırılabilir veya değiştirilebilir.

2. Göreceli URL(Relative URL) - Web sitesinde barındırılan bir resme bağlantılıdır. Burada URL, alan adını içermez. URL eğik çizgi olmadan başlıyorsa, geçerli sayfaya göre olacaktır.

Örnek: `src="img_girl.jpg"`

URL bir eğik çizgi ile başlıyorsa, etki alanına göre olacaktır.

Örnek: `src="/images/img_girl.jpg"`

Öneri: Göreli URL'leri kullanmak neredeyse her zaman en iyisidir. Etki alanını değiştirirseniz bozulmazlar.

### widht ve height Özellikleri

`<img>` etiketi görüntünün genişliğini ve yüksekliğini (piksel olarak) belirten widht ve height özelliklerini de içermelidir.

Örnek verecek olursak: `<img src="img_girl.jpg" width="500" height="600">`

### alt Özelliği
`<img>` etiketi için gerekli alt özelliği, resim herhangi bir nedenle görüntülenemiyorsa, resim için alternatif bir metin belirtir. Bunun nedeni, yavaş bağlantı veya src özelliğindeki bir hata ya da kullanıcının bir ekran okuyucu kullanması olabilir.

Örnek: `<img src="img_girl.jpg" alt="Girl with a jacket">`

### style Özelliği
style özelliği, bir öğeye renk, yazı tipi(font), boyut gibi stiller eklemek için kullanılır.

Örnek: `<p style="color:red;">Bu kırmızı bir paragraftır.</p>`

### lang Özelliği
Web sayfasının dilini bildirmek için her zaman `<html>` etiketinin içine lang özelliğinizi eklemelisiniz. Bu, arama motorlarına ve tarayıcılara yardımcı olmak içindir.

Örnek:

```
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```
### title Özelliği
title özelliği, bir öğe hakkında bazı ek bilgileri tanımlar.( Daha açıklayıcı olursak sss ifadesini tıklanabilir yani başka sayfaya gönderebilir bir hale getirir.)

title özelliğinin değeri, fareyi öğenin üzerine getirdiğinizde bir araç ipucu olarak görüntülenecektir.

Örnek: `<p title="I'm a tooltip">Bu bir paragraftır.</p>`

## 1. Bölüm Özeti 
- Tüm HTML öğelerinin özellikleri olabilir
- `<a>` öğesinin href özelliği, bağlantının gittiği sayfanın URL'sini belirtir.
- `<img>` öğesinin src özelliği, görüntülenecek görüntünün yolunu belirtir.
- `<img>` öğesinin `width` ve `height` özellikleri, görüntüler için boyut bilgisi sağlar.
- `<img>` öğesinin alt özelliği, bir resim için alternatif bir metin sağlar.
- style özelliği, bir öğeye renk, yazı tipi, boyut ve daha fazlası gibi stiller eklemek için kullanılır.
- `<html>` etiketinin `lang` özelliği, Web sayfasının dilini bildirir.
- `title` özelliği, bir öğe hakkında bazı ek bilgileri tanımlar.

# Bölüm 2

## HTML Başlıkları
- HTML başlıkları `<h1>, <h2>, <h3>, <h4>, <h5>, <h6>` tag'leri ile ifade edilir. `<h1>` en büyük başlıktır ve en önemli içeriği temsil eder. `<h6>` ise en az değerli olan başlıktır.
- Tarayıcılar başlıklardan sonra otomatik olarak bir satır boşluk bırakır.
- Başlıklar önemlidir. Arama motorları sayfaların yapısı hakkında bilgi edinirken başlıklara da dikkat eder.

Bir örnekle gösterelim:
```
<html>

<body>

<h1>Başlık 1</h1>

<h2>Başlık 2</h2>

<h3>Başlık3</h3>

<h4>Başlık4</h4>

<h5>Başlık 5</h5>

<h6>Başlık 6</h6>

</body>

</html>
```
![Çıktı](https://i.hizliresim.com/i7i6mbc.png)

Her bir HTML başlığı default büyüklüğe sahiptir. style özelliğini kullanarak bu büyüklüğü değiştirebilirsiniz.

## HTML Paragrafları

- HTML'de paragraflar `<p>` tag'i ile tanımlanır.
- Bir paragraf her zaman yeni bir satırla başlar ve tarayıcılar otomatik olarak paragrafın önüne ve arkasına biraz boşluk bırakırlar.
- `<hr>` tag'i, bir HTML sayfasında tematik bir mola tanımlar.
- `<hr>` öğesi, bir HTML sayfasındaki içeriği ayırmak (veya bir değişikliği tanımlamak) için kullanılır.

Örnek:
```
<html>

<body>

<h1>Bu başlık 1</h1>

<p>merhaba ben vancoondehni</p>

<hr>

<h2>Bu başlık 2</h2>

<p>Green Team</p>

<hr>

</body>

</html>
```
![Çıktı](https://i.hizliresim.com/aaoihja.png)

`<hr>` tag'i boş bir tagdir. Yani bitiş tag'i yoktur.

## HTML Satır Sonları

- `<br>` tag'i bir satır sonunu tanımlar.
- Yeni bir paragraf başlatmadan bir satır sonu (yeni bir satır) istiyorsanız `<br>` kullanılır.
- `<br>` boş bir tag'dir yani bitiş tag'i bulunmaz.

Örnek:
```
<html>

<body>

<p>Bu<br>bir paragraftır<br>Bu paragrafta satır sonu bulunuyor.</p>

</body>

</html>
```

## HTML `<pre>` Elementi(Öğesi)

- HTML `<pre>`öğesi, önceden biçimlendirilmiş metni tanımlar.

- `<pre>` öğesinin içindeki metin sabit genişlikli bir yazı tipinde (genellikle Courier) görüntülenir ve hem boşlukları hem de satır sonlarını korur.

Örnek:
```
<html>
<body>
<pre>
Selam.

Ben.

Vancoondehni.

#GreenTeam.
</pre>
</body>
</html>
```
![Çıktı](https://i.hizliresim.com/4qcx8y6.png)

## HTML Style

style özelliği bir öğeye renk, font, yazı boyutu gibi özellikleri eklemek için kullanılır.

Bir HTML öğesinin stilini ayarlamak, style özelliği ile yapılabilir.

HTML stili özelliği aşağıdaki sözdizimine sahiptir.

Örnek: `<tagname style="property:value;">`

propery bir CSS özelliğidir. value ise bir CSS değeridir.

### Arka plan rengi
CSS arka plan rengi özelliği, bir HTML öğesinin arka plan rengini tanımlar.
```
<html>
<body style="background-color:powderblue;">

<h1>Bu bir başlıktır. Selam THT</h1>
<p>Bu bir paragraftır. #GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/aris46d.png)

### Metin Rengi
CSS color özelliği, bir HTML öğesinin metin rengini tanımlar.
```
<html>
<body style="background-color:powderblue;">

<h1 style="color:blue;">Bu bir başlıktır. Selam THT</h1>
<p style="color:green;">Bu bir paragraftır. #GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/mcs2vkc.png)

### Font(Yazı Tipi)
CSS `font-family` özelliği, bir HTML öğesi için kullanılacak yazı tipini tanımlar.
```
<html>
<body style="background-color:powderblue;">

<h1 style="font-family:verdana;">Bu bir başlıktır. Selam THT</h1>
<p  style="font-family:courier;" >Bu bir paragraftır. #GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/it7k68q.png)

### Metin Boyutu(Text Size)
CSS `font-size` özelliği, bir HTML öğesinin metin boyutunu tanımlar.
```
<html>
<body style="background-color:green;">

<h1 style="font-size:300%;">Bu bir başlıktır. Selam THT</h1>
<p  style="font-size:160%;">Bu bir paragraftır. #GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/eqmoren.png)

### Metin Hizalama
CSS `text-align` özelliği, bir HTML öğesi için yatay metin hizalamasını tanımlar.
```
<html>
<body style="background-color:orange;">

<h1 style="text-align:center;">Bu bir başlıktır. Selam THT</h1>
<p  style="text-align:center;">Bu bir paragraftır. #GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/tvcqlps.png)

# Bölüm 3

## HTML Metin Formatları
`<b>` - Bold text(kalın metin)
`<strong>` - Important text(önemli metin)
`<i>` - Italic text(italik metin)
`<em>` - Emphasized text(vurgulanmış metin)
`<mark>` - Marked text(işaretlenmiş metin)
`<small>` - Smaller text(daha küçük metin)
`<del>` - Deleted text(silinmiş metin)
`<ins>` - Inserted text(eklenen metin)
`<sub>` - Subscript text(alt simge metni)
`<sup>` - Superscript text(üst simge metni)`

Yukarıdaki formatların hepsini içeren bir örnek:
```
<html>

<body>
<p> Green Team - vancoondehni - Aziz </p>
<p> <b>    Bold text(kalın metin) </b>
    <em> Emphasized text(vurgulanmış metin) </em>
    <i>     Italic text(italik metin)</i>
    <small>    Smaller text(daha küçük metin) </small>
    <strong> Important text(önemli metin) </strong>
    <sub>    Subscript text(alt simge metni) </sub>
    <sup>    Superscript text(üst simge metni) </sup>
    <ins>     Inserted text(eklenen metin) </ins>
    <del>     Deleted text(silinmiş metin) </del>
    <mark>   Marked text(işaretlenmiş metin) </mark>


    </p>

</body>

</html>
```
![Çıktı](https://i.hizliresim.com/j1iahpw.png)

## HTML Alıntı ve Alıntı Öğeleri
Bu bölümde `<blockquote>,<q>, <abbr>, <address>, <cite>, <bdo> `elemanlarına değineceğiz.

### HTML Alıntıları için `<blockquote>`
HTML `<blockquote>` öğesi, başka bir kaynaktan alıntılanan bir bölümü tanımlar.
```
<html>

<body>

    <p>THT'den bir alıntı:</p>
    <blockquote cite="https://www.turkhackteam.org/">
    2002 yılında kurulan THT Türkiye'nin en büyük siber güvenlik forumudur.
    </blockquote>

</body>

</html>
```
![Çıktı](https://i.hizliresim.com/3k0ct4b.png)

### HTML'de Kısa Alıntılar için `<q>`
HTML `<q>` etiketi kısa bir alıntıyı tanımlar.

Tarayıcılar normalde alıntının etrafına tırnak işaretleri ekler.
```
<html>

<body>

    <p>Green Team'in hedefi: <q>Kaliteli eğitici içerikler üretmek.</q></p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/a68w8kv.png)

### HTML'de Kısaltmalar için `<abbr>`
HTML `<abbr>` etiketi, "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM" gibi bir kısaltma veya kısaltma tanımlar.

Kısaltmaları işaretlemek, tarayıcılara, çeviri sistemlerine ve arama motorlarına faydalı bilgiler verebilir.
```
<html>

<body>

    <p> #GreenTeam içeriği - <abbr title="Türk Hack Team">THT</abbr> 2002 yılında kurulmuştur.</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/qi5mysh.png)

### İletişim Bilgileri için HTML `<address>`
HTML `<address>` etiketi, bir belgenin veya makalenin yazarı/sahibi için iletişim bilgilerini tanımlar.

İletişim bilgileri bir e-posta adresi, URL, fiziksel adres, telefon numarası, sosyal medya tanıtıcısı vb. olabilir.
`<address>` öğesindeki metin genellikle italik olarak işlenir ve tarayıcılar her zaman <address> öğesinden önce ve sonra bir satır sonu ekler.
```
<html>

<body>

    <p> Merhaba ben vancoondehni</p>
    <address>
        Written by vancoondehni<br>
        Visit us at:"https://www.turkhackteam.org/"<br>
        TR
        </address>

</body>

</html>
```
![Çıktı](https://i.hizliresim.com/3wcynud.png)

### HTML'de İş Başlığı için <cite>
HTML `<cite>` etiketi, yaratıcı bir çalışmanın (ör. kitap, şiir, şarkı, film, resim, heykel vb.) başlığını tanımlar.

Not: Bir kişinin adı bir eserin başlığı değildir.

`<cite>` öğesindeki metin genellikle italik olarak işlenir.
```
<html>

<body>

    <p><cite>Gülpembe</cite> 1991 yılında Barış Manço tarafından çıkartılmış bir şarkıdır.</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/hghlfla.png)

### HTML'de Çift Yönlü Geçersiz Kılma için `<bdo>`
BDO, Çift Yönlü Geçersiz Kılma anlamına gelir.

Geçerli metin yönünü geçersiz kılmak için HTML `<bdo>` etiketi kullanılır.
```
<html>

<body>

    <bdo dir="rtl">Bu metin sağdan sola doğru yazılacaktır.</bdo>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/5do4h2b.png)

## HTML'de Yorumlar
HTML yorumları tarayıcıda görüntülenmez, ancak HTML kaynak kodunuzu açıklayarak yazmanıza yardımcı olabilirler.

Aşağıdaki şekilde bir kullanımla yorum satırınızı HTML içeriğinize gizleyebilirsiniz.

<!-- Yorumunuzu buraya yazınız. -->

Dikkat: Başlangıç etiketinde bir ünlem işareti (!) olduğuna, ancak bitiş etiketinde bulunmadığına dikkat edin.
```
<html>

<body>

    <!-- Bu bir yorumdur. -->

<p>Bu bir paragraftır. Selam THT</p>

<!-- Buraya daha fazla bilgi eklemeyi unutma -->


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/pjmk92h.png)
### İçerik Saklamak
Yorumlar içerik saklamak için kullanılabilir.

Geçici olarak içerik saklamak çok işe yarayabilir.

<!-- blablabla --> etiketi ile birden çok satırı saklayabilirsiniz.
```
<html>

<body>

    <p>Bu bir paragraftır..</p>
    <!--
    <p>Şu güzel resime bak:</p>
    <img border="0" src="pic_trulli.jpg" alt="Trulli">
    -->
    <p>Bu da bir paragrafır.</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/l1mjc7o.png)

### Satır İçi İçeriği Gizleme
Yorumlar, HTML kodunun ortasındaki bölümleri gizlemek için kullanılabilir.
```
<html>

<body>

    <p> Merhaba <!-- Green Team --> ben vancoondehni</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/mjsc126.png)

# Bölüm 4

