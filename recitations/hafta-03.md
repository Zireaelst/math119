# Hafta 3 · Süreklilik, teğet ve türev

[Özgün soru föyü (PDF)](hafta-03.pdf)

## 1. Çıktıdaki hatadan girdideki uzaklığa

<details><summary>Kesin uzaklık sınırı</summary>

$3x-1$ ile $5$ arasındaki uzaklık $|(3x-1)-5|=3|x-2|$ olur. Bunun $1/100$'den küçük olması için ve ancak $|x-2|<1/300$ gerekir. Uç noktalar hatanın tam $1/100$ olduğu noktalardır.

</details>

## 2. Trigonometrik denklemin en az iki kökü

<details><summary>İki ayrı işaret değişimi</summary>

$h(x)=2\sin x+6\cos^2x-x$ süreklidir. $h(-\pi)=6+\pi>0$, $h(-\pi/2)=-2+\pi/2<0$, $h(0)=6>0$. Ara Değer Teoremi $(-\pi,-\pi/2)$ ve $(-\pi/2,0)$ aralıklarının her birinde bir kök verir. Aralıklar ayrık olduğundan kökler farklıdır.

</details>

## 3. İki birleşme noktasını aynı anda düzeltmek

<details><summary>Parametre denklemleri</summary>

$x<-3$ için $(x^2-9)/(x+3)=x-3$, dolayısıyla $-3$'te sol limit $-6$. Orta parçanın değeri $9a+3b+1$. Eşitleyince $3a+b=-7/3$.

$x=3$ noktasında orta parçanın limiti $9a-3b+1$, sağ parçanın değeri $6a-4b$. Eşitlik bu kez $3a+b=-1$ gerektirir. Aynı toplam iki farklı sayı olamayacağından fonksiyonu her yerde sürekli yapan bir $(a,b)$ yoktur.

</details>

## 4. Türev fonksiyonu ve teğet doğruları

<details><summary>Üç teğet probleminin çözümü</summary>

**(i)** $f(0)=0$, $x\ne0$ için $f(x)=x^3\sin(1/x)/\sin x$. $-1<x<1$, $x\ne0$ için bölüm kuralından

$$
f'(x)=\frac{[3x^2\sin(1/x)-x\cos(1/x)]\sin x-x^3\sin(1/x)\cos x}{\sin^2x}.
$$

Payın türevindeki ikinci terim $x^3\cos(1/x)(-1/x^2)$ çarpımından gelir. Sıfırda türev tanımına dönün:

$$
\frac{f(h)-f(0)}h
=\frac{h}{\sin h}\,h\sin(1/h)\longrightarrow1\cdot0=0.
$$

Dolayısıyla $f'(0)=0$ ve teğet $y=0$. Tanım aralığının uçları $\pm1$ için içe doğru tek taraflı türevler yukarıdaki formülün uç değerleridir.

**(ii)** $f(x)=x^2/(x-1)$ için $f'(x)=[2x(x-1)-x^2]/(x-1)^2=x(x-2)/(x-1)^2$. $f'(2)=0$, $f(2)=4$, dolayısıyla teğet $y=4$.

**(iii)** $f(x)=|x^3|$, $f(0)=0$. Fark oranı $|h|^3/h$'nin mutlak değeri $h^2$ olduğu için limit $0$. Orijindeki teğet $y=0$.

</details>

## 5. Çarpım ve zincir kuralları

<details><summary>Türevleri çarpanlar hâlinde yazın</summary>

**(a)** $u=x^2+3x$ ve $v=3\sec^2x-5$ ile $f=5\cos^3(u)v$. $u'=2x+3$ ve $v'=6\sec^2x\tan x$ kullanılır:

$$
f'(x)=5\left[-3\cos^2u\sin u\,(2x+3)v+6\cos^3u\,\sec^2x\tan x\right].
$$

**(b)** Özgün tanım kümesinde $\sin x\ne0$, $\cos x\ne0$ ve $1/\cot^3x=\tan^3x$. $A=\tan^2x-1$, $B=\sin^4(x^3)+x^5-4$ seçilirse $f=AB\tan^3x$. İç türevler

$$
A'=2\tan x\sec^2x,\qquad B'=12x^2\sin^3(x^3)\cos(x^3)+5x^4.
$$

Üç çarpanın her birini sırayla türetince $f'=(A'B+AB')\tan^3x+3AB\tan^2x\sec^2x$ çıkar.

</details>

## 6. Fonksiyonel denklemden türev

<details><summary>Artımı fark oranına dönüştürün</summary>

$f(x+y)=f(x)+f(y)+xy^2+x^2y$ denkleminde $y=0$ alınca $f(0)=0$. Şimdi $y=h\ne0$ yazın:

$$
\frac{f(x+h)-f(x)}h=\frac{f(h)}h+xh+x^2.
$$

Verilen $\lim_{h\to0}f(h)/h=3$ eşitliğiyle her $x$ için $f'(x)=3+x^2$. Özellikle **$f'(2)=7$**.

</details>
