# Hafta 5 · Kapalı türev, ters fonksiyon ve logaritmik türev

**Kapsam.** Q1–Q8, MT2'nin kapalı türev, monotonluk, ters fonksiyon ve üstel-logaritmik türev başlıklarını çalıştırır. Final tekrarı için de temel oluşturur. [Özgün soru kâğıdı](hafta-05.pdf)

## Q1 · Kapalı eğride teğet

$2(x^2+y^2)^2=4(x^2-y^2)$ eğrisinde **(a)** $y'$, **(b)** yatay teğetli noktalar ve **(c)** $y''$ isteniyor. Yöntem olarak önce $s=x^2+y^2$ yazıp türev al. Paydanın sıfır olduğu noktaları ayrıca incele.

<details><summary>Çözümü ve tekil nokta kontrolünü aç</summary>

**(a)** $s^2=2(x^2-y^2)$ bağıntısı $2s(2x+2yy')=4x-4yy'$ verir. Terimleri toplayınca $x(s-1)+y(s+1)y'=0$. Böylece $y\ne0$ için

$$y'=\frac{x(1-s)}{y(1+s)}.$$

**(b)** Pay sıfırsa $x=0$ veya $s=1$. $x=0$ özgün bağıntıda yalnız orijini verir. $s=1$ için $x^2+y^2=1$ ve $x^2-y^2=1/2$ olduğundan dört nokta $(\pm\sqrt3/2,\pm1/2)$ elde edilir (işaretler bağımsız). Orijinde türev formülü $0/0$ verir. Orijinden geçen türevlenebilir bir dalda $y/x\to m$ ise bağıntıyı $x^2$ ile bölünce $x^2(1+(y/x)^2)^2=2(1-(y/x)^2)$, dolayısıyla $m^2=1$. Orijin yatay teğet vermez. Diğer $y=0$ noktalarında $x=\pm\sqrt2$ ve teğet diktir.

**(c)** $p=y'$ yazıp $x(s-1)+y(s+1)p=0$ eşitliğini yeniden türet. $s'=2x+2yp$ kullanılırsa

$$y''=-\frac{(3x^2+y^2-1)+4xyp+(x^2+3y^2+1)p^2}{y(s+1)}.$$

Burada $p$ (a)'daki ifadedir. Kontrol için yatay teğette $p=0$ yazılabilir. Üstteki iki noktada ikinci türev negatiftir.

</details>

## Q2 · Artma ve azalma aralıkları

$f(x)=3x^4-4x^3-12x^2+5$ için türevin işaret tablosunu kur.

<details><summary>Çözümü aç</summary>

$f'(x)=12x^3-12x^2-24x=12x(x-2)(x+1)$. Kritik sayılar sırasıyla $-1,0,2$. Basit köklerin her birinde işaret değişir. $x>2$ için işaret pozitif olduğundan soldan sağa işaret dizisi $-,+,-,+$ olur. Fonksiyon $(-1,0)$ ve $(2,\infty)$ üzerinde artar, $(-\infty,-1)$ ve $(0,2)$ üzerinde azalır. Kontrol olarak $-1$ ve $2$ yerel minimum, $0$ yerel maksimum verir.

</details>

## Q3 · Tersin tanım ve değer kümeleri

$f(x)=(1-2\sqrt x)/(1+\sqrt x)$, $x\ge0$. **(a)** Tersin varlığını göster, **(b)** tanım ve görüntü kümelerini bul, **(c)** açık formülü çıkar.

<details><summary>Üç adımı aç</summary>

**(a)** $t=\sqrt x$ yaz. $f=-2+3/(1+t)$, $t\ge0$ için kesin azalır. Karekök kesin arttığı için $f$ bire birdir.

**(b)** $f(0)=1$ ve $x\to\infty$ iken $f(x)\to-2$ üstten. Süreklilikten görüntü $(-2,1]$ olur. Tersin tanım kümesi $(-2,1]$, görüntüsü $[0,\infty)$.

**(c)** $u=(1-2t)/(1+t)$ denkleminde $t(u+2)=1-u$. Böylece $f^{-1}(u)=((1-u)/(u+2))^2$. Bulduğumuz tanım kümesinde oran negatif olamaz, dolayısıyla kare alma fazladan kök getirmez. $f^{-1}(1)=0$ uç değeri doğrular.

</details>

## Q4 · Tersin türevini bir noktada bulma

**(a)** $f(x)=4x^3/(x^2+1)$ için $(f^{-1})'(2)$, **(b)** $f(x)=x^3+5x-1+2\cos x+2\sin x$ için $(f^{-1})'(1)$ ile tersin tanım ve görüntü kümelerini bul. İki durumda da bire birliği kanıtla.

<details><summary>Çözümü aç</summary>

**(a)** $f'=4x^2(x^2+3)/(x^2+1)^2$ yalnız $0$'da sıfırdır ve diğer noktalarda pozitiftir. İki yarı eksende kesin artar, sıfırın iki tarafında da $f$ işaretini $x$'ten alır. Bu yüzden tüm doğruda kesin artar. Sonsuzdaki davranışı $4x$ gibidir ve görüntüsü $\mathbb R$'dir. $f(1)=2$, $f'(1)=4$ olduğundan $(f^{-1})'(2)=1/4$.

**(b)** $f'=3x^2+5-2\sin x+2\cos x\ge3x^2+1>0$. Kübik terim uç limitleri belirler, dolayısıyla sürekli $f$ her gerçek değeri bir kez alır. Tersin hem tanım hem görüntü kümesi $\mathbb R$. $f(0)=1$ ve $f'(0)=7$ verir. Sonuç $(f^{-1})'(1)=1/7$. Her iki şıkta da payda, özgün fonksiyonun **ön görüntüdeki** türevidir.

</details>

## Q5 · Ters grafiğin teğeti

$(3,5)$ noktasında $f$'nin teğeti $y=2x-1$. Tersin $(5,3)$'teki teğetini yaz.

<details><summary>Çözümü aç</summary>

Verilen noktadan $f(3)=5$, doğrunun eğiminden $f'(3)=2$. Tersin eğimi $1/f'(3)=1/2$. Nokta-eğim denklemi $y-3=(x-5)/2$, yani $y=x/2+1/2$. Kontrol olarak özgün teğet denkleminde $x$ ve $y$ yer değiştirince aynı doğru çıkar.

</details>

## Q6 · İç içe üstel ve logaritmik fonksiyonlar

**(a)** $e^{\sin(x^3-3)}$, **(b)** $\ln(\tan x)/e^{\tan x}$ ve **(c)** $\ln(3^{x^2+1}\ln x)$ ifadelerinin türevlerini bul.

<details><summary>Çözümü aç</summary>

**(a)** Dıştan içe üstel, sinüs ve kübik fonksiyon sıralanır. Türev $3x^2\cos(x^3-3)e^{\sin(x^3-3)}$.

**(b)** $u=\tan x$ yazınca $f=e^{-u}\ln u$. $u$'ya göre türev $e^{-u}(1/u-\ln u)$, $x$'e göre türev ise $\sec^2 x\,e^{-\tan x}(1/\tan x-\ln(\tan x))$. Özgün ifade $\tan x>0$ ve tanjant tanımlıyken geçerlidir.

**(c)** Çarpımın pozitif olması $\ln x>0$, yani $x>1$ gerektirir. Bu aralıkta $f=(x^2+1)\ln3+\ln(\ln x)$. Sonuç $2x\ln3+1/(x\ln x)$.

</details>

## Q7 · Logaritmik türevin dışarıda bıraktığı kök

$f=(x^2+1)^3(2x-5)^3/(x^2+5)^2$ için $f'$ ve $f'(5/2)$ isteniyor. İşaret değiştiren çarpan için $\ln|f|$ kullan.

<details><summary>Çözümü aç</summary>

$x\ne5/2$ iken $\ln|f|=3\ln(x^2+1)+3\ln|2x-5|-2\ln(x^2+5)$. Bu yüzden

$$f'=f\left(\frac{6x}{x^2+1}+\frac6{2x-5}-\frac{4x}{x^2+5}\right).$$

$5/2$'de parantez tanımsızdır. Ancak $f=(2x-5)^3h(x)$ ve $h=(x^2+1)^3/(x^2+5)^2$ her yerde düzgündür. Gösterilen ifadede kutuplu terim bile $6(2x-5)^2h$ biçiminde sıfıra gider. $f'$ sürekli olduğu için $f'(5/2)=0$.

</details>

## Q8 · Hem taban hem üs değişirken

**(a)** $x^{\sec x}$, **(b)** $(x^2+1)^{\sqrt[3]x}$, **(c)** $x^{\sqrt x}$, **(d)** $(1/x)^{\ln x}$ için $y'$ bul. Başlangıç eşitliği $\ln y=v\ln u$.

<details><summary>Çözümleri ve sıfırdaki özel durumu aç</summary>

**(a)** $\ln y=\sec x\ln x$. Dolayısıyla $y'=x^{\sec x}(\sec x\tan x\ln x+\sec x/x)$, $x>0$ ve $\cos x\ne0$.

**(b)** $\ln y=\sqrt[3]x\ln(1+x^2)$. $x\ne0$ için

$$y'=(1+x^2)^{\sqrt[3]x}\left(\frac{\ln(1+x^2)}{3x^{2/3}}+\frac{2x\sqrt[3]x}{1+x^2}\right).$$

Sıfırda $y(0)=1$. $w=\sqrt[3]x\ln(1+x^2)$ için $w/x\to0$ çünkü $\ln(1+x^2)\sim x^2$. Bu yüzden $(e^w-1)/x=((e^w-1)/w)(w/x)\to0$ ve $y'(0)=0$.

**(c)** $\ln y=\sqrt x\ln x$ denkleminden $y'=x^{\sqrt x}(\ln x+2)/(2\sqrt x)$, $x>0$.

**(d)** $\ln y=-(\ln x)^2$, dolayısıyla $y'=-(2\ln x/x)(1/x)^{\ln x}$, $x>0$. $x=1$'de üssün türevi sıfır olduğundan teğet yataydır.

</details>
