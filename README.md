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

# Bölüm 8

## HTML'de Favicon
Favicon internet sitelerini açtığımızda sayfa başlığının yanında gözüken küçük görsellerdir. Örnek verecek olursak:

![Çıktı](https://i.hizliresim.com/sdmhf5d.png)

THT'yi ziyaret ettiğinizde sayfa başlığının yanında THT Logosunu görüyorsunuz. İşte buraya konulan görsel Favicon olarak adlandırılır.

### HTML'de Favicon Nasıl Eklenir?

Her görseli favicon olarak ekleyebilirsiniz. Hatta kendi favicon tasarımınızı da yapabilirsiniz.

Kendi favicon tasarımınızı yapabileceğiniz bir site önerisi: favicon.cc

İnternet sitenize favicon eklemek için root kısmında images adıyla bir dosya oluşturunuz. Bu dosyanın içine favicon olarak kullanmak istediğiniz görseli aktarınız.

NOT: Favicon eklerken genellikle kullanılan adlandırma: favicon.ico

Sonrasında index.html dosyanıza `<title>` elementinden sonra bir `<link>` elementi ekleyin.

Son olarak index.html dosyasını kaydedin ve internet sitenizi yenileyin. Artık favicon görseliniz sitenize eklenmiş olacaktır.
```
<!DOCTYPE html>
<html>
<head>
  <title>vancoondehni</title>
  <link rel="icon" type="image/x-icon" href="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRC_5HSEFL27dWyQlK6gG8PMdkVZeO9Cb6iMg&usqp=CAU">
</head>
<body>

<h1>Selamlar THT</h1>
<p>Favicon - örnek</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/6wgxwsf.png)

## HTML'de Tablolar
Tablolar verileri kolonlara ve sütunlara ayırarak düzenlememizi sağlar.

HTML'de tablolar, satırlar ve sütunlar içindeki tablo hücrelerinden oluşur.

### Tablo Hücreleri
Her bir tablo hücresi `<td>` ve `</td>` etiketleriyle tanımlanır.

Not: td etiketinin açılımı: table data

`<td>` ve `</td>` etiketleri arasındaki tüm içerik o hücrenin içeriğidir.

Not: table data elementleri, tablonun veri kapsayıcılarıdır.

Her türlü HTML elementini içerebilirler; metin, resimler, listeler, diğer tablolar vb.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
border:1px solid black;
}
</style>
<body>

<h2>TD elementi tablo hücrelerini tanımlarken kullanılır.</h2>

<table style="width:100%">
<tr>
<td>TürkHackTeam</td>
<td>Bulunduğu Team</td>
<td>Kullanıcı Adı</td>
</tr>
</table>

<p>Örneği daha iyi anlayabilmeniz için border yani sınır kısımlarını ekledik.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/i0w7u69.png)

### Tablo Satırları
Her bir tablo satırı `<tr>` etiketi ile başlar ve `</tr>` etiketi ile biter.

Not: tr etiketinin açılımı table row

Bir tabloya istediğiniz kadar satır ekleyebilirsiniz, sadece her satırdaki hücre sayısının aynı olduğuna dikkat edin.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
}
</style>
<body>

<h2>TR elementi tablo satırlarını tanımlamak için kullanılır</h2>

<table style="width:100%">
  <tr>
    <td>THT Kullanıcı Adı</td>
    <td>Bulunduğu Ekip</td>
    <td>Rütbesi</td>
  </tr>
  <tr>
    <td>vancoondehni</td>
    <td>GreenTeam</td>
    <td>Mod</td>
  </tr>
</table>

<p>Örneği daha iyi anlayabilmeniz için tabloya sınırlar ekledik(border özelliği ile).</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/eoo14n6.png)

### Tablo Başlıkları
Bazen hücrelerin başlık olmasını isteyebilirsiniz. Bu durumda `<td>` etiketi yerine `<th>` etiketini kullanıyoruz.

Varsayılan başlıklar kalın, ortalanmış haldedirler. Değiştirmek için CSS'i kullanabilirsiniz.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
}
</style>
<body>

<h2>TH elementi tablolardaki başlıkları tanımlamak için kullanılır</h2>

<table style="width:100%">
  <tr>
    <th>THT Kullanıcı Adı</th>
    <th>Bulunduğu Ekip</th>
    <th>Ekipteki rölü</th>
  </tr>
  <tr>
    <td>vancoondehni</td>
    <td>GreenTeam</td>
    <td>Mod</td>
  </tr>
  <tr>
    <td>ALTAY'</td>
    <td>GreenTeam</td>
    <td>Genel Sorumlu</td>
   </tr>
   <tr>
    <td>Eşref'</td>
    <td>GreenTeam</td>
    <td>Genel Sorumlu</td>
  </tr>
</table>

<p>Örneğin anlaşılırlığını arttırmak için border yani sınır özelliği eklenmiştir.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/id5a3lg.png)

![Table](https://i.hizliresim.com/1zihog2.png)

### HTML'de Tablo Sınırları

HTML'de farklı boyutlarda ve biçimlerde tablo sınırları tanımlamak mümkündür.

##### Nasıl bir sınır eklenir?
Bir tabloya kenarlık eklediğinizde, her bir tablo hücresinin çevresine de kenarlıklar eklersiniz. 
![Çıktı](https://i.hizliresim.com/4fj02zx.png)
Tablolara sınır eklemek için CSS'in border özelliğini table,th ve td elementlerinde kullanmalıyız.
```
table, th, td {
  border: 1px solid black;
}

```
## Daraltılmış Tablo Sınırları(Kenarlıkları)
Tablolarda ikili kenarlıklar eklemek istemiyorsal CSS'in `border-collapse` özelliği `collapse` ile kullanılır.

Bu tablolarda tek kenarlığa sahip olmanızı sağlar.
![Çıktı](https://i.hizliresim.com/d7znw6m.png)
```

<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Daraltılmış Tablo Sınırları(Kenarlıkları)

</h2>
<p>Tablolarda ikili kenarlıklar eklemek istemiyorsal CSS'in border-collapse özelliği collapse ile kullanılır.

</p>

<table style="width:100%">
   <tr>

    <th>THT Kullanıcı Adı</th>

    <th>Bulunduğu Ekip</th>

    <th>Ekipteki rölü</th>

  </tr>

  <tr>

    <td>vancoondehni</td>

    <td>GreenTeam</td>

    <td>Mod</td>

  </tr>

  <tr>

    <td>ALTAY'</td>

    <td>GreenTeam</td>

    <td>Genel Sorumlu</td>

   </tr>

   <tr>

    <td>Eşref'</td>

    <td>GreenTeam</td>

    <td>Genel Sorumlu</td>

  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/trkxzur.png)

## Style Tablo Kenarlıkları
Her hücrenin arka plan rengini ayarlarsanız ve kenarlığa beyaz bir renk verirseniz, görünmez bir kenarlık izlenimi elde edersiniz.
![Çıktı](https://i.hizliresim.com/83mq3uz.png)
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid white;
  border-collapse: collapse;
}
th, td {
  background-color: #96D4D4;
}
</style>
</head>
<body>

<h2>Görünmez Kenarlıklarla Tablo Oluşturmak</h2>

<p>Her hücrenin arka plan rengini ayarlarsanız ve kenarlığa beyaz bir renk verirseniz, görünmez bir kenarlık izlenimi elde edersiniz.

</p>

<table style="width:100%">
   <tr>



    <th>THT Kullanıcı Adı</th>



    <th>Bulunduğu Ekip</th>



    <th>Ekipteki rölü</th>



  </tr>



  <tr>



    <td>vancoondehni</td>



    <td>GreenTeam</td>



    <td>Mod</td>



  </tr>



  <tr>



    <td>ALTAY'</td>



    <td>GreenTeam</td>



    <td>Genel Sorumlu</td>



   </tr>



   <tr>



    <td>Eşref'</td>



    <td>GreenTeam</td>



    <td>Genel Sorumlu</td>

  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/7ygkfr2.png)

### Yuvarlak Tablo Kenarları
`border-radius` özelliği ile kenarları yuvarlaklaştırılmış tablolar elde edebilirsiniz.
![Çıktı](https://i.hizliresim.com/a7fpra1.png)
Yukarıdaki görseli elde etmek için kullanacağınız table kodları:
```
table, th, td {
  border: 1px solid black;
  border-radius: 10px;
}
```
Tablonun kenarındaki kenarlıkları yok etmek istiyorsanız table etiketini çıkartmanız gerekir.
![Çıktı](https://i.hizliresim.com/ak0b8om.png)
```
<!DOCTYPE html>
<html>
<head>
<style>
th, td {
  border: 1px solid black;
  border-radius: 10px;
}
</style>
</head>
<body>

<h2>Yuvarlak Tablo Kenarları

</h2>

<p>border-radius özelliği ile kenarları yuvarlaklaştırılmış tablolar elde edebilirsiniz.
Tablonun kenarındaki kenarlıkları yok etmek istiyorsanız table etiketini çıkartmanız gerekir.



</p>

<table style="width:100%">
  <tr>


    <th>THT Kullanıcı Adı</th>

    <th>Bulunduğu Ekip</th>

    <th>Ekipteki rölü</th>

  </tr>

  <tr>

    <td>vancoondehni</td>

    <td>GreenTeam</td>

    <td>Mod</td>

  </tr>

  <tr>

    <td>ALTAY'</td>

    <td>GreenTeam</td>

    <td>Genel Sorumlu</td>

   </tr>

   <tr>

    <td>Eşref'</td>

    <td>GreenTeam</td>

    <td>Genel Sorumlu</td>


  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/e5mdzwo.png)

## Noktalı Tablo Kenarları
`border-style` özelliğini kullanarak tabloların kenarlarını noktalı hale getirebilirsiniz.
![Çıktı](https://i.hizliresim.com/9z2gr06.png)

### Kenarlık Rengi
`border-color` özelliği ile tabloların kenarlık renklerini değiştirebilirsiniz.
```
<!DOCTYPE html>
<html>
<head>
<style>
th, td {
  border-style:solid;
  border-color: #96D4D4;
}
</style>
</head>
<body>

<h2>Kenarlık Rengi

</h2>

<p>border-color özelliği ile tabloların kenarlık renklerini değiştirebilirsiniz.

</p>

<table style="width:100%">
  <tr>


    <th>THT Kullanıcı Adı</th>


    <th>Bulunduğu Ekip</th>


    <th>Ekipteki rölü</th>


  </tr>


  <tr>


    <td>vancoondehni</td>


    <td>GreenTeam</td>


    <td>Mod</td>


  </tr>


  <tr>


    <td>ALTAY'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>


   </tr>


   <tr>


    <td>Eşref'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>



  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/ri0xhor.png)

## HTML'de Tablo Boyutları

Tablolarının her sütun, satır veya tüm tablo için farklı boyutları olabilir.

`style` özelliğini kullanarak `width` ve `height` ile tablo, sütun ve satır boyutlarını değiştirebilirsiniz.

### Tablo Genişliği
Tablonun genişliğini değiştirmek için style özelliğini `<table>` etiketinde kullanmalıyız.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
  border-collapse: collapse;
}
</style>

<body>

<h2>%200 Genişlikte Bir HTML Tablosu</h2>

<table style="width:200%">
   <tr>


    <th>THT Kullanıcı Adı</th>

    <th>Bulunduğu Ekip</th>

    <th>Ekipteki rölü</th>

  </tr>

  <tr>

    <td>vancoondehni</td>


    <td>GreenTeam</td>


    <td>Mod</td>



  </tr>


  <tr>


    <td>ALTAY'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>


   </tr>


   <tr>

    <td>Eşref'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>



  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/bk4a9xe.png)

### Hücre Genişliği
Belirli bir sütunun boyutunu ayarlamak için, bir `<th>` veya `<td>` öğesine style özelliğini ekleyebilirsiniz.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
  border-collapse: collapse;
}
</style>
<body>

<h2>THT Kullanıcı Adı hücresinin genişliği %120</h2>

<table style="width:100%">
 
 
   <tr>


    <th style="width:120%">THT Kullanıcı Adı</th>



    <th>Bulunduğu Ekip</th>



    <th>Ekipteki rölü</th>


  </tr>



  <tr>


    <td>vancoondehni</td>


    <td>GreenTeam</td>


    <td>Mod</td>


  </tr>


  <tr>


    <td>ALTAY'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>



   </tr>


   <tr>

    <td>Eşref'</td>


    <td>GreenTeam</td>


    <td>Genel Sorumlu</td>


  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/i2q3qro.png)

### Tablo Satır Yüksekliği

Belirli bir satırın yüksekliğini ayarlamak için, bir tablo satırı elementine `style` özelliği eklenir.
```
<!DOCTYPE html>
<html>
<style>
table, th, td {
  border:1px solid black;
  border-collapse: collapse;
}
</style>
<body>

<h2>İkinci sütunun boyutu %200</h2>

<table style="width:100%">
  <tr>
    <th>THT Kullanıcı Adı</th>
    <th>Bulunduğu Ekip</th>
    <th>Ekipteki Rolü</th>
  </tr>
  <tr style="height:200px">
    <td>a</td>
    <td>b</td>
    <td>c</td>
  </tr>
  <tr>
    <td>d</td>
    <td>e</td>
    <td>f</td>
  </tr>
  <tr>
    <td>g</td>
    <td>h</td>
    <td>z</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/mnyxk0s.png)

### Tablo Başlıkları
Tablolar her sütun veya satır için veya birçok sütun/satır için başlık içerebilir.
![Çıktı](https://i.hizliresim.com/hldpndd.png)
Tablo başlıkları `<th>` etiketi ile tanımlanırlar.

### Dikey Tablo Başlıkları
İlk sütunu tablo başlıkları olarak kullanmak için her satırdaki ilk hücreyi `<th>` etiketiyle tanımlarız.

```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Dikey Tablo Başlıkları

</h2>

<p>İlk sütunu tablo başlıkları olarak kullanmak için her satırdaki ilk hücreyi th etiketiyle tanımlarız.

</p>

<table style="width:100%">
  <tr>
    <th>AD</th>
    <td>Ahmet</td>
    <td>Kaş</td>
  </tr>
  <tr>
    <th>SOYAD</th>
    <td>Mehmet</td>
    <td>Taş</td>
  </tr>
  <tr>
    <th>YAŞ</th>
    <td>15</td>
    <td>53</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/hrj4cvv.png)

### Tablo Başlıklarını Hizalamak
Varsayılan tablo başlıkları kalın ve ortalanmış şekildedir. Başlıkları sağa veya sola yaslamak için CSS'in `text-align` özelliği kullanılır.

Sağa yaslamak için:
```
th {
  text-align: right;
}
```
Sola yaslamak için:
```
th {
  text-align: left;
}
```
### Birden Çok Sütun için Başlık Oluşturmak
İki veya daha fazla sütuna yayılan bir başlık tanımlamak mümkündür.
Bunu yapabilmek için colspan özelliğini `<th>` etiketinin içinde kullanmalıyız.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Birden Çok Sütun için Başlık Oluşturmak

</h2>

<p>İki veya daha fazla sütuna yayılan bir başlık tanımlamak mümkündür.

Bunu yapabilmek için colspan özelliğini <th> etiketinin içinde kullanmalıyız.</p>

<table style="width:100%">
  <tr>
    <th colspan="2">Kişi</th>
    <th>Yaş</th>
  </tr>
  <tr>
    <td>Ahmet</td>
    <td>Kocakafa</td>
    <td>45</td>
  </tr>
  <tr>
    <td>Celil</td>
    <td>Cüce</td>
    <td>15</td>
  </tr>
</table>
</body>
</html>
```
![Çıktı](https://i.hizliresim.com/hlan7k4.png)

### Tablo Başlığı

Tüm tablo için bir tablo başlığı ekleyebilirsiniz.

Bunun için table etiketinin içerisine `<caption>` etiketi eklenir.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
th, td {
  padding: 5px;
  text-align: left;
}
</style>
</head>
<body>

<h2>Tablo Başlığı</h2>
<p>Tüm tablo için bir tablo başlığı ekleyebilirsiniz.

Bunun için table etiketinin içerisine caption etiketi eklenir.</p>

<table style="width:100%">
  <caption>Aylık Yatırımlar</caption>
  <tr>
    <th>Aylık</th>
    <th>Yatırım Miktarı</th>
  </tr>
  <tr>
    <td>Ocak</td>
    <td>3000TL</td>
  </tr>
  <tr>
    <td>Şubat</td>
    <td>2000TL</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/3stlfsl.png)

### HTML Tablo Doldurma ve Aralık Ekleme(Padding&Spacing)
HTML tablolarında, hücrelerin içindeki dolguyu ve hücreler arasındaki boşluğu ayarlayabiliriz.
![Çıktı](https://i.hizliresim.com/j7nfqll.png)
Doldurma(Padding): Tablo hücrelerine dolgu eklemek için CSS padding özelliği kullanılır.
```
th, td {
  padding: 15px;
}
```
Aralık Ekleme(Spacing): Tablo hücreleri arasındaki boşluğu değiştirmek için table elementinin içerisinde CSS'in `border-spacing` özelliğini kullanabiliriz.
```
table {
  border-spacing: 30px;
}
```
## HTML Tablolarında Colspan ve Rowspan
HTML tabloları, birden çok satıra ve/veya sütuna yayılan hücrelere sahip olabilir.
![Çıktı](https://i.hizliresim.com/9tiygwv.png)
### Colspan
Bir hücreyi birden çok sütuna yaymak için `colspan` özelliği kullanılır.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>İki sütuna yayılan hücre</h2>
<p>Bir hücreyi birden çok sütuna yaymak için colspan özelliği kullanılır.

</p>

<table style="width:100%">
  <tr>
    <th colspan="2">Kullanıcı</th>
    <th>Yaş</th>
  </tr>
  <tr>
    <td>Mahmut</td>
    <td>Tuncer</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Ajdar</td>
    <td>Süperstarxd</td>
    <td>31</td>
  </tr>
</table>
</body>
</html>
```
![Çıktı](https://i.hizliresim.com/ngfsmxl.png)

### Rowspan
Bir hücreyi birden çok satıra yaymak için `rowspan` özelliği kullanılır.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Rowspan - bir hücreyi 2 satıra yayalım

</h2>
<p>Bir hücreyi birden çok satıra yaymak için rowspan özelliği kullanılır.

</p>

<table style="width:100%">
  <tr>
    <th>Kullanıcı</th>
    <td>mahmutqral123</td>
  </tr>
  <tr>
    <th rowspan="2">Sosyal Medya Hesapları</th>
    <td>twitter.com/mahmutqral123</td>
  </tr>
  <tr>
    <td>instagram.com/mahmutqral123</td>
  </tr>
</table>
</body>
</html>
```
![Çıktı](https://i.hizliresim.com/2ua06lz.png)

## HTML Tablo Stilleri
CSS'i kullanarak tablonuzun görünüşünü daha iyi hale getirebilirsiniz.

### HTML Tabloları - Zebra Çizgileri
Her 2 tablo satırından birisine arka plan rengi eklerseniz, güzel bir zebra çizgili efekti elde edersiniz.

Her 2 satırdan birisini farklı renk yapmak için `:nth-child(even)` özelliği kullanılır.
```
<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #D6EEEE;
}
</style>
</head>
<body>

<h2>HTML Tabloları - Zebra Çizgileri

</h2>
<p>Her 2 tablo satırından birisine arka plan rengi eklerseniz, güzel bir zebra çizgili efekti elde edersiniz.

Her 2 satırdan birisini farklı renk yapmak için :nth-child(even) özelliği kullanılır.</p>

<table>
  <tr>
  <th>Kullanıcı Adı</th>
  <th>Ekip</th>
  <th>Rol</th>
  </tr>
  <tr>
  <td>SafakBey</td>
  <td>GreenTeam</td>
  <td>Mod</td>
  </tr>
  <tr>
  <td>Kuvayihackiye</td>
  <td>GreenTeam</td>
  <td>Green Team Senior</td>
  </tr>
  <tr>
  <td>connec</td>
  <td>GreenTeam</td>
  <td>Mod</td>
  </tr>
  <tr>
  <td>Reina</td>
  <td>Basın Medya</td>
  <td>Lider</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/awyrraj.png)

### HTML Tabloları - Dikey Zebra Çizgileri
Dikey zebra çizgileri oluşturmak için, her iki sütundan birisine renk vermemiz gerekir.

Bunu yapmak için :nth-child(even) özelliğini kullanırız.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}

th:nth-child(even),td:nth-child(even) {
  background-color: #D6EEEE;
}
</style>
</head>
<body>

<h2>HTML Tabloları - Dikey Zebra Çizgileri

</h2>
<p>Dikey zebra çizgileri oluşturmak için, her iki sütundan birisine renk vermemiz gerekir.

Bunu yapmak için :nth-child(even) özelliğini kullanırız.</p>

<table style="width:100%">
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
    <th>FRI</th>
    <th>SAT</th>
    <th>SUN</th>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/ch6nuyb.png)

### Dikey ve Yatay Zebra Çizgilerini Birleştirin
Yukarıdaki iki örnekteki stili birleştirebilirsiniz ve her iki satırda bir ve her iki sütunda bir çizgiler olacaktır.

Bu özelliği kullanabilmek için `rgba()` özelliği ile renkleri belirtmeliyiz.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}

tr:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}

th:nth-child(even),td:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}
</style>
</head>
<body>

<h2>Dikey ve Yatay Zebra Çizgilerini Birleştirin

</h2>
<p>Yukarıdaki iki örnekteki stili birleştirebilirsiniz ve her iki satırda bir ve her iki sütunda bir çizgiler olacaktır.

Bu özelliği kullanabilmek için rgba() özelliği ile renkleri belirtmeliyiz.</p>

<table style="width:100%">
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
    <th>FRI</th>
    <th>SAT</th>
    <th>SUN</th>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/8n0qcmp.png)

### Yatay Bölücüler
Eğer kenarları sadece altta belirtmek istiyorsanız yatay bölücüleri kullanabilirsiniz.

Bunun için tr elementinin içine `border-bottom` özelliği eklenir.
```
<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

tr {
  border-bottom: 1px solid #ddd;
}
</style>
</head>
<body>

<h2>Yatay Bölücüler

</h2>
<p>Eğer kenarları sadece altta belirtmek istiyorsanız yatay bölücüleri kullanabilirsiniz.

Bunun için tr elementinin içine border-bottom özelliği eklenir.</p>

<table>
  <tr>
    <th>İsim</th>
    <th>Soyad</th>
  <th>Numara</th>
  </tr>
  <tr>
    <td>a</td>
    <td>b</td>
    <td>1</td>
  </tr>
  <tr>
    <td>c</td>
    <td>d</td>
    <td>2</td>
  </tr>
  <tr>
    <td>e</td>
    <td>r</td>
    <td>3</td>
  </tr>
  <tr>
    <td>z</td>
    <td>y</td>
    <td>4</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/jx2wgva.png)

### Üzerine Geldiğinde Renk Değiştiren Tablo
`tr` etiketinde `:hover` özelliğini kullanarak mouse bir satırın üstüne geldiğinde farklı renge dönen(efekt) tablolar oluşturabilirsiniz.
```
<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #DDD;
}

tr:hover {background-color: #D6EEEE;}
</style>
</head>
<body>

<h2>Üzerine Geldiğinde Renk Değiştiren Tablo

</h2>
<p>Efekti görmek için bir satırın üzerine mouse imlecinizi getirin</p>

<table>
  <tr>
    <th>Ad</th>
    <th>Soyad</th>
    <th>Şehir</th>
  </tr>
  <tr>
    <td>a</td>
    <td>b</td>
    <td>1</td>
  </tr>
  <tr>
    <td>c</td>
    <td>d</td>
    <td>2</td>
  </tr>
  <tr>
    <td>z</td>
    <td>x</td>
    <td>3</td>
  </tr>
  <tr>
    <td>g</td>
    <td>h</td>
    <td>5</td>
  </tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/i1rz8hu.png)

### HTML Tablolarında Ortak Grup(Colgroup)

`<colgroup>` elementi ile bazı kolonları ortak şekilde görünümünü değiştirebilirsiniz.

Eğer ilk iki kolonu aynı görünüşte yapmak istiyorsak `<colgroup>` ve `<col>` elementlerini kullanırız.

![Çıktı](https://i.hizliresim.com/3wafbgn.png)

`<colgroup>` elementi, sütun özellikleri için bir kapsayıcı olarak kullanılmalıdır.

Her grup bir `<col>` elementi ile belirtilir.

`span` eklentisi ile kaç tane sütunun aynı özelliği alacağı belirtilir.

`style` eklentisi ile sütüna verilecek özellikler belirtilir.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>HTML Tablolarında Ortak Grup(Colgroup)

</h2>
<p>Eğer ilk iki kolonu aynı görünüşte yapmak istiyorsak colgroup ve col elementlerini kullanırız.

</p>

<table style="width: 100%;">
<colgroup>
  <col span="2" style="background-color: #D6EEEE">
</colgroup>
<tr>
<th>MON</th>
<th>TUE</th>
<th>WED</th>
<th>THU</th>
<th>FRI</th>
<th>SAT</th>
<th>SUN</th>
</tr>
<tr>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
<td>6</td>
<td>7</td>
</tr>
<tr>
<td>8</td>
<td>9</td>
<td>10</td>
<td>11</td>
<td>12</td>
<td>13</td>
<td>14</td>
</tr>
<tr>
<td>15</td>
<td>16</td>
<td>17</td>
<td>18</td>
<td>19</td>
<td>20</td>
<td>21</td>
</tr>
<tr>
<td>22</td>
<td>23</td>
<td>24</td>
<td>25</td>
<td>26</td>
<td>27</td>
<td>28</td>
</tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/76lf4oz.png)
Legal CSS özellikleri çok azdır. <colgroup> ile birlikte kullanılabilecek Legal CSS özellikleri:

- width

- visibility

- background

- border

### Çoklu <col> Elementi
Farklı stillerle daha fazla sütuna farklı görünüm vermek istiyorsanız, `<colgroup>` sütunun içinde daha fazla `<col>` öğesi kullanın.

```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Çoklu <col> Elementi

</h2>
<p>Farklı stillerle daha fazla sütuna farklı görünüm vermek istiyorsanız, colgroup sütunun içinde daha fazla col öğesi kullanın.

</p>

<table style="width: 100%;">
  <colgroup>
    <col span="2" style="background-color: #D6EEEE">
    <col span="3" style="background-color: pink">
  </colgroup>
<tr>
<th>MON</th>
<th>TUE</th>
<th>WED</th>
<th>THU</th>
<th>FRI</th>
<th>SAT</th>
<th>SUN</th>
</tr>
<tr>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
<td>6</td>
<td>7</td>
</tr>
<tr>
<td>8</td>
<td>9</td>
<td>10</td>
<td>11</td>
<td>12</td>
<td>13</td>
<td>14</td>
</tr>
<tr>
<td>15</td>
<td>16</td>
<td>17</td>
<td>18</td>
<td>19</td>
<td>20</td>
<td>21</td>
</tr>
<tr>
<td>22</td>
<td>23</td>
<td>24</td>
<td>25</td>
<td>26</td>
<td>27</td>
<td>28</td>
</tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/1u0sfok.png)

### Boş Colgroup
Bir tablonun ortasındaki sütunlara stil vermek istiyorsak, önce sütunlar için "boş" bir `<col>` öğesi ekleriz.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Boş Colgroup

</h2>
<p>Bir tablonun ortasındaki sütunlara stil vermek istiyorsak, önce sütunlar için "boş" bir col öğesi ekleriz.

</p>

<table style="width: 100%;">
<colgroup>
  <col span="3">
  <col span="2" style="background-color: pink">
</colgroup>
<tr>
<th>MON</th>
<th>TUE</th>
<th>WED</th>
<th>THU</th>
<th>FRI</th>
<th>SAT</th>
<th>SUN</th>
</tr>
<tr>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
<td>6</td>
<td>7</td>
</tr>
<tr>
<td>8</td>
<td>9</td>
<td>10</td>
<td>11</td>
<td>12</td>
<td>13</td>
<td>14</td>
</tr>
<tr>
<td>15</td>
<td>16</td>
<td>17</td>
<td>18</td>
<td>19</td>
<td>20</td>
<td>21</td>
</tr>
<tr>
<td>22</td>
<td>23</td>
<td>24</td>
<td>25</td>
<td>26</td>
<td>27</td>
<td>28</td>
</tr>
</table>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/tkjl1h3.png)

### Sütunları Saklamak
Sütunları `visibility: collapse` özelliğiyle saklayabiliriz.
```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Sütunları Saklamak

</h2>
<p>Sütunları visibility: collapse özelliğiyle saklayabiliriz.

</p>

<table style="width: 100%;">
<colgroup>
    <col span="2">
    <col span="3" style="visibility: collapse">
  </colgroup>
<tr>
<th>MON</th>
<th>TUE</th>
<th>WED</th>
<th>THU</th>
<th>FRI</th>
<th>SAT</th>
<th>SUN</th>
</tr>
<tr>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td>5</td>
<td>6</td>
<td>7</td>
</tr>
<tr>
<td>8</td>
<td>9</td>
<td>10</td>
<td>11</td>
<td>12</td>
<td>13</td>
<td>14</td>
</tr>
<tr>
<td>15</td>
<td>16</td>
<td>17</td>
<td>18</td>
<td>19</td>
<td>20</td>
<td>21</td>
</tr>
<tr>
<td>22</td>
<td>23</td>
<td>24</td>
<td>25</td>
<td>26</td>
<td>27</td>
<td>28</td>
</tr>
</table>


</body>
</html>
```
![Çıktı](https://i.hizliresim.com/hntovpg.png)

# Bölüm 9

## HTML'de Listeler

### Sırasız(Unordered) HTML Listeleri
Sırasız bir HTML listesi `<ul>` etiketiyle başlar. Listedeki her bir madde `<li>` etiketiyle tanımlanır.

Liste elementleri varsayılan olarak madde işaretleri (küçük siyah daireler) ile işaretlenecektir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Sırasız(Unordered) HTML Listeleri</h2>

<ul>
<li>Selamın Aleyküm</li>
<li>THT</li>
<li>HTML'de Listeler</li>
</ul>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/rvqjyl6.png)

Listelerin başındaki * işaretleri farklı tiplerde olabilir. Bu tipleri belirlemek için CSS'in list-style-type özelliği kullanılır.

Örnek kullanımlar: 
`<ul style="list-style-type:disc;">`

`<ul style="list-style-type:circle;">`

`<ul style="list-style-type:square;">`

`<ul style="list-style-type:none;">`

## Sıralı(Ordered) HTML Listeleri
Sırali bir HTML listesi `<ol>` etiketiyle başlar. Her bir madde `<li>` etiketiyle tanımlanır.
Liste elementleri varsayılan olarak sayılarla işaretlenecektir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Sıralı HTML Listeleri</h2>

<ol>
<li>Real Madrid</li>
<li>Barcelona</li>
<li>Çorumspor</li>
</ol>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/14po1di.png)

## Sıralı HTML Listelerinde type Özelliği
type özelliği `<ol>` etiketiyle birlikte kullanıldığında liste elementlerinin türünü tanımlar.

![Çıktı](https://i.hizliresim.com/6mx6wzr.png)
Örnek kullanımlar:
`<ol type="1">`

`<ol type="A">`

`<ol type="a">`

`<ol type="I">`

`<ol type="i">`

## HTML Açıklama Listeleri(Description Lists)
HTML açıklama listelerini destekler.

Açıklama listesi, bir terimin açıklamasıyla birlikte sıralandığı listelerdir.

`<dl>` etiketi açıklama listelerini tanımlamak için kullanılır. `<dt>` etiketi açılanacak terimi ifade ederken kullanılır,` <dd> `etiketiyse açıklama kısmını içerir.
```

<!DOCTYPE html>
<html>
<body>

<h2>Açıklama listeleri</h2>

<dl>
<dt>Satoshi Nakamoto</dt>
<dd>-Bitcoin'in mucidi olan, kim olduğu bilinmeyen kişi, grup</dd>
<dt>Vitalik</dt>
<dd>-Ethereum'un ağası</dd>
</dl>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/pzeoeln.png)

## Gömülü HTML Listeleri(Nested Lists)
Listeler iç içe oluşturulabilir.
```
<!DOCTYPE html>
<html>
<body>

<h2>Gömülü HTML Listeleri(Nested Lists)

</h2>
<p>Listeler iç içe oluşturulabilir.</p>

<ul>
<li>Blue Team</li>
<li>Green Team
<ul>
<li>İçerik Ekibi</li>
<li>Proje Ekibi</li>
</ul>
</li>
<li>Anka Red Team</li>
</ul>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/4zyrvhp.png)

## CSS ile Yatay Liste Oluşturmak
HTML listeleri CSS kullanılarak farklı görünümlerde oluşturulabilir.
Popüler liste oluşturma yollarından birisi yatay liste oluşturmaktır.
```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
list-style-type: none;
margin: 0;
padding: 0;
overflow: hidden;
background-color: #333333;
}

li {
float: left;
}

li a {
display: block;
color: white;
text-align: center;
padding: 16px;
text-decoration: none;
}

li a:hover {
background-color: #111111;
}
</style>
</head>
<body>

<h2>Navigasyon Menüsü</h2>
<p>Bu örnekte yatay listeleri daha iyi anlaşılır kılmak için navigasyon menüsü oluşturuyoruz.</p>

<ul>
<li><a href="#home">Home</a></li>
<li><a href="#news">News</a></li>
<li><a href="#contact">Contact</a></li>
<li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/chejrma.png)

## Kontrol Listelerinde Sayım
Varsayılan olarak sıralı listeler saymaya 1'den başlar. Eğer farklı bir sayıdan saymaya başlamasını istiyorsanız start özelliğini kullanabilirsiniz.
```
<!DOCTYPE html>
<html>
<body>

<h2>start Özelliği</h2>
<p>Varsayılan olarak sıralı listeler saymaya 1'den başlar. Eğer farklı bir sayıdan saymaya başlamasını istiyorsanız start özelliğini kullanabilirsiniz.

</p>

<ol start="50">
<li>Ahmet</li>
<li>Mahmut</li>
<li>Ayşe</li>
</ol>

<ol type="I" start="50">
<li>Caner</li>
<li>Cülcül</li>
<li>Berkecan</li>
</ol>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/2x33vum.png)

# Bölüm 10

## HTML'de Blok ve Satır İçi Elementler
Her bir HTML elementi varsayılan(default) bir çıktı verir. Bu çıktı elementin hangi türde olduğuna göre değişiklik gösterir.

İki tür çıktı değeri vardır: Blok ve Satır içi

## Blok Seviyesinde Elementler
Blok seviyesinde bir element her zaman yeni bir satırla başlar ve tarayıcı otomatik olarak elementin önüne ve arkasına biraz boşluk ekler.

Blok seviyesinde bir element her zaman mevcut tüm genişliği kapsar.(olabildiğince sağa ve sola doğru yayılır)

Sıklıkla iki blok seviyesinde element kullanılır. Bunlar `<p>` ve `<div>` elementleridir.

`<p>` elementi HTML dökümanlarında bir paragraf tanımlarken kullanılır.

`<div>` elementi HTML dökümanlarında bir bölümü tanımlar.

![Çıktı](https://i.hizliresim.com/ntmtnui.png)

HTML'de blok seviyesindeki elementler:
```
<address>
<article>
<aside>
<blockquote>
<canvas>
<dd>
<div>
<dl>
<dt>
<fieldset>
<figcaption>
<figure>
<footer>
<form>
<h1> - <h6>
<header>
<hr>
<li>
<main>
<nav>
<noscript>
<ol>
<p>
<pre>
<section>
<table>
<tfoot>
<ul>
<video>
```
## Satır İçi Elementler
Satır içi bir element yeni bir satırla başlamaz.

Satır içi elementler sadece gerektiği kadar boşluğu doldururlar.
![Çıktı](https://i.hizliresim.com/r8sfd0q.png)
HTML'de satır içi elementler:
```
<a>
<abbr>
<acronym>
<b>
<bdo>
<big>
<br>
<button>
<cite>
<code>
<dfn>
<em>
<i>
<img>
<input>
<kbd>
<label>
<map>
<object>
<output>
<q>
<samp>
<script>
<select>
<small>
<span>
<strong>
<sub>
<sup>
<textarea>
<time>
<tt>
<var>
```
Not: Bir satır içi element blok seviyesinde bir elementi bünyesinde barındıramaz.

## <div> Elementi
`<div>` elementi sıklıkla diğer HTML elementlerini kapsayacağı şekilde kullanılır.

`<div>` elementi özniteliğe ihtiyaç duymaz. Fakat style, class ve id ortaktır.

CSS ile birlikte kullanıldığında içeriğin bloklarını şekillendirebilirsiniz.
```
<!DOCTYPE html>
<html>
<body>

<div style="background-color:black;color:white;padding:20px;">
  <h2>THT</h2>
  <p>Türk Hack Team 2002 yılında Arsenik tarafından kurulmuş olan siber güvenlik platformudur.</p>
  <p>Türk Hack Team bünyesinde çeşitli ekipleri barındıran Türkiye'nin en büyük siber güvenlik platformudur.</p>
</div>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/kgzvge2.png)

## <span> Elementi
`<span>` elementi bir dökümanın bir parçasını veya bir metnin bir parçasını işaretlemek için kullanılan satır içi bir kapsayıcıdır.

`<span>` elementi özniteliğe ihtiyaç duymaz. Fakat style, class ve id ortaktır.

CSS ile birlikte kullanıldığında metnin stilini değiştirebilirsiniz.
```

<!DOCTYPE html>
<html>
<body>

<h1>span Elementi</h1>

<p>THT'nin en iyi içerik üreten ekibi <span style="color:green;font-weight:bold">Green Team</span> forum üyeleri için detaylı içerikler hazırlarlar.  <span style="color:blue;font-weight:bold">Basın Medya</span> ekibi ise bu içeriklerin tanıtmını yapmaktadır.</p>

</body>
</html>

```
![Çıktı](https://i.hizliresim.com/hunn0sy.png)

## HTML'de class Özelliği
class özelliği bir HTML elementinin sınıfını belirtmek için kullanılır.

Birden fazla HTML elementi aynı sınıfta olabilir.

class özelliği genellikle bir style sayfasında bir sınıf adını işaret etmek için kullanılır. Belirli sınıf adına sahip öğelere erişmek ve bunları değiştirmek için bir JavaScript tarafından da kullanılabilir.

Aşağıdaki örnekte, "city" değerine sahip bir sınıf özelliğinde üç `<div>` elemanımız var. Üç <div> elementinin tümü, başlık bölümündeki .city style tanımına göre eşit şekilde stillendirilecektir:
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  border: 2px solid black;
  margin: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<div class="city">
<h2>Londra</h2>
<p>Londra İngiltere'nin başkentidir.</p>
</div>

<div class="city">
<h2>Paris</h2>
<p>Paris Fransa'nın başkentidir.</p>
</div>

<div class="city">
<h2>Tokyo</h2>
<p>Tokyo Japonya'nın başkentidir..</p>
</div>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/of91wr8.png)

İpucu: class özelliği her HTML elementinde kullanılabilir.

Not: class name(sınıf özelliği) büyük harf-küçük harf duyarlılığına sahiptir.(case sensitive)

## class Özelliği için Sözdizimi(syntax)
Bir sınıf oluşturabilmek için bir nokta (.) karakteri ve ardından bir sınıf adı(class name) yazın. Ardından, küme parantezleri {} içinde CSS özelliklerini tanımlayın.
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>
</head>
<body>

<h2>class Özelliği</h2>
<p>"city" sınıf adı ile elementleri şekillendirmek için CSS kullanın:</p>

<h2 class="city">Londra</h2>
<p>Londa İngiltere'nin başkentidir.</p>

<h2 class="city">Paris</h2>
<p>Paris Fransa'nın başkentidir.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo Japonya'nın başkentidir.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/mpthjs6.png)

## Çoklu Sınıflar(Multiple Classes)
HTML elementleri birden fazla sınıfa ait olabilirler.

Çoklu sınıflar tanımlamak için sınıf adlarını bir boşlukla ayırın, örneğin `<div class="city main">`. Öğe, belirtilen tüm sınıflara göre şekillendirilecektir.
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}

.main {
  text-align: center;
}
</style>
</head>
<body>

<h2>Çoklu Sınıflar(Multiple Classes)

</h2>
<p>HTML elementleri birden fazla sınıfa ait olabilirler.

</p>

<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>

</body>
</html>
```

![Çıktı](https://i.hizliresim.com/sz5ha81.png)

## Farklı Elementler Aynı Sınıfı Paylaşabilir
Farklı HTML elementleri aynı sınıf adını işaret edebilirler.

Aşağıdaki örnekte `<h2>` ve `<p>` elementleri "city" sınıfını işaret etmektedir. Ayrıca aynı stili paylaşacaklardır:
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Farklı Elementler Aynı Sınıfı Paylaşabilir

</h2>

<p>İki HTML elementi aynı etiket ismine sahip olmasa bile aynı sınıfı işaret edebilirler ve CSS ile birlikte aynı görünümü elde edebilirler.</p>

<h2 class="city">Paris</h2>
<p class="city">Paris Fransa'nın başkentidir.</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/3jln0aq.png)

## class Özelliğini JavaScript'te Kullanmak

Sınıf adı(class name), belirli elementler için belirli görevleri gerçekleştirmek amacıyla JavaScriptte kullanılabilir.

JavaScript, `getElementsByClassName()` yöntemiyle belirli bir sınıf adına sahip öğelere erişebilir.
```
<!DOCTYPE html>
<html>
<body>

<h2>class Özelliğini JavaScript'te Kullanmak</h2>
<p>"city" sınıf adıyla tüm özellikleri saklamak için butona basınız</p>

<button onclick="myFunction()">Elementleri sakla</button>

<h2 class="city">London</h2>
<p>Londra İngiltere'nin başkentidir.</p>

<h2 class="city">Paris</h2>
<p>Paris Fransa'nın başkentidir.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo Japonya'nın başkentidir.</p>

<script>
function myFunction() {
  var x = document.getElementsByClassName("city");
  for (var i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
}
</script>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/1tsextg.png)
"Elementleri sakla" butonuna bastığımızda ekrandaki çıktı:
![Çıktı](https://i.hizliresim.com/jp8x1vu.png)

## id Özelliği

id özelliği HTML elementleri için eşsiz bir id tanımlamak için kullanılır.
Bir HTML dökümanında aynı id'ye sahip birden fazla element bulunamaz.
id özelliği, bir style sayfasında belirli bir stil bildirimine işaret etmek için kullanılır. Ayrıca JavaScript tarafından belirli bir kimliğe sahip öğeye erişmek ve bunları işlemek için kullanılır.
id özelliği için sözdizimi: `#` işaretinden sonra id ismini yazarız. Sonrasında CSS özelliklerinden `{}` işaretlerini kullanırız.

Aşağıdaki örnekte, "myHeader" id'sine işaret eden bir `<h1>` elemanımız var. Bu `<h1>` öğesi, head bölümündeki #myHeader style tanımına göre biçimlendirilecektir:

```
<!DOCTYPE html>
<html>
<head>
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>
</head>
<body>

<h2>id Özelliği</h2>
<p>
"myHeader" kimliğine sahip bir öğeye stil vermek için CSS kullanın:</p>

<h1 id="myHeader">My Header</h1>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/k9icfqt.png)

Not: id ismi küçük harf-büyük harf duyarlılığına sahiptir.(case sensitive)

Not: id isimleri en az bir karakter içermek zorundadır. id isimleri numara ile başlayamaz ve boşluk içeremez.

## id Özelliğini JavaScript'te Kullanmak

id özelliği, JavaScript tarafından belirli öğe için bazı görevleri gerçekleştirmek için kullanılabilir.

JavaScript, `getElementById()` yöntemiyle belirli bir kimliğe sahip bir öğeye erişebilir.
```
<!DOCTYPE html>
<html>
<body>

<h2>id Özelliğini JavaScript'te Kullanmak</h2>
<p>id özelliği, JavaScript tarafından belirli öğe için bazı görevleri gerçekleştirmek için kullanılabilir.



JavaScript, getElementById() yöntemiyle belirli bir kimliğe sahip bir öğeye erişebilir</p>

<h1 id="myHeader">Merhaba THT</h1>
<button onclick="displayResult()">Metni Değiştir.</button>

<script>
function displayResult() {
  document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/nt4m88r.png)

## HTML'de Iframe
Bir web sayfasını bir web sayfasının içinde görüntülemek için Iframe kullanılır.
![Çıktı](https://i.hizliresim.com/teb1n1q.png)
## Iframe ifadesinin sözdizimi(Syntax)

`<iframe>` etiketi satır içi bir çerçeve oluşturmak için kullanılır.
Satır içi bir çerçeve bir dökümanı mevcut HTML dökümanına gömmek için kullanılır.

Kullanım biçimi:
`<iframe src="url" title="description"></iframe>`

İpucu: `<iframe>` için her zaman bir `<title>` özelliği eklemek iyi bir uygulamadır. Bu, ekran okuyucular tarafından iframe içeriğinin ne olduğunu okumak için kullanılır.

## Iframe - Yüksekliği ve genişliği ayarlamak
Iframe'in genişliğini ve yüksekliğini ayarlamak için `height` ve `width` özelliklerini kullanırız.
Kullanım biçimi:
`<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>`
veya style özelliğini kullanarak CSS'in height ve width özelliklerini kullanabilirsiniz.
Kullanım biçimi:
`<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>`

## Iframe - Sınırları Kaldırmak
Varsayılan olarak iframe çevresinde bir sınırla birlikte oluşur. Bu sınırı kaldırmak için style özelliğini CSS'in border özelliğiyle kullanabiliriz.
`<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>`
Ayrıca CSS ile birlikte iframe'in sınırının boyutunu ve rengini değiştirebilirsiniz.
`<iframe src="demo_iframe.htm" style="border:2px solid red;" title="Iframe Example"></iframe>`

## Iframe - Bağlantı Hedefi
Bir iframe, bir bağlantı için hedef çerçeve olarak kullanılabilir.

Bağlantının target özelliği iframe'in name özelliğini anmalıdır.
```
<!DOCTYPE html>
<html>
<body>

<h2>Iframe - Bağlantı Hedefi

</h2>

<iframe src="demo_iframe.htm" name="iframe_a" height="300px" width="100%" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>

<p>Bir bağlantının hedef niteliği, bir iframe'in adıyla eşleştiğinde, bağlantı iframe'de açılır..</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/oa4klhx.png)

## HTML ve JavaScript
JavaScript HTML sayfalarını daha dinamik ve etkileşimli kılar.

### HTML'de <script> Etiketi
`<script>` etiketi kullanıcı tarafında bir script tanımlamak için kullanılır.(JavaScript)

`<script>` öğesi ya script deyimleri içerir ya da src özelliği aracılığıyla harici bir komut dosyasına işaret eder.

JavaScript'in yaygın kullanımları, görüntü işleme, form doğrulama ve dinamik içerik değişiklikleridir.

JavaScript, bir HTML elementi seçmek için çoğunlukla `document.getElementById()` yöntemini kullanır.

JavaScript ne yapabilir?

* Javascript içeriği değiştirmek için kullanılabilir.
* Javascript stil değiştirmek için kullanılabilir. 
* Javascript özellik değiştirmek için kullanılabilir.

### <noscript> Etiketi
`<noscript>` etiketi tarayıcılarında komut dosyalarını devre dışı bırakmış veya komut dosyalarını desteklemeyen bir tarayıcıya sahip kullanıcılara gösterilecek alternatif bir içeriği tanımlar.
```
<!DOCTYPE html>
<html>
<body>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "Merhaba JavaScript!";
</script>

<noscript>Üzgünüm, tarayıcınız JavaScript'i desteklemiyor.</noscript>

<p>JavaScript desteği olmayan bir tarayıcı, noscript öğesinin içine yazılan metni gösterecektir.</p>
 
</body>
</html>
```
![Çıktı](https://i.hizliresim.com/ohc9j5x.png)
Eğer tarayıcımız JavaScript'i desteklemiyor olsaydı "Üzgünüm, tarayıcınız JavaScript'i desteklemiyor." çıktısını verecekti.

## HTML'de Dosya Yolları
Dosya yolu, bir web sitesinin klasör yapısındaki bir dosyanın konumunu tanımlar.

Dosya yolları, aşağıdakiler gibi harici dosyalara bağlanırken kullanılır:

-Web sayfaları

-Görseller

-Style sheets

-JavaScripts

#### Örnek Dosya Yolları
![Çıktı](https://i.hizliresim.com/dc1ouxs.png)

### Mutlak Dosya Yolları
Mutlak dosya yolu, bir dosyanın tam URL'sidir:
`<img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">`

### Relative Dosya Yolları
Göreli bir dosya yolu, geçerli sayfaya göre bir dosyaya işaret eder.

Aşağıdaki örnekte, dosya yolu, geçerli web'in kökünde bulunan resimler klasöründeki bir dosyaya işaret eder:
`<img src="/images/picture.jpg" alt="Mountain">`

# Bölüm 11

## HTML'de <head> Elementi
`<head> elementi <title>,<style>,<meta>,<link>,<script> ve <base>` etiketlerini kapsayan bir elementtir.
`<head>` elementi metadata'yı kapsayan bir elementtir. `<html>` ve `<body>` etiketlerinin arasında yer alır.

Metadata HTML dökümanı hakkındaki verilerdir. Metadata çıktı olarak görünmez.

Metadata genellikle dökümanın başlığını(title), karakter setini, stilini(styles), scriptlerini ve meta bilgisini tanımlar.

## <title> Elementi

`<title>` elementi dökümanın başlığını tanımlamak için kullanılır. Başlık sadece karakter içermelidir.(text-only). Başlık internet tarayıcısının sekmeler kısmında görünen metindir.

`<title>` tüm HTML dökümanlarında gereklidir.

Sayfanızın başlığı SEO(Arama Motoru Optimizasyonu) için önemli bir parametredir. Sayfa başlıkları arama motorlarının algoritmaları tarafından listelenecek sitelerin kararlaştırılmasında kullanılır.

## <style> Elementi
`<style>` elementi HTML sayfalarının biçimini belirlemek için kullanılır.

## <link> Elementi
`<link>` elementi mevcut döküman ile bir dış kaynak arasındaki ilişkiyi tanımlar.

`<link>` etiketi çoğunlukla harici style sheet(stil sayfalarına) bağlanmak için kullanılır.

## <meta> Elementi

`<meta>` elementi karakter setini, sayfa açıklamasını, anahtar kelimeleri, dökümanın yazarını ve viewport özelliklerini belirlemek için kullanılır.

Metadata sayfada çıktı olarak gösterilmeyecektir ancak tarayıcı tarafından kullanılacaktır.(Tarayıcı sayfanın nasıl yükleneceğine dadir bilgi edinir.) Metadata arama motorları ve diğer web servisleri tarafından da kullanılır.

Örnek Kullanımlar:

Kullanılan karakter setini belirtmek için: `<meta charset="UTF-8">`

Arama motorları için anahtar kelime belirtme: `<meta name="keywords" content="HTML, CSS, JavaScript">`

Web sitesine bir açıklama tanımlamak için: `<meta name="description" content="HTM Egitimi">`

Sayfanın yazarını tanımlamak için: `<meta name="author" content="Aziz - vancoondehni">`

Dökümanı her 30 saniyede bir yenilemek için: `<meta http-equiv="refresh" content="30">`

Web sitenizin tüm cihazlarda iyi görünmesini sağlamak için görünüm alanını(viewport) ayarlama: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

`<meta>` etiketlerinin örneği:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="description" content="HTM ogrenelim">
  <meta name="keywords" content="HTML, CSS, JavaScript">
  <meta name="author" content="vancoondehni">
</head>
<body>

<p>Tüm meta bilgileri head kısmının içerisinde belirtilir.</p>

</body>
</html>
```

## Görünüm Alanı(viewport) Ayarları
Viewport kullanıcıların internet sitesindeki görebildikleri alandır. Bu alan cihazdan cihaza, ekran boyutuna göre değişiklik gösterir.

Tüm web sitelerinde `<meta>` elementinin aşağıdaki kodunu bulundurmalısınız:
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
Yukarıdaki kod, tarayıcıya sayfanın boyutlarını ve ölçeklendirmesini nasıl kontrol edeceğine dair talimatlar verir.

`width=device-width` kısmı ekran genişliğini cihazın genişliğine uyarlayacaktır.
`initial-scale=1.0` kısmı sayfa tarayıcı tarafından ilk yüklendiğinde başlangıç yakınlaştırma düzeyini ayarlar.

viewport meta etiketi olmadan ve olduğunda bir sayfanın nasıl göründüğüne bakalım:
![Çıktı](https://i.hizliresim.com/o113k8y.png)

## <script> Elementi
`<script>` elementi istemci tabanlı JavaScriptler oluşturmak için kullanılır.

Örnek: Aşağıdaki JavaScript kodunda `:demo` idsine sahip element "Merhaba THT" yazmaktadır.
```
<!DOCTYPE html>
<html>
<head>
  <title>THT - HTML Öğrenelim</title>
  <script>
  function myFunction() {
    document.getElementById("demo").innerHTML = "Merhaba THT";
  }
  </script>
</head>
<body>

<h1>THT</h1>
<p id="demo">Selamlar</p>
<button type="button" onclick="myFunction()">Deneme</button>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/c5x2wwm.png)
Deneme butonuna tıkladıktan sonraki çıktı:
![Çıktı](https://i.hizliresim.com/1fbgcdq.png)

## <base> Elementi
`<base>` elementi, bir sayfadaki tüm göreli URL'ler için temel URL'yi veya hedefi belirtir.

`<base>` etiketi, bir href veya target özelliğini veya her ikisini birden içermelidir.

Bir dökümanda sadece bir `<base>` elementi bulunabilir.
```
<!DOCTYPE html>
<html>
<head>
  <base href="turkhackteam.org" target="_blank">
</head>
<body>

<h1>base elementi</h1>

<p><img src="https://www.turkhackteam.org/styles/v1/tht/logo.png" width="24" height="39" alt="Logo"> - Görüntü için yalnızca göreli bir adres belirttiğimize dikkat edin. Head bölümünde bir temel URL belirttiğimizden, tarayıcı "https://www.turkhackteam.org/styles/v1/tht/logo.png"adresindeki resmi arayacaktır.</p>

<p><a href="tags/tag_base.asp">HTML base etiketi</a> - Dikkat edin linke tıkladığınızda  target="_blank" özelliği bulunmadığı halde yan sekmede açılıyor. Bunun nedeni, temel öğenin hedef niteliğinin "_blank" olarak ayarlanmış olmasıdır..</p>

</body>
</html>
```
![Çıktı](https://i.hizliresim.com/7bv5jtj.png)

## HTML'de Düzen Öğeleri ve Teknikleri(HTML Layout Elements and Techniques)
Web siteleri genellikle içeriği birden çok sütunda görüntülerler.

HTML birkaç semantik elemente sahiptir. Bu semantik elementleri web sayfasının farklı kısımlarını tanımlamakta kullanılır.
![Çıktı](https://i.hizliresim.com/elm1j6r.png)
- `<header>` - Bir döküman veya kısım için başlık tanımlarken kullanılır.

- `<nav>` - Bir dizi gezinme bağlantısı tanımlarken kullanılır.

- `<section>` - Bir dökümandaki bir kısmı tanımlarken kullanılır.

- `<article>` - Bağımsız(kendi kendine yeten) bir içerik tanımlar.

- `<aside>` - İçeriğin kenarına bir içerik tanımlar.(kenar çubuğu gibi)

- `<footer>` - Bir belge veya bölüm için bir altbilgi tanımlar.

- `<details>` - Kullanıcın istediği zaman açıp kapatabileceği ek detay tanımlamak için kullanılır.

- `<summary>` - <details>elementi için bir başlık tanımlar.

## HTML'de Düzen Teknikleri
Çok sütunlu düzenler oluşturmak için dört farklı teknik vardır.

Her tekniğin artıları ve eksileri vardır:

- CSS framework

- CSS float property

- CSS flexbox

- CSS grid

## CSS Frameworks
Eğer düzeni hızlıca oluşturmak istiyorsanız CSS frameworklerinden birisini kullanabilirsiniz.(örnek: Bootstrap)

## CSS Float Düzeni
Tüm düzeni CSS'in float özelliğiyle oluşturmak yaygın bir durumdur. Float'ı öğrenmesi kolaydır. Sadece float ve clear özelliklerinin nasıl çalıştığını hatırlamanız gerekir.

Eksi yönleri: Float elemanlar esnek şekilde sitenizi oluşturmanızda size zarar verebilecek belge akışına bağlıdır.

## CSS Flexbox Düzeni
Flexbox, sayfa düzeninin farklı ekran boyutlarını ve farklı görüntüleme cihazlarını barındırması gerektiğinde öğelerin öngörülebilir şekilde davranmasını sağlar.

## CSS Grid Düzeni
Grid Düzen Modülü, satırlar ve sütunlar içeren ızgara tabanlı bir düzen sistemi sunarak, kayan noktalar ve konumlandırma kullanmak zorunda kalmadan web sayfalarını tasarlamayı kolaylaştırır.

## HTML'de Duyarlı Web Tasarımı
Duyarlı web tasarımı demek internet sitelerinin tüm cihazlarda güzel gözükmesini sağlamaktır.

Duyarlı bir web tasarımı, farklı ekran boyutları ve görünüm alanları için otomatik olarak ayarlanacaktır.
Örnek kullanım(Kaynak W3Schools):
![Çıktı](https://www.w3schools.com/css/img_temp_startpage.jpg)

Duyarlı bir web tasarımı yapmak için HTML ve CSS'in resize, hide, shrink veya enlarge gibi özelliklerini kullanarak sitemizi tasarlamamız gerekir. (Bu şekilde tasarlandığında masaüstü cihazınızda, tabletinizde, telefonunuzda ve laptopta güzel gözükecektir.)

Bunun için viewport özelliğini ayarlamamız gerekir. (Yukarıda detaylı bahsettiğim için tekrardan detaylı değinmeyeceğim)

`<meta name="viewport" content="width=device-width, initial-scale=1.0">`

## Duyarlı Görseller
Duyarlı görseller tarayıcınızın boyutuna göre ekrana sığan görsellerdir. Bunun için aşağıdaki şekilde kullanırız.
Daha doğru bir yapı için max-width özelliği de kullanılabilir.

`<img src="img_girl.jpg" style="max-width:100%;height:auto;">`

## Tarayıcı Genişliğine Göre Farklı Görseller Gösterme
`<picture>` elementi farklı ekran boyutlarında farklı görsellerin çıktı olarak verilmesini sağlar.
```
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h2>Tarayıcı Genişliğine Göre Farklı Görseller Gösterme

</h2>
<p>Tarayıcınızın boyutunu 600px ve 1500px olarak değiştirin</p>

<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

</body>
</html>
```

## Duyarlı Metin Boyutu

Metin boyutu, "görünüm alanı genişliği" anlamına gelen bir "vw" birimi ile ayarlanabilir.

Bu şekilde metin boyutu tarayıcı penceresinin boyutunu takip edecektir.
`<h1 style="font-size:10vw">Selam THT</h1>`

## Media Queries(Medya Sorguları)
Görselleri ve metinleri yeniden boyutlandırabilmek için yukarıda bahsettiğimiz özelliklerin yanı sıra media queries de kullanılabilir.
Media Queries ile birlikte farklı ekran boyutları için farklı stiller oluşturabilirsiniz.

Aşağıdaki üç div öğesinin büyük ekranlarda yatay olarak görüntüleneceğini ve küçük ekranlarda dikey olarak istifleneceğini görmek için tarayıcı penceresini yeniden boyutlandırın:
```
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.left {
  background-color: #2196F3;
  padding: 20px;
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  background-color: #f1f1f1;
  padding: 20px;
  float: left;
  width: 60%; /* The width is 60%, by default */
}

.right {
  background-color: #04AA6D;
  padding: 20px;
  float: left;
  width: 20%; /* The width is 20%, by default */
}

/* Use a media query to add a break point at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
</style>
</head>
<body>

<h2>Media Queries(Medya Sorguları)

</h2>
<p>Tarayıcı boyutunu değiştirin.</p>

<p>Bu çerçeveyi yeniden boyutlandırırken 800 pikselde kesme noktasına ulaştığınızdan emin olun.</p>

<div class="left">
  <p>Sol Menü</p>
</div>

<div class="main">
  <p>Ana İçerik</p>
</div>

<div class="right">
  <p>Sağ İçerik</p>
</div>

</body>
</html>
```

# Bölüm 12

## HTML'de Bilgisayar Kodları
HTML, kullanıcıdan alınan bilgiyi ve bilgisayar kodunu tanımlama için çeşitli elementleri içerir.
Örnek:
```
<!DOCTYPE html>
<html>
<body>

<h2>Bilgisayar kodları</h2>
<p>Bazı programlama kodları</p>

<code>
x = 5;
y = 6;
z = x + y;
</code>

</body>
</html>
```
## Klavyeden Girdi Almak - `<kbd>` Elementi
`<kbd>` elementi klavyeden bir girdi almak için kullanılır. Alınan içerik tarayıcının varsayılan monospace fontunda görülür.
![Çıktı](https://i.hizliresim.com/hwu0pr4.png)

## Program Çıktısı - `<samp>` Elementi
Bir bilgisayar programından çıktı elde etmek için `<samp>` elementi kullanılır. Programın içerisindeki içerik tarayıcı tarafından varsayılan olarak monospace fontunda verilir.
![Çıktı](https://i.hizliresim.com/hurw7dv.png)

## `<code>` Elementi
`<code>` elementi, bir bilgisayar kodunu tanımlamak için kullanılır. İçindeki içerik, tarayıcının varsayılan monospace yazı tipinde görüntülenir.
![Çıktı](https://i.hizliresim.com/7dhller.png)
`<code>` elementinin fazladan boşluk ve satır sonlarını korumadığına dikkat edin. Bunu düzeltmek için `<code>` elementini bir `<pre>` öğesinin içine koyabilirsiniz.
![Çıktı](https://i.hizliresim.com/5u7vh8f.png)

## `<var>` Elementi
HTML'de `<var>`elementi programlamada bir değişken tanımlarken kullandığımız variable ile aynı işlevi görür. İçerisindeki içerik italik şekilde gösterilir.
![Çıktı](https://i.hizliresim.com/ov2824f.png)

## Semantik Elementler nelerdir?
Semantik Elementler nelerdir?

Bir semantik element tarayıcıya ve geliştiriciye hangi amaçla kullanıldığını çok iyi şekilde açıklayan elementlerdir.

Semantik olmayan elementlere örnek verecek olursak: `<div>` ve `<span>` (İçerik hakkında bir bilgi vermiyorlar)

Semantik elementlere örnek verecek olursak: `<form>,<table> ve <article>` (Anlaşılır şekilde içeriği tanımlar)

### HTML'de Semantik elementler nelerdir?
![Semantik](https://i.hizliresim.com/dy4owto.png)


## '<section>' Elementi

'<section>' elementi bir dökümandaki bir kısımı tanımlamak için kullanılır.

Bu elementin nerelerde kullanılabileceğine yönelik örnekler:
- Bölümler(Chapters)
- Giriş(Introduction)
- Haber Öğeleri
- İletişim Bilgileri(Contact Info)

Bir web sayfası giriş, içerik ve iletişim bilgileri için bölümlere ayrılabilir.

Örnek:
```
<section>
<h1>TürkHackTeam</h1>
<p>Türkiye'nin en büyük siber güvenlik platformu. Bu içerik vancoondehni(Aziz) tarafından THT için hazırlanmıştır.</p>
</section>

<section>
<h1>İletişim</h1>
<p>Github - kartalaziz.</p>
</section>
```
## `<article>` Elementi

`<article>` elementi bağımsız, kendi kendine yeten bir içeriği tanımlarken kullanılır.

`<article>` elementinin kullanıldığı yerler:
- Forum postlarında
- Blog postlarında
- Kullanıcı yorumlarında
- Ürün kartlarında
- Gazete haberlerinde

Örnek:
```
<article>
<h2>Google Chrome</h2>
<p>Chrome 2008 yılında Google tarafından geliştirilmiş olan bir tarayıcıdır.</p>
</article>

<article>
<h2>Mozilla Firefox</h2>
<p>Firefox Mozilla şirketi tarafından geliştirilmiş olan bir tarayıcıdır..</p>
</article>
```
!Önemli! `<article>` elementi kendi kendine yeten, bağımsız bir elementtir. Bu elementi `<section>` elementinin içerisinde kullanamayız.

## `<header>` Elementi

`<header>` elementi, tanıtım içeriği için bir dizi gezinme bağlantısını temsil eder.
Bir <header> elementi tipik olarak aşağıdakileri içerir:
- Bir veya daha fazla heading elementi`(<h1>-<h6>)`
- Logo veya ikon
- Yazar bilgisi

NOT: Bir HTML dökümanında birden fazla `<header>` elementine sahip olabilirsiniz. Ancak `<header>` elementi `<footer>`,`<address>` veya başka bir `<header>` elementi içerisinde bulunamaz.

Örnek:
```
<article>
  <header>
    <h1>THT</h1>
    <p>THT Türkiye'nin en büyük siber güvenlik platformu</p>
  </header>
  <p>THT faydalı içerikler üreten ekipleri barındıran ve gelişime odaklanan bir forumdur.</p>
</article>
```
## `<footer>` Elementi
`<footer>` elementi bir döküman veya bölüm için bir footer(altbilgi) tanımlamak için kullanılır.
Bir `<footer>` elementi tipik olarak aşağıdakileri içerir:
- Yazar bilgisi
- Copyright bilgisi
- İletişim bilgisi
- Site haritası
- En iyi bağlantılara dön
- İlgili dökümanlar

Bir dökümanda birkaç `<footer>` elementine sahip olabilirsiniz.

Örnek:
```
<footer>
  <p>Yazar: Aziz</p>
  <p><a href="mailto:bilmemnde@bilmemsi.com">bilmemne.com</a></p>
</footer>
```

## `<nav>` Elementi
`<nav>` elementi bir navigasyon bağlantısı tanımlamak için kullanılır.
Örnek:
```
<nav>
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```
## `<aside>` Elementi
`<aside>` elementi yerleştirildiği içeriğin dışında bazı içerikleri tanımlar (kenar çubuğu gibi)
`<aside>` elementi içeriği, çevreleyen içerikle dolaylı olarak ilişkili olmalıdır.
```
<html>
<head>
<style>
aside {
  width: 30%;
  padding-left: 15px;
  margin-left: 15px;
  float: right;
  font-style: italic;
  background-color: lightgray;
}
</style>
</head>
<body>

<p>THT</p>

<aside>
<p> Yazar: vancoondehni(Aziz).</p>
</aside>

<p>GreenTeam</p>
<p> HTML Öğrenelim Serisi </p>

</body>
</html>
```
## `<figure>` ve `<figcaption>` Elementleri
`<figure>` elementi, çizimler, diyagramlar, fotoğraflar, kod listeleri gibi bağımsız içerikleri belirtir.
`<figcaption>` elementi, bir `<figure>` elementi için bir resim yazısı tanımlar.
`<img>` elementi gerçek görüntüyü/illüstrasyonu tanımlar.

Örnek:
```
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure>
```
## HTML'de Stil Önerileri
- Bir dökümanda her zaman dökümanın tipini belirtin.
Örneğin:
`<!DOCTYPE html>`

- Element isimlerinde küçük harfleri kullanın. (HTML case sensitive değildir bu sebeple `<b>` veya `<B>` aynı işlevi görür fakat görünüm açısından küçük harfleri kullanmak daha faydalıdır.)

- HTML'de tüm elementleri kapatmak zorunda değilsiniz. Örneğin <p> elementini kapatmanıza gerek yok. Fakat kapatmanız daha iyi olacaktır.

- Görseller için her zaman alt,width ve height özelliğini belirtin.

- `<title>` elementini eklemeyi asla unutmayın. (SEO sıralamanız için çok önemli bir nokta)

- Her zaman lang özelliğini kullanarak web sayfasının dilini belirtiniz. Arama motorları ve tarayıcılar için önemli bir nokta.

- Meta data(Doğru arama motoru indeksini yakalamak için metadata tanımlamasını kullanın)

- Viewportu ayarlama(Farklı cihazlarda sitenin görünümününün bozulmaması için bu özelliği kullanın.)

## HTML Entities
Reserved karakterler olarak adlandırılan karakterler vardır. `>` ve `<` gibi

Tarayıcılar bu işaretleri etiketlerle karıştırabilir.

Bundan kaçınmak için `<` işareti yerine `&lt;` veya `&#60` ifadesini kullanmalıyız.

Bazı reserved karakterler:
![Reserved](https://i.hizliresim.com/n4pyr5q.png)
## HTML'de Semboller
Çoğu matematiksel, teknik ve para birimi simgesi normal bir klavyede bulunmaz. HTML sayfasına bu tür semboller eklemek için entity adını veya entity numarasını kullanabilirsiniz.

Örnek:
![Örnek](https://i.hizliresim.com/2ls46tm.png)

### HTML Tarafından Desteklenen Bazı Matematiksel Semboller
Tam liste: https://www.w3schools.com/charsets/ref_utf_math.asp

Ok işaretleri: https://www.w3schools.com/charsets/ref_utf_arrows.asp
Para birimi işaretleri: https://www.w3schools.com/charsets/ref_utf_currency.asp
Diğer işaretler: https://www.w3schools.com/charsets/ref_utf_symbols.asp

## HTML'de Emojiler
Emojiler UTF-8 karakter setleridir.
UTF_8 neredeyse tüm karakterleri ve sembolleri içerir.

## charset Özelliği
Bir HTML sayfasının doğru şekilde çıktı verebilmesi için tarayıcının sayfada kullanılan karakter setlerini bilmesi gerekir. Bunu için `<meta>` etiketinde kullanılan karakter seti belirtilir.
Örneğin: `<meta charset="UTF-8">`

Tüm emojilerin listesi: https://www.w3schools.com/charsets/ref_emoji.asp

# Bölüm 13
