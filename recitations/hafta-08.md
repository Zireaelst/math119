# Hafta 8 · Doğrusallaştırma, optimizasyon ve alan

**Kapsam.** Q1–Q3, MT2'deki 4.9 (doğrusal yaklaşım) ve 4.8 (ekstremum problemleri) başlıklarını çalıştırır. Q4–Q5, toplamlar ve integralin alan tanımıyla final konularına geçiştir. [Özgün soru kâğıdı](hafta-08.pdf)

## Q1 · Teğet doğruyla yaklaşık değer

**(a)** $e^{0.015}$ ve **(b)** $\sin(3)$ için doğrusal yaklaşım yap. Açılar radyandır. Yakındaki, fonksiyon ve türev değerleri bilinen bir $a$ seç.

<details><summary>Çözümü aç</summary>

Genel formül $L(x)=f(a)+f'(a)(x-a)$.

**(a)** $a=0$ noktasında $e^0=1$, türev de $1$. Dolayısıyla $e^{0.015}\approx1+0.015=1.015$. Üstel fonksiyon yukarı konkav olduğu için teğet gerçek değerin altında kalır.

**(b)** $3$, $\pi$'ye yakındır. $\sin\pi=0$, $\cos\pi=-1$. Böylece $\sin3\approx-(3-\pi)=\pi-3\approx0.14159$. $[3,\pi]$'de sinüs aşağı konkav olduğu için sonuç gerçek değerin biraz üstündedir.

</details>

## Q2 · Bir metre telden daire ve kare

Telin bir kısmı çembere, kalanı kareye bükülüyor. Toplam alanı **(a)** en büyük, **(b)** en küçük yapan kesimi bul. İki şeklin de pozitif boyutlu olması koşulunun uçları nasıl etkilediğini incele.

<details><summary>Çözümü ve uç nokta yorumunu aç</summary>

Çember için $x$ metre ayrılırsa $r=x/(2\pi)$, karenin kenarı $(1-x)/4$. Amaç fonksiyonu

$$A(x)=\frac{x^2}{4\pi}+\frac{(1-x)^2}{16},\qquad
A'(x)=\frac{x}{2\pi}-\frac{1-x}{8},\qquad
A''(x)=\frac1{2\pi}+\frac18>0.$$

**(a)** Kapalı aralıkta maksimum uçlardadır. $A(0)=1/16$, $A(1)=1/(4\pi)>1/16$. Sıfır uzunluklu parça kabul edilirse telin tamamını çembere ayırmak maksimum verir. İki parça da pozitif olmak zorundaysa $0<x<1$ ve maksimum alınmaz. Karenin payı sıfıra yaklaşırken alanın üst sınırı $1/(4\pi)$ m² olur.

**(b)** $A'=0$ denklemi $4x=\pi(1-x)$ verir. Çembere $\pi/(4+\pi)$ m, kareye $4/(4+\pi)$ m ayrılır. İkinci türev pozitif olduğundan bu tek kritik nokta mutlak minimumdur. Yerine koyunca $A_{\min}=1/[4(4+\pi)]$ m². İki uzunluğun toplamı bir metredir.

</details>

## Q3 · Noktadan eğriye en kısa uzaklık

$(8,1)$ noktasından $y=1+x^{3/2}$ eğrisine en kısa uzaklığı bul. Karekök işlemini azaltmak için uzaklığın karesini küçült.

<details><summary>Çözümü aç</summary>

Gerçel tanım kümesi $x\ge0$. Eğri noktası $(x,1+x^{3/2})$ olup uzaklığın karesi $S=(x-8)^2+x^3$. Türevi $S'=2(x-8)+3x^2=(3x+8)(x-2)$. İlk çarpan pozitif olduğundan $S$ önce azalır, $x=2$'den sonra artar. Uç değer $S(0)=64$, iç minimum $S(2)=36+8=44$, sonsuzda $S\to\infty$. En yakın nokta $(2,1+2\sqrt2)$, en kısa **uzaklık** $\sqrt{44}=2\sqrt{11}$.

</details>

## Q4 · Teleskopik ve geometrik toplam

Pozitif tamsayı $n$ için $\sum_{i=1}^n(1/[i(i+1)]+2^{-i})=n/(n+1)+(2^n-1)/2^n$ özdeşliğini kanıtla.

<details><summary>Çözümü aç</summary>

İlk terimi $1/[i(i+1)]=1/i-1/(i+1)$ biçiminde ayır. Yazılan ardışık terimler birbirini götürür. Başta $1$, sonda $-1/(n+1)$ kalır; toplam $n/(n+1)$.

İkinci toplamın ilk terimi ve ortak oranı $1/2$. Sonlu geometrik seri formülü ile $\sum_{i=1}^n2^{-i}=\frac12(1-2^{-n})/(1-1/2)=1-2^{-n}$. İki sonucu toplamak istenen eşitliği verir. $n=1$ için iki taraf da $1$ eder.

</details>

## Q5 · Alt ve üst toplamların ortak limiti

$[0,2]$ üzerinde $f(x)=2^x$ ile $x$ ekseni arasındaki alanı, $n$ eşit alt aralıktan oluşan $P_n$ için $L(f,P_n)$ ve $U(f,P_n)$ hesaplayarak bul.

<details><summary>Alt ve üst toplamların çözümünü aç</summary>

$\Delta x=2/n$, $x_i=2i/n$. Fonksiyon artan olduğundan her aralığın en küçük yüksekliği sol, en büyük yüksekliği sağ uçtadır. $r=2^{2/n}$ yazılırsa $r^n=4$ ve

$$L(f,P_n)=\frac2n\sum_{i=0}^{n-1}r^i=\frac6{n(r-1)},\qquad
U(f,P_n)=\frac2n\sum_{i=1}^{n}r^i=\frac{6r}{n(r-1)}.$$

Kontrol olarak $U-L=6/n$, yani dikdörtgenlerden gelen iki tahmin birbirine yaklaşır. $r=e^{(2\ln2)/n}$ ve $(e^t-1)/t\to1$ olduğundan $n(r-1)\to2\ln2$. Dolayısıyla iki toplam da $3/\ln2$ değerine gider. Arada kalan alan $3/\ln2$ birim karedir.

</details>
