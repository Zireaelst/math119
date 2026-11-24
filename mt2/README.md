# MT2 çalışma rehberi

**Ana çalışma aracı: [MT2 notebook](notebook.html).** Her konuda formül kartı, tuzaklar, çıkmışlardan çıkarılmış bütün soru tipleri, çözümlü gerçek sorular, 210 çıkmışın tamamına bağlantı ve üç süreli mock var. Repoyu indirip tarayıcıda aç.

Bu sayfa notebook’un GitHub’da okunabilen kısa özetidir. Kapsam, duyuru ve [kapsam görselindeki](kapsam.png) 12 başlıktır. Kalın numaralar [210 soruluk bankadaki](210-cikmis.pdf) Item numaralarıdır, sayfaları [dizinde](cikmis-dizini.md).

[Teoremle ispat örnekleri](teoremle-ispat.pdf) · [Haftalık çözümler](../recitations/README.md) · [Özgün deneme](deneme.md) · [Genel defter](../defter.html)

## 2.8 Mean-Value Theorem

$f$, $[a,b]$’de sürekli ve $(a,b)$’de türevlenebilir ise $f'(c)=\dfrac{f(b)-f(a)}{b-a}$ olan bir $c\in(a,b)$ vardır. Rolle için ayrıca $f(a)=f(b)$ gerekir. Hipotezleri her seferinde yaz.

**Örnek.** $x^3+x=4$ denkleminin tam bir gerçek çözümü olduğunu kanıtla.

**Çözüm.** $g(x)=x^3+x-4$ için $g(1)\lt 0\lt g(2)$. Süreklilik ve IVT bir kök verir. İki kök olsaydı Rolle aralarında $g'=0$ gerektirirdi, oysa $g'=3x^2+1\gt 0$.

**Soru tipleri:** teorem ve Doğru/Yanlış · eşitsizlik ispatı · türev sınırından değer sınırı · tam bir kök · verilen değerlerden $f'(c)=k$ ya da $f''(c)=0$ · türevi sıfır olan özdeşlik.
**Pekiştirme.** [H04](../recitations/hafta-04.md) Q3–7 · Çıkmış **12, 30, 43, 49, 37, 14**

## 2.9 Implicit Differentiation

$y$ içeren her terimi $x$’e göre türetirken zincir kuralını uygula. $F(x,y)=0$ ve $F_y\neq0$ için $y'=-F_x/F_y$.

**Örnek.** $x^2+xy+y^2=7$ eğrisinin $(1,2)$’deki teğeti.

**Çözüm.** $2x+y+(x+2y)y'=0$. Nokta denklemi sağlar ve $x+2y=5$. Eğim $-\frac45$, teğet $y-2=-\frac45(x-1)$.

**Soru tipleri:** teğet/normal · verilen $x$’te tüm noktalar ve yatay teğet · $y''$ · soyut $f$ içeren denklem · geometrik özellik ispatı · örtük doğrusallaştırma.
**Pekiştirme.** [H05](../recitations/hafta-05.md) Q1 · Çıkmış **11, 42, 18, 5, 15, 47**

## 3.1 Inverse Functions

Önce bire birliği ve görüntü kümesini göster. $(f^{-1})'(b)$ için $f(a)=b$ denklemini tahminle çöz ve $1/f'(a)$ al.

**Örnek.** $f(x)=x^3+2x$ için $(f^{-1})'(3)$.

**Çözüm.** $f'=3x^2+2\gt 0$ ve uç limitler $\pm\infty$, $f$ $\mathbb R$’de terslenir. $f(1)=3$ ve $f'(1)=5$, sonuç $\frac15$.

**Pekiştirme.** [H05](../recitations/hafta-05.md) Q3–5 · Çıkmış **76, 64, 57, 27(b)**

## 3.3 Natural Logarithm and Exponential

Taban ve üs birlikte değişiyorsa logaritma al: $\ln y=g\ln f$, dolayısıyla $y'=y\big(g'\ln f+g\,f'/f\big)$.

**Örnek.** $x\gt 0$ için $y=x^{\sin x}$’in $x=\pi/2$’deki türevi.

**Çözüm.** $\ln y=\sin x\ln x$, $y'=y\big(\cos x\ln x+\frac{\sin x}{x}\big)$. Noktada $y=\frac\pi2$ ve parantez $\frac2\pi$, sonuç $1$.

**Pekiştirme.** [H05](../recitations/hafta-05.md) Q6–8, [H06](../recitations/hafta-06.md) Q1–2 · Çıkmış **56, 54, 53, 60**

## 3.5 Inverse Trigonometric Functions

$\arcsin$ değer aralığı $[-\frac\pi2,\frac\pi2]$, $\arccos$ $[0,\pi]$, $\arctan$ $(-\frac\pi2,\frac\pi2)$. $(\arcsin u)'=\frac{u'}{\sqrt{1-u^2}}$, $(\arctan u)'=\frac{u'}{1+u^2}$.

**Örnek.** $g(x)=\arcsin(2x)$ için tanım kümesi ve $g'(1/4)$.

**Çözüm.** $-1\le2x\le1$ verir $[-\frac12,\frac12]$. İçeride $g'=\frac{2}{\sqrt{1-4x^2}}$, dolayısıyla $g'(\frac14)=\frac4{\sqrt3}$. Uçlarda türev yoktur.

**Pekiştirme.** [2024 föy 7](../recitations/2024-guz/hafta-07.pdf) · Çıkmış **50, 52, 55, 58**

## 4.1 Related Rates

Bağıntıyı zamanın fonksiyonlarıyla yaz, türet, sonra anlık değerleri koy. İşaret ve birim cevabın parçası.

**Örnek.** Yarıçapı 5 cm iken kürenin hacmi dakikada 12 cm³ azalıyor. $r'$?

**Çözüm.** $V=\frac43\pi r^3$, dolayısıyla $-12=4\pi\cdot25\,r'$ ve $r'=-\frac{3}{25\pi}$ cm/dk.

**Pekiştirme.** [H06](../recitations/hafta-06.md) Q3–5 · Çıkmış **84, 112, 134, 183, 79**

## 4.3 Indeterminate Forms

L’Hôpital’den önce $\frac00$ ya da $\frac\infty\infty$ biçimini göster. $1^\infty$, $0^0$, $\infty^0$ için $\ln L$ hesapla ve sonunda $e$’ye dön.

**Örnek.** $\lim_{x\to0^+}x^x$.

**Çözüm.** $\ln(x^x)=\frac{\ln x}{1/x}$, $\frac\infty\infty$. Türev oranı $-x\to0$, dolayısıyla $x^x\to e^0=1$.

**Pekiştirme.** [H06](../recitations/hafta-06.md) Q6, Q8 · Çıkmış **81, 86, 97, 74, 125, 135**

## 4.4 Extreme Values

Kapalı aralıkta sürekli fonksiyonun uçlarını, kritik ($f'=0$) ve tekil ($f'$ yok) noktalarını karşılaştır.

**Örnek.** $f(x)=x^{2/3}$ için $[-1,8]$’de mutlak ekstremumlar.

**Çözüm.** $f'=\frac{2}{3\sqrt[3]x}$, adaylar $-1,0,8$, değerler $1,0,4$. Min $0$ (tekil nokta), maks $4$.

**Pekiştirme.** [H07](../recitations/hafta-07.md) Q1–2 · Çıkmış **88, 181, 159, 170, 95**

## 4.5 Concavity and Inflections

$f''$ işaret tablosunu kur. Büküm noktasında $f$ süreklidir, teğet vardır ve konkavlık yön değiştirir.

**Örnek.** $f=x^4$ ve $g=x^3$ için $x=0$.

**Çözüm.** $f''=12x^2$ iki tarafta pozitif, büküm yok. $g''=6x$ işaret değiştirir, $(0,0)$ büküm.

**Pekiştirme.** [H07](../recitations/hafta-07.md) Q3–4 · Çıkmış **107, 169, 195**

## 4.6 Sketching the Graph

Tanım kümesi, kesişimler, asimptotlar, $f'$ ve $f''$ işaretlerini tek tabloda birleştir.

**Örnek.** $f=\frac{x^2}{x-1}$.

**Çözüm.** $f=x+1+\frac1{x-1}$: düşey $x=1$, eğik $y=x+1$. $f'=\frac{x(x-2)}{(x-1)^2}$: artan $(-\infty,0]$, $[2,\infty)$, azalan $[0,1)$, $(1,2]$. Yerel maks $(0,0)$, min $(2,4)$. $f''=\frac{2}{(x-1)^3}$: solda aşağı, sağda yukarı konkav.

**Pekiştirme.** [H07](../recitations/hafta-07.md) Q3–4 · Çıkmış **93, 98, 87, 82, 210**

## 4.8 Extreme-Value Problems

Amaç fonksiyonunu ve kısıtı ayrı yaz. Tek değişkene indir, fiziksel aralıkta iç ve sınır adaylarını karşılaştır.

**Örnek.** Duvar boyunca üç kenarı 60 m tel ile çevrilen dikdörtgenin en büyük alanı.

**Çözüm.** Dik kenar $x$, paralel kenar $60-2x$. $A=60x-2x^2$, $0\le x\le30$. $A'=0$ için $x=15$. Maks $450$ m².

**Pekiştirme.** [H08](../recitations/hafta-08.md) Q2–3 · Çıkmış **92, 99, 85, 194, 202**

## 4.9 Linear Approximations

$L(x)=f(a)+f'(a)(x-a)$. Konkavlık teğetin eğrinin hangi tarafında kaldığını söyler.

**Örnek.** $\sqrt{4.1}$.

**Çözüm.** $a=4$, $f(4)=2$, $f'(4)=\frac14$. Tahmin $2.025$. $\sqrt x$ aşağı konkav, tahmin gerçek değerden büyük.

**Pekiştirme.** [H08](../recitations/hafta-08.md) Q1 · Çıkmış **132, 91, 201, 80**
