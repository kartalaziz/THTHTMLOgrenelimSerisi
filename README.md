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

## HTML'de Renkler
HTML renkleri, önceden tanımlanmış renk adlarıyla veya RGB, HEX, HSL, RGBA veya HSLA değerleriyle belirtilir.

### Renklerin İsimleri
HTML'de, bir renk adı kullanılarak bir renk belirtilebilir.

HTML 140 farklı rengi desteklemektedir. Bu listeye bağlantıdan ulaşabilirsiniz.
![Renkler](https://www.w3schools.com/colors/colors_names.asp)

### Arka plan Rengi
HTML öğeleri için arka plan rengini ayarlayabilirsiniz.
```
<html>

<body>

    <h1 style="background-color:DodgerBlue;">HTML Öğrenelim 4</h1>
    <p style="background-color:Tomato;"> #GreenTeam</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/ud1c21c.png)

### Metin Rengi
Metnin rengini ayarlayabilirsiniz.

```
<html>

<body>

    <h1 style="color:Tomato;">Merhaba THT</h1>
    <p style="color:DodgerBlue;">Ben vancoondehni</p>
    <p style="color:MediumSeaGreen;">#GreenTeam</p>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/bity5ll.png)

### Sınır Rengi
Kenarlıkların rengini ayarlayabilirsiniz.
```
<html>

<body>

    <h1 style="border:2px solid Tomato;">Merhaba</h1>
<h1 style="border:2px solid DodgerBlue;">THT</h1>
<h1 style="border:2px solid Violet;">Beraberce HTML Öğrenelim</h1>


</body>

</html>
```
![Çıktı](https://i.hizliresim.com/u6zm14b.png)


### Renk Değerleri
HTML'de renkler RGB değerleri, HEX değerleri, HSL değerleri, RGBA değerleri ve HSLA değerleri kullanılarak da belirlenebilir.

### HTML RGB ve RGBA Renkleri
Bir RGB renk değeri KIRMIZI, YEŞİL ve MAVİ ışık kaynaklarını temsil eder.

RGBA renk değeri, RGB'nin Alfa kanalına (opaklığa) sahip bir uzantısıdır.


### RGB Renk Değerleri
HTML'de bir renk, şu formül kullanılarak RGB değeri olarak belirtilebilir:

rgb (kırmızı, yeşil, mavi)

Her parametre (kırmızı, yeşil ve mavi), rengin yoğunluğunu 0 ile 255 arasında bir değerle tanımlar.

Bu, 256 x 256 x 256 = 16777216 olası renk olduğu anlamına gelir!

Örneğin, rgb(255, 0, 0) kırmızı olarak görüntülenir, çünkü kırmızı en yüksek değerine (255) ve diğer ikisi (yeşil ve mavi) 0'a ayarlanmıştır.

Başka bir örnek, rgb(0, 255, 0) yeşil olarak görüntülenir, çünkü yeşil en yüksek değerine (255) ve diğer ikisi (kırmızı ve mavi) 0'a ayarlanmıştır.

Siyahı görüntülemek için, tüm renk parametrelerini şu şekilde 0'a ayarlayın: rgb(0, 0, 0).

Beyazı görüntülemek için, tüm renk parametrelerini şu şekilde 255'e ayarlayın: rgb(255, 255, 255).

![Çıktı](https://i.hizliresim.com/n1z4vjy.png)

### Grinin Tonları

Gri tonları genellikle üç parametrenin tümü için eşit değerler kullanılarak tanımlanır.
![Çıktı](https://i.hizliresim.com/mn8wxin.png)

### RGBA Renk Değerleri
RGBA renk değerleri, bir rengin opaklığını belirten Alfa kanalıyla RGB renk değerlerinin bir uzantısıdır.

Bir RGBA renk değeri şu şekilde belirtilir:

rgba(kırmızı, yeşil, mavi, alfa)

Alfa parametresi, 0.0 (tamamen şeffaf) ile 1.0 (hiç şeffaf değil) arasında bir sayıdır.

![Çıktı](https://i.hizliresim.com/lawnyqo.png)

### HTML HEX Renkleri
Onaltılık bir renk şu şekilde belirtilir: #RRGGBB, burada RR (kırmızı), GG (yeşil) ve BB (mavi) onaltılık tam sayılar rengin bileşenlerini belirtir.

### HEX Renk Değerleri
HTML'de, onaltılık formda bir değer kullanılarak bir renk belirtilebilir:

#rrggbb

Burada rr (kırmızı), gg (yeşil) ve bb (mavi), 00 ve ff arasındaki onaltılık değerlerdir (ondalık 0-255 ile aynı).

Örneğin, kırmızı en yüksek değerine (ff) ve diğer ikisi (yeşil ve mavi) 00'a ayarlandığından #ff0000 kırmızı olarak görüntülenir.

Başka bir örnek, #00ff00 yeşil olarak görüntülenir, çünkü yeşil en yüksek değerine (ff) ve diğer ikisi (kırmızı ve mavi) 00'a ayarlanmıştır.

Siyahı görüntülemek için tüm renk parametrelerini 00'a ayarlayın, bunun gibi: #000000.

Beyazı görüntülemek için tüm renk parametrelerini şu şekilde ff olarak ayarlayın: #ffffff.

![Çıktı](https://i.hizliresim.com/ij9hdoh.png)

### Grinin Tonları
Gri tonları genellikle üç parametrenin tümü için eşit değerler kullanılarak tanımlanır.

![Çıktı](https://i.hizliresim.com/3wt7dq3.png)

### HTML HSL ve HSLA Renkleri

HSL, ton, doygunluk ve hafiflik anlamına gelir.

HSLA renk değerleri, Alfa kanalı (opaklık) ile HSL'nin bir uzantısıdır.

### HSL Renk Değerleri

HTML'de bir renk, şu şekilde ton, doygunluk ve açıklık (HSL) kullanılarak belirtilebilir:

hsl(ton, doygunluk, hafiflik)

Ton, renk tekerleğinde 0 ile 360 arasındaki bir derecedir. 0 kırmızı, 120 yeşil ve 240 mavidir.

Doygunluk bir yüzde değeridir, %0 bir gri tonu anlamına gelir ve %100 tam renktir.

Açıklık da bir yüzde değeridir, %0 siyahtır ve %100 beyazdır.

![Çıktı](https://i.hizliresim.com/a4cnk7a.png)

### Doyma(Satürasyon)
Doygunluk, bir rengin yoğunluğu olarak tanımlanabilir.

%100 saf renktir, gri tonları yoktur.

%50, %50 gridir, ancak yine de rengi görebilirsiniz.

%0 tamamen gri, artık rengi göremezsiniz.

![Çıktı](https://i.hizliresim.com/pkqlqxv.png)

### Açıklık
Bir rengin açıklığı, renge ne kadar ışık vermek istediğiniz olarak tanımlanabilir, burada %0 ışık yok (siyah), %50 %50 ışık (ne karanlık ne açık) anlamına gelir %100 tam açıklık (beyaz) anlamına gelir.

![Çıktı](https://i.hizliresim.com/nyy7kww.png)

### Grinin Tonları
Gri tonları genellikle ton ve doygunluk 0'a ayarlanarak ve daha koyu/daha açık gölgeler elde etmek için açıklığı %0'dan %100'e ayarlayarak tanımlanır.

![Çıktı](https://i.hizliresim.com/eipshea.png)

# Bölüm 5

## HTML Stilleri - CSS
CSS'in açılımı Cascading Style Sheets'dir.
CSS çok fazla iş tasarrufu sağlar. Aynı anda birden fazla websitesinin düzenini kontrol edebilir.

### CSS nedir?
CSS website düzenini biçimlendirmek için kullanılır.
CSS ile birlikte rengi, yazı tipini, yazı boyutunu, elementler arasındaki boşluğu ve elementlerin pozisyonunu, arka plandaki görseli ve ekran boyutunu ayarlayabilirsiniz.

#### CSS'i Kullanmak
HTML dökümanlarına 3 şekilde CSS'i ekleyebilirsiniz:
1 - Inline(Satır içi) - HTML öğelerinin içindeki style özelliğini kullanarak
2 - Internal(Dahili) - `<head>` bölümünde bir `<style>` özelliğini kullanarak
3 - External(Harici) - harici bir CSS dosyasına bağlanmak için bir `<link>` özelliğini kullanarak
CSS'i eklemenin en yaygın yolu, stilleri external(harici) CSS dosyalarının dışında tutmaktır.

## Satır İçi(Inline) CSS

Tek bir HTML öğesine benzersiz bir still uygulamak için satır içi(Inline) CSS kullanılır.

Satır içi(Inline) CSS, bir HTML öğesinin style özelliği kullanır.

Aşağıdaki örnek, `<h1>` öğesinin rengini maviye ve `<p>` öğesinin rengini kırmızıya ayarlar:
```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;">Mavi bir başlık.</h1>

<p style="color:red;">Kırmızı bir paragraf</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/2nltp4t.png)

## Dahili(Internal) CSS

Tek bir HTML sayfası için bir still tanımlamak için dahili(Internal) bir CSS kullanılır.

Bir HTML sayfasının <head> bölümünde, bir `<style>` elementi içinde dahili bir CSS tanımlanır.
Aşağıdaki örnek, tüm `<h1>` öğelerinin metin rengini maviye ve tüm `<p>` öğelerinin metin rengini kırmızıya ayarlar. Ayrıca, sayfa "pudra mavisi" arka plan rengiyle görüntülenecektir:
```
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>THT</h1>
<p>#GreenTeam</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/cze6lou.png)

## Harici(External) CSS
Birçok HTML sayfasının stilini tanımlamak için harici bir style sayfası kullanılır.

Harici bir style sayfası kullanmak için, her HTML sayfasının `<head>` bölümüne bir bağlantı ekleyin:
```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>THT</h1>
<p>vancoondehni HTML Öğrenelim Serisi</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/pp0otld.png)

## CSS Renkleri, Yazı Tipleri ve Boyutları

color özelliği CSS'te metin rengini tanımlamak için kullanılır.

font-family özelliği CSS'te yazı tipini tanımlamak için kullanılır.

font-size özelliği CSS'te metin boyutunu tanımlamak için kullanılır.
```
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: blue;
  font-family: verdana;
  font-size: 300%;
}
p {
  color: red;
  font-family: courier;
  font-size: 160%;
}
</style>
</head>
<body>

<h1>HTML öğrenmek keyifli</h1>
<p>-vancoondehni</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/353tds9.png)

## CSS'te Kenarlar
border özelliği ile HTML elementlerinin etrafını sınırlayabiliriz.
```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 2px solid powderblue;
}
</style>
</head>
<body>

<h1>CSS Border Özelliği</h1>

<p>Merhabalar</p>
<p>ben.</p>
<p>Aziz aka vancoondehni</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/fwyee9z.png)

## CSS Padding
CSS padding özelliği, metin ve kenarlık arasında bir boşluk tanımlar.
```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 2px solid powderblue;
  padding: 30px;
}
</style>
</head>
<body>

<h1>Padding Özelliği</h1>

<p>THT</p>
<p>#GreenTeam</p>
<p>Altay ve Eşref Hocalarıma selamlar</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/316u9do.png)

## CSS Margin(Kenar Boşluğu)
CSS kenar boşluğu özelliği, sınırın dışında bir kenar boşluğu tanımlar.
```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 2px solid powderblue;
  margin: 50px;
}
</style>
</head>
<body>

<h1>Margin Özelliği</h1>

<p>#SafakBey</p>
<p>#W1sdom</p>
<p>#deltaturk</p>


</body>
</html>
```
![Çıktı](https://i.hizliresim.com/n557gnh.png)

## Harici CSS'e Link Eklemek
Harici style sayfalarına tam bir URL veya web sayfasına göre bir yolla(path) başvurulabilir.
```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="https://www.turkhackteam.org">
</head>
<body>

<h1>THT</h1>
<p>vancoondehni</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/qlrqqp7.png)

# Bölüm 6
## HTML Linkleri(Bağlantıları)
Bağlantılar tüm web sayfalarında bulunur.
Bağlantılar, kullanıcıların sayfadan sayfaya tıklamalarına izin verir.

## HTML Bağlantıları - Hyperlinks
HTML bağlantıları köprülerdir.

Bir bağlantıya tıklayıp başka bir belgeye atlayabilirsiniz.

Fareyi bir bağlantının üzerine getirdiğinizde, fare oku küçük bir ele dönüşecektir.

Not: Bir bağlantının metin olması zorunlu değildir. Bir bağlantı bir resim veya başka bir HTML öğesi olabilir.

## HTML Bağlantıları - Syntax
HTML'de `<a>` etiketi bir hyperlink tanımlar.

Örnek kullanım: `<a href="url">Bağlantı metni</a>`

`<a>` etiketinde en önemli özellik href özelliğidir. href özelliği bağlantının hedefini belirtir.

Yukarıdaki örnek kullanımda belirttiğimiz bağlantı metni kullanıcılar tarafından görülebilir.

Bağlantı metnine tıklandığında kullanıcı belirtilmiş olan URL adresine gönderilecektir.
```
<!DOCTYPE html>
<html>
<body>

<h1>HTML Links</h1>

<p><a href="https://www.turkhackteam.org/">Türk Hack Team'i ziyaret edin.</a></p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/n55wxau.png)

Varsayılan olarak, bağlantılar tüm tarayıcılarda aşağıdaki gibi görünecektir:

Ziyaret edilmemiş bir bağlantının altı çizili ve mavidir.

Ziyaret edilen bir bağlantının altı çizili ve mordur.

Aktif bir bağlantının altı çizili ve kırmızıdır.

## HTML Linkleri(Bağlantıları) - target özelliği
Bağlantılı sayfa mevcut tarayıcı penceresinde varsayılan(yani default olarak tanımlanmış) şekilde görüntülenecektir. Bunu değiştirmek için bağlantı için başka bir hedef belirtmelisiniz.

target özelliği bağlantılı belgenin nerede açılacağını belirtir.

target özelliği aşağıda belirttiğim eklentilerle birlikte kullanılabilir:

`_self` :Varsayılan eklentidir. Belgeyi, tıklandığı pencerede/sekmede açar.

`_blank` : Belgeyi yeni bir pencerede veya sekmede açar

`_parent` :Belgeyi üst çerçevede açar

`_top` : Belgeyi pencerenin tam gövdesinde açar
```
<!DOCTYPE html>
<html>
<body>

<h2>target özelliği    </h2>

<a href="turkhackteam.org" target="_blank">THT'yi karşılayın.</a>

<p>Eğer target="_blank", ise bağlantı yeni bir tarayıcı penceresinde veya sekmesinde açılacaktır.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/3lf10qr.png)

## Absolute URL vs. Relative URL(Mutlak URL'ler ve Göreli URL'ler)

Yukarıdaki her iki örnek de href özelliğinde mutlak bir URL (tam web adresi) kullanıyor.

Yerel bir bağlantı (aynı web sitesindeki bir sayfaya bağlantı), göreli bir URL ile belirtilir ("https://www" olmadan):

```
<!DOCTYPE html>
<html>
<body>

<h2>Absolute URLs</h2>
<p><a href="https://www.turkhackteam.org">THT</a></p>
<p><a href="https://github.com/kartalaziz/THTHTMLOgrenelimSerisi">Reposityory/a></p>

<h2>Relative URLs</h2>

<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/3crdr32.png)

## HTML Linkleri - Bir görseli link(bağlantı) olarak kullanmak

Bir görseli link olarak kullanmamız için yapmamız gereken `<img>` etiketini `<a>` etiketinin içerisine yerleştirmektir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Görsellerin Bağlantı Olarak Kullanılması</h2>

<p>Aşağıdaki görsel bir bağlantıdır. Görmek için tıklayınız.</p>

<a href="default.asp"><img src="smiley.gif" alt="HTML Öğrenelim - THT" style="width:42px;height:42px;"></a>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/c3peru4.png)

## E-mail adresini bağlantı olarak eklemek
Kullanıcının yeni bir e-posta göndermesine izin vermek için bir bağlantı oluşturmak istiyorsak href özelliğinin içinde `mailto:` ifadesi kullanılır.
```
<!DOCTYPE html>
<html>
<body>

<h2>E-mail adresini bağlantı olarak eklemek

</h2>

<p>Kullanıcının yeni bir e-posta göndermesine izin vermek için bir bağlantı oluşturmak istiyorsak href özelliğinin içinde mailto: ifadesi kullanılır.

</p>

<p><a href="mailto:selamınaleykümtht@gmail.com">Mail Gönder</a></p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/m90hdkf.png)

## Butonları Bağlantı(Link) Olarak Kullanmak
Bir HTML butonunu bağlantı olarak kullanmak için biraz JavaScript kodu eklemeniz gerekir.

JavaScript, bir buton tıklaması gibi belirli olaylarda ne olacağını belirtmenize olanak tanır:
```
<!DOCTYPE html>
<html>
<body>

<h2>Butonları Bağlantı(Link) Olarak Kullanmak</h2>

<p>Türk Hack Team'e ulaşmak için tıklayınız.</p>

<button onclick="document.location='https://www.turkhackteam.org/'">HTML Öğrenelim - Green Team - vancoondehni</button>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/k4n4u4x.png)

## Link(Bağlantı) Başlıkları
title özelliği bir element hakkında ekstradan bilgi sağlamak için kullanılır. Bu bilgiler genellikle mouse üzerine geldiğinde ipucu metni olarak gösterilir.
```
<!DOCTYPE html>
<html lang="en-TR">
<body>

<h2>Link Başlıkları</h2>
<p>title özelliği bir element hakkında ekstradan bilgi sağlamak için kullanılır. Bu bilgiler genellikle mouse üzerine geldiğinde ipucu metni olarak gösterilir..</p>
<a href="https://www.turkhackteam.org" title="THT">Türk Hack Team'i ziyaret edin.</a>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/38u95lp.png)

## HTML Linkleri(Bağlantıları) - Farklı Renkler
Bir HTML bağlantısı, ziyaret edilmiş olmasına, ziyaret edilmemiş olmasına veya etkin olmasına bağlı olarak farklı renklerde görüntülenir.

## HTML Bağlantı Renkleri

Varsayılan olarak, şu şekilde bir bağlantı görünecektir (tüm tarayıcılarda):

-Ziyaret edilmemiş bir bağlantının altı çizili ve mavidir.

-Ziyaret edilen bir bağlantının altı çizili ve mordur.

-Aktif bir bağlantının altı çizili ve kırmızıdır.

CSS kullanarak bağlantı durumu renklerini değiştirebilirsiniz:
```
<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  color: green;
  background-color: blue;
  text-decoration: none;
}
a:visited {
  color: pink;
  background-color:black;
  text-decoration: none;
}
a:hover {
  color: red;
  background-color: gray;
  text-decoration: underline;
}
a:active {
  color: yellow;
  background-color: orange;
  text-decoration: underline;
}
</style>
</head>
<body>

<h2>Bağlantı Renkleri</h2>

<p>Bağlantılar için tanımlanmış default renkleri değiştirebilirsiniz.</p>

<a href="html_images.asp" target="_blank">Selamın Aleyküm THT</a>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/f9u0g8q.png)

## Bağlantı Butonları
Bir bağlantı, CSS kullanılarak bir buton olarak da biçimlendirilebilir:
```
<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 15px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
</style>
</head>
<body>

<h2>Bağlantı Butonları</h2>
<p>Bir bağlantı, CSS kullanılarak bir buton olarak da biçimlendirilebilir:</p>
<a href="https://www.turkhackteam.org" target="_blank">Bu bir bağlantıdır. - THT</a>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/jokkac7.png)

## HTML Bağlantıları - Yer İmleri Oluşturun
Yer imleri, okuyucuların bir web sayfasının belirli bölümlerine atlayabilmeleri için kullanılabilir.

Bir web sayfası çok uzunsa yer imleri yararlı olabilir.

Bir yer imi oluşturmak için: önce yer imini oluşturun, ardından ona bir bağlantı ekleyin.

Bağlantı tıklandığında, sayfa aşağı veya yukarı kaydırılarak yer iminin bulunduğu konuma gelir.
```
<!DOCTYPE html>
<html>
<body>


<p><a href="#C10">10. Bölüme atlamak için tıklayınız</a></p>

<h2>Bölüm 1</h2>
<p>Merhaba</p>

<h2>Bölüm 2</h2>
<p>THT</p>

<h2>Bölüm 3</h2>
<p>Ben</p>

<h2 id="C4">Bölüm 4</h2>
<p>Aziz</p>

<h2>Bölüm 5</h2>
<p>Bu da HTML Öğrenelim Serisi</p>

<h2>Bölüm 6</h2>
<p>Serinin 6. bölümü</p>

<h2>Bölüm 7</h2>
<p>Konumuz bağlantılar</p>

<h2>Bölüm 8</h2>
<p>Bağlantılara yer imleri ekleme</p>

<h2>Bölüm 9</h2>
<p> ba bla bla</p>

<h2 id="C10">Bölüm 10</h2>
<p>ba bla bla</p>

<h2>Bölüm 11</h2>
<p> ba bla bla</p>

<h2>Bölüm 12</h2>
<p> ba bla bla</p>

<h2>Bölüm 13</h2>
<p> ba bla bla</p>

<h2>Bölüm 14</h2>
<p> ba bla bla</p>

<h2>Bölüm 15</h2>
<p>ba bla bla</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/2lav2vh.png)

# Bölüm 7
## HTML'de Görseller

HTML'de `<img>` etiketi bir görseli bir internet sayfasına gömmek için kullanılır.

Görseller teknik olarak bir web sayfasına eklenmez; görseller web sayfalarına bağlıdır. `<img>` etiketi, başvurulan görüntü için bir tutma alanı oluşturur.

`<img>` etiketi kapanış etiketine ihtiyaç duymaz.

`<img>` etiketinde 2 özellik öne çıkar:

- `src`: Görselin yolunu(path) belirtir.
- `alt`: Resim için alternatif bir metin belirtir.

### src Özelliği
`src` özelliği görselin yolunu(URL) belirtir.
Not: Bir web sayfası yüklendiğinde görüntüyü bir web sunucusundan alan ve sayfaya ekleyen tarayıcıdır(Chrome,Mozilla vs.). Bu nedenle, görüntünün web sayfasına göre aynı yerde kaldığından emin olun, aksi takdirde ziyaretçileriniz kırık bir bağlantı simgesi alır. Tarayıcı resmi bulamıyorsa, bozuk bağlantı simgesi ve alternatif metin gösterilir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Alternatif metin</h2>

<p>Alt özelliği, görsel içeriğini metin halinde yansıtmalıdır, böylece görseli göremeyen kullanıcılar görselin ne içerdiğini okuyarak anlar:</p>

<img src="https://i.hizliresim.com/c5awiw0.jpg" alt="Green Team" width="460" height="345">

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/kpsegnn.png)

### alt Özelliği
Kullanıcı herhangi bir nedenle (yavaş bağlantı, src özelliğindeki bir hata veya kullanıcı bir ekran okuyucu kullanıyorsa) görseli görüntüleyemiyorsa, alt özelliği bir resim için alternatif bir metin sağlar.

alt özelliğinde kullanacağınız metin resmi açıklayıcı nitelikte olmalıdır.

Yukarıdaki görseli görüntüleyemeseydik görselin alt metni olarak Green Team yazısını görüntüleyecektik.

## Görsel Boyutu - Genişlik ve Yükseklik
Görselin genişliğini ve yüksekliğini değiştirmek için `style` özelliğinin `width` ve `height` eklentilerini kullanıyoruz.

İki şekilde kullanım mümkündür:
1- `style="width:500px;height:600px;"`

2- `width="500" height="600"`
```
<!DOCTYPE html>
<html>
<body>

<h2>Görsel Boyutu</h2>

<p>Görselin genişliğini ve yüksekliğini değiştirmek için style özelliğinin width ve height eklentilerini kullanıyoruz.

</p>

<img src="https://upload.wikimedia.org/wikipedia/commons/a/a8/Ataturk1930s.jpg" alt="Atatürk" width="500" height="600">

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/arles7b.png)

## Başka Bir Klasördeki Görseller
Görselleriniz bir alt klasördeyse, src özelliğine klasör adını eklemelisiniz.
```
<!DOCTYPE html>
<html>
<body>

<h2>Başka Bir Klasördeki Görseller

</h2>
<p>Görselleriniz bir alt klasördeyse, src özelliğine klasör adını eklemelisiniz.

</p>

<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/hy84tmw.png)

## Başka bir internet sitesindeki/sunucudaki görseller
Bazı web siteleri başka bir sunucudaki bir görseli işaret eder. Başka bir sunucudaki bir görseli işaret etmek için, `src` özelliğinde mutlak bir URL belirtmelisiniz.
```
<!DOCTYPE html>
<html>
<body>

<h2>Başka bir internet sitesindeki/sunucudaki görseller

</h2>

<img src="https://www.turkhackteam.org/styles/v1/tht/logo.png" alt="www.turkhackteam.org" style="width:555px;height:225px;">

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/bf9y93v.png)

## Hareketli Görseller(GIF)
HTML hareketli görsellere(GIF'lere) izin verir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Hareketli Görseller</h2>

<p>HTML hareketli görsellere(GIF'lere) izin verir.

</p>

<img src="programming.gif" alt="Computer man" style="width:111px;height:111px;">

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/qqlqpn5.png)

## Bağlantı(Link) olarak Görseller
Bir görseli bağlantı(link) olarak kullanmak için `<a>` etiketinin içerisine `<img>` etiketini koymalıyız.
```
<!DOCTYPE html>
<html>
<body>

<h2>Bağlantı(Link) olarak Görseller

</h2>

<p>Görsel aslında bir bağlantıdır. Tıklayabilirsiniz. </p>

<a href="default.asp">
<img src="smiley.gif" alt="HTML Öğrenelim" style="width:42px;height:42px;">
</a>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/tswl2em.png)

## Görsel Kaydırma(Image Floating)
Görselin bir metnin sağına veya soluna kaymasını sağlamak için CSS float özelliğini kullanırız.
```
<!DOCTYPE html>
<html>
<body>

<h2>Görsel Kaydırma(Image Floating)

</h2>
<p><strong>Görseli sağa kaydır:</strong></p>

<p>
<img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
Sağa kaydırılmış görselle birlikte bir paragraf.
</p>

<p><strong>Görseli sola kaydır:</strong></p>
<p>
<img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
Sola kaydırılmış görselle birlikte bir paragraf.
</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/olwlj1k.png)

## Sıklıkla Kullanılan Görsel Formatları
Tüm tarayıcılarda (Chrome, Edge, Firefox, Safari, Opera) desteklenen en yaygın görüntü dosyası türleri şunlardır:
![Çıktı](https://i.hizliresim.com/p9up174.png)

## HTML'de Görsel Haritaları
Görsel haritalarını kullanarak görsellerde tıklanabilir alanlar oluşturabilirsiniz.

HTML'de `<map>` etiketi bir görsel haritası tanımlar. Bir görsel haritası görselde tıklanabilir alanlar oluşturur. Bu alanlar bir veya birden çok `<area>` etiketi kullanarak oluşturulur.
```
<!DOCTYPE html>
<html>
<body>

<h2>Görsel Haritaları</h2>
<p>Büyüteç görseline gitmek için ortadaki yeşil alana, Türk Hack Team'e gitmek için alttaki yazıya arka plana gitme için ise sağ taraftaki boş alana tıklayınız.</p>

<img src="https://i.hizliresim.com/c5awiw0.jpg" alt="GreenTeam" usemap="#workmap" width="400" height="379">

<map name="workmap">
<area shape="rect" coords="34,44,270,350" alt="Büyüteç" href="https://productimages.hepsiburada.net/s/29/375/10279573717042.jpg">
<area shape="rect" coords="290,172,333,250" alt="TürkHackTeam" href="https://www.turkhackteam.org/styles/v1/tht/logo.png">
<area shape="circle" coords="337,300,44" alt="Arkaplan" href="https://i.hizliresim.com/c5awiw0.jpg">
</map>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/2v25uvi.png)

## Görsel Haritaları Nasıl Çalışır?
Bir görsel haritasının arkasındaki fikir, görüntünün neresine tıkladığınıza bağlı olarak farklı eylemler gerçekleştirebilmenizdir.

Bir görsel haritası oluşturmak için bir resme ve tıklanabilir alanları tanımlayan bir HTML koduna ihtiyacınız vardır.

Görsel Haritası oluşturma hakkında daha detaylı bilgi edinmek istiyorsanız bağlantıyı inceleyebilirsiniz. (Çok detaya giriyor bahsetmek istemedim.)

## HTML'de Arka plan Görselleri
HTML'de bir elemana arka plan eklemek için `style` özelliğini ve CSS'in `background-image` özelliğini kullanırız.
```
<!DOCTYPE html>
<html>
<body>

<h2>Arkaplan Görselleri</h2>

<p>p elementi için bir arka plan:</p>

<p style="background-image: url('https://www.turkhackteam.org/styles/v1/tht/logo.png');">
Arka plan görsellerini belirtebilirsiniz.<br>
Bu örnekte, arka plan görseli<br>
bir p elementi için belirlendi.<br>
Arka plan varsayılan olarak<br>
aynı yönde tekrar edecek<br>

</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/195jjy1.png)

## Bir Sayfanın Arka Planı
Tüm sayfanın bir arka plan görüntüsüne sahip olmasını istiyorsanız, arka plan görüntüsünü `<body>` öğesinde belirtmelisiniz.
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
background-image: url('https://i.hizliresim.com/cv48p7d.png');
}
</style>
</head>
<body>

<h2>Arkaplan Görseli</h2>

<p>Arka plan görüntüsü, belirtildiği yerde, gövde öğesinden daha küçükse kendini tekrar eder.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/pn2wosq.png)

## Arka plan Tekrarı
Arka plan görüntüsü öğeden daha küçükse, görüntü öğenin sonuna ulaşana kadar yatay ve dikey olarak kendini tekrar eder.
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
background-image: url('example_img_girl.jpg');
}
</style>
</head>
<body>

<h2>Arka plan Tekrarı</h2>

<p>Arka plan görüntüsü öğeden daha küçükse, görüntü öğenin sonuna ulaşana kadar yatay ve dikey olarak kendini tekrar eder.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/e7uodvi.png)
Arka plan görüntüsünün kendini tekrarlamasını önlemek için `background-repeat` özelliğini `no-repeat` özelliğiyle değiştiriniz.
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
background-image: url('example_img_girl.jpg');
background-repeat: no-repeat;
}
</style>
</head>
<body>

<h2>Arka plan Tekrarı

</h2>

<p>Arka plan görüntüsünün kendini tekrarlamasını önlemek için background-repeat özelliğini no-repeat özelliğiyle değiştiriniz.

</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/obon52t.png)

## Arka Plan Kapağı

Arka plan görüntüsünün tüm öğeyi kaplamasını istiyorsanız, `background-size` özelliğini `cover` şekilde ayarlayabilirsiniz.

Ayrıca, tüm öğenin her zaman kapsandığından emin olmak için `background-attachment` özelliğini `fixed` olarak ayarlayın.

Bu şekilde, arka plan görüntüsü, herhangi bir esneme olmaksızın tüm öğeyi kaplayacaktır (görüntü orijinal orantılarını koruyacaktır).

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
background-image: url('img_girl.jpg');
background-repeat: no-repeat;
background-attachment: fixed;
background-size: cover;
}
</style>
</head>
<body>

<h2>Arka Plan Kapağı

</h2>

<p>Arka plan görüntüsünün tüm öğeyi kaplamasını istiyorsanız, background-size özelliğini cover şekilde ayarlayabilirsiniz.

Ayrıca, tüm öğenin her zaman kapsandığından emin olmak için background-attachment özelliğini fixed olarak ayarlayın.
Bu şekilde, arka plan görüntüsü, herhangi bir esneme olmaksızın tüm öğeyi kaplayacaktır (görüntü orijinal orantılarını koruyacaktır).</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/6ldqowz.png)
## Arka plan Germek
Arka plan görüntüsünün tüm öğeye sığacak şekilde uzamasını istiyorsanız `background-size` özelliğini `100% 100%` olarak değiştirin.
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
background-image: url('https://i.hizliresim.com/c5awiw0.jpg');
background-repeat: no-repeat;
background-attachment: fixed;
background-size: 100% 100%;
}
</style>
</head>
<body>

<h2>Arka plan Germek

</h2>

<p>Arka plan görüntüsünün tüm öğeye sığacak şekilde uzamasını istiyorsanız background-size özelliğini 100% 100% olarak değiştirin.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/tlp4mvr.png)

## HTML <picture> Elementi

HTML `<picture>` elementi, farklı cihazlar veya ekran boyutları için farklı görseller görüntülemenize olanak tanır.

`<picture>` öğesi, her biri srcset özelliği aracılığıyla farklı görüntülere atıfta bulunan bir veya daha fazla `<source>` öğesi içerir. Bu şekilde tarayıcı, mevcut görünüme ve/veya cihaza en uygun görüntüyü seçebilir. Her `<source>` öğesinin, görüntünün en uygun olduğu zamanı tanımlayan bir media özelliği vardır.

```
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h2>HTML <picture> Elementi</h2>

<picture>
<source media="(min-width: 650px)" srcset="img_food.jpg">
<source media="(min-width: 465px)" srcset="img_car.jpg">
<img src="img_girl.jpg" style="width:auto;">
</picture>

<p>Farklı görüntü alanı boyutlarında yüklenen resmin farklı sürümlerini görmek için tarayıcıyı yeniden boyutlandırın.
Tarayıcı, medya sorgusunun kullanıcının mevcut görüntü alanı genişliğiyle eşleştiği ilk kaynak öğeyi arar,
ve srcset özelliğiyle belirtilen resmi getirir.</p>

<p>img öğesi, resim bildirim bloğunun son alt etiketi olarak gereklidir.
img öğesi, resim öğesini desteklemeyen tarayıcılar için veya kaynak etiketlerden hiçbiri eşleşmediyse geriye dönük uyumluluk sağlamak için kullanılır.
</p>

<p><strong>Not:</strong> picture elementi, IE12 ve önceki sürümlerde veya Safari 9.0 ve önceki sürümlerde desteklenmez.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/j94y0lp.png)

