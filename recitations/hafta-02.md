# Hafta 2 · Limit kuralları ve süreklilik

[Özgün soru föyü (PDF)](hafta-02.pdf)

## 1. Sekiz limit

<details><summary>Her limit için yöntem ve sonuç</summary>

**(a)** $x\to2$ iken $|(x^3-8)\sin(1/(x^3-8))|\le|x^3-8|\to0$. Sıkıştırma teoremi limiti $0$ verir.

**(b)** $x\to+\infty$ iken pay ve paydayı $x^3$ ile bölün. $\sqrt{x^6}=|x|^3=x^3$ olduğundan

$$
\frac{4x^3+4x^2+1}{\sqrt{3x^6+x^4-12}}
=\frac{4+4/x+1/x^3}{\sqrt{3+1/x^2-12/x^6}}\longrightarrow\frac4{\sqrt3}.
$$

**(c)** $x\to-\infty$ için $\sqrt{x^2+2x}-x=(-x)(\sqrt{1+2/x}+1)\to+\infty$. Dolayısıyla bu ifadenin tersinin limiti $0$'dır.

**(d)** Paydada bu kez $\sqrt{x^2+2x}+x$ var. Eşlenikle genişletince

$$
\frac1{\sqrt{x^2+2x}+x}
=\frac{\sqrt{x^2+2x}-x}{2x}
=\frac{-\sqrt{1+2/x}-1}{2}\longrightarrow-1.
$$

**(e)** $x\to+\infty$ iken $|\sin x/(3x)|\le1/(3x)\to0$.

**(f)** $x\to-\infty$ iken $(\pi x^2+5x+1)/(x^2+1)\to\pi$. Sinüsün sürekliliği ile $\sin(\pi-\pi/6)=1/2$.

**(g)** İki kökün farkını eşleniğiyle genişletin. $x\to+\infty$ için

$$
\sqrt{x^2+x}-\sqrt{x^2-x}
=\frac{2x}{\sqrt{x^2+x}+\sqrt{x^2-x}}
=\frac2{\sqrt{1+1/x}+\sqrt{1-1/x}}\longrightarrow1.
$$

**(h)** $x>0$ için $x^2(2+\sin^2 x)/(3x+1)\ge2x^2/(3x+1)$. Alt sınır $+\infty$'ye gittiğinden limit $+\infty$.

</details>

## 2. Bilinen limitlerden yeni limitler

<details><summary>Toplam, fark ve çarpım</summary>

**(a)** $x\to a$ için $f+g\to2$ ve $f-g\to5$. Özdeşlik $4fg=(f+g)^2-(f-g)^2$ verir. Böylece $\lim fg=(4-25)/4=-21/4$.

**(b)** $x\ne3$ için $f(x)=5+(x-3)[(f(x)-5)/(x-3)]$. Köşeli parantezin limiti $4$ olduğundan çarpım $0\cdot4=0$'a gider. $\lim_{x\to3}f(x)=5$ vardır.

</details>

## 3. Taban fonksiyonunda soldan limit

<details><summary>Önce işareti belirleyin</summary>

$x\to0^-$ için taban fonksiyonunun içi

$$
\frac{x^3-x}{x^4-1}=\frac{x(x^2-1)}{(x^2-1)(x^2+1)}=\frac{x}{x^2+1}
$$

olur. Bu ifade sıfıra negatif taraftan yaklaşır. $-1<x<0$ için değeri $(-1,0)$ aralığındadır. Bu aralıktaki her sayının tabanı $-1$ olduğundan istenen limit $-1$.

</details>

## 4. Parçalı fonksiyonda parametre seçimi

<details><summary>İki birleşme noktasında süreklilik</summary>

$x=0$ noktasında $f(0)=3$. Sol limit $\lim_{x\to0^-}\sin(ax)/x=a$ olduğundan $a=3$ gerekir. Sağda $|x^3\sin(\pi/x^3)|\le x^3$ olduğu için sağ limit de $3$.

$x=1$ noktasında sol parça $f(1)=3+\sin\pi=3$ verir. Sağ limit $a+b$ olduğundan $a+b=3$. **$a=3$, $b=0$**. Açık aralıklarda her parça sürekli olduğundan bu iki eşitlik yeterlidir.

</details>

## 5. Eşitsizlikten süreklilik

<details><summary>Sıkıştırma ve fonksiyon değeri</summary>

$|f(x)|\le x^2$ eşitsizliğinde $x=0$ seçilirse $f(0)=0$. Her $x$ için $-x^2\le f(x)\le x^2$. Her iki sınır da $x\to0$ iken sıfıra gittiği için $\lim_{x\to0}f(x)=0=f(0)$.

</details>

## 6. Doğru mu, yanlış mı?

<details><summary>Kanıtlar ve karşı örnekler</summary>

**(a) Yanlış.** $f(x)=2$ ($x\ge0$) ve $f(x)=-2$ ($x<0$) olsun. $f^2(x)=4$ sabittir. $f$'nin iki tek taraflı limiti farklı olduğu için $\lim_{x\to0}f(x)$ yoktur.

**(b) Doğru** (sonlu limitler için). $\lim f$ mevcutken $\lim(f+g)$ de mevcut olsaydı $g=(f+g)-f$ eşitliği $\lim g$'nin varlığını gerektirirdi. Bu, varsayımla çelişir.

**(c) Yanlış.** $f(x)=0$ ve $g(x)=\sin(1/x)$ ($x\ne0$) seçilsin. $g$'nin sıfırda limiti yoktur ama $fg=0$ sabittir.

**(d) Yazıldığı biçimiyle eksik.** $f(x)\le g(x)$ tek başına iki limitin varlığını sağlamaz. Örneğin $a=0$ için $f=g$ fonksiyonunu (a)'daki gibi seçin. İki limitin varlığı ayrıca varsayılırsa ifade doğrudur. $g-f\ge0$ ve $\lim(g-f)=\lim g-\lim f$ olduğundan bu fark negatif olamaz.

</details>

## 7. Bir parabolle kesişme

<details><summary>Ara Değer Teoremi</summary>

$h(x)=f(x)-x^2$, $[0,2]$ üzerinde süreklidir. $h(0)=f(0)>0$ ve $h(2)=f(2)-4<0$. Ara Değer Teoremi $h(c)=0$ sağlayan bir $c\in(0,2)$ verir. Bu nokta tam olarak $f(c)=c^2$ koşulunu sağlar.

</details>
