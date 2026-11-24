# Hafta 4 · Zincir kuralı, Rolle ve Ortalama Değer Teoremi

[Özgün soru föyü (PDF)](hafta-04.pdf)

## 1. Altı zincir kuralı uygulaması

<details><summary>İç fonksiyonlardan türeve</summary>

**(a)** $f(x)=(5-3/x)^{2026}$, $x\ne0$. İç fonksiyonun türevi $3/x^2$'dir. Böylece $f'=2026(5-3/x)^{2025}(3/x^2)$.

**(b)** $f(x)=\sqrt{(1+\sqrt x)^3}=(1+\sqrt x)^{3/2}$. $x>0$ için
$f'(x)=\frac32(1+\sqrt x)^{1/2}\frac1{2\sqrt x}=\frac{3\sqrt{1+\sqrt x}}{4\sqrt x}$. $x=0$'da sağ fark oranı $+\infty$'ye gider.

**(c)** $f(x)=\cos(5x)/x$ için bölüm kuralı
$f'(x)=[-5x\sin(5x)-\cos(5x)]/x^2$ verir ($x\ne0$).

**(d)** $v=\cos^2(x^2)$ seçilirse $f=\sin^3v$. Önce $v'=-4x\cos(x^2)\sin(x^2)$, ardından

$$
f'=-12x\sin^2v\cos v\,\cos(x^2)\sin(x^2).
$$

**(e)** $u=x/(x^2+1)$ için $u'=(1-x^2)/(x^2+1)^2$. $f=\tan^4u$ olduğundan $f'=4\tan^3u\sec^2u\,(1-x^2)/(x^2+1)^2$.

**(f)** $v=\sin(\tan(x^2))$ ve $u=\sqrt v$ için $f=\sec u$. $v>0$ ve $\tan(x^2)$ tanımlı iken

$$
f'(x)=\sec u\tan u\,\frac{x\cos(\tan(x^2))\sec^2(x^2)}u.
$$

Sıfırda bu formül $0/0$ verir. $v(x)/x^2\to1$ ve $(\sec u-1)/u^2\to1/2$ olduğundan $(f(x)-1)/x\to0$, yani $f'(0)=0$. Diğer $v=0$ noktalarında $v'\ne0$ olduğundan $v$ işaret değiştirir. Bunlar doğal tanım kümesinin sınırıdır. Tek taraflı türev istenirse $(\sec\sqrt v-1)/v\to1/2$ ile değeri $v'(x)/2$ olur.

</details>

## 2. Değer tablosuyla bileşke türevi

<details><summary>Hangi noktadaki türev kullanılıyor?</summary>

$u=x^2+3$, $v=f(u)+3$ seçilirse $g=f(v)^2$. Zincir kuralı
$g'=2f(v)f'(v)f'(u)\cdot2x$ verir. $x=2$ için $u=7$, $v=f(7)+3=4$. Bu yüzden
$g'(2)=2\cdot2\cdot3\cdot4\cdot4=192$.

</details>

## 3. $\cos x>1-x^2/2$ eşitsizliği

<details><summary>Kesin eşitsizliği türevle kanıtlayın</summary>

$H(x)=\cos x-1+x^2/2$ alın. $H(0)=H'(0)=0$, $H'(x)=x-\sin x$ ve $H''(x)=1-\cos x\ge0$. Her $x>0$ için $(0,\min\{x,\pi\})$ aralığında $H''>0$ olduğundan $H'$ burada kesin artar, sonra da azalamaz. Dolayısıyla her $x>0$ için $H'(x)>0$. Böylece $H(x)>H(0)=0$ elde edilir.

</details>

## 4. $\cos x=1-2x$ denkleminin tek çözümü

<details><summary>Tekdüzelikle teklik</summary>

$h(x)=\cos x-1+2x$ için $h(0)=0$ ve her gerçek $x$ için $h'(x)=2-\sin x\ge1$. Fonksiyon kesin artandır. Bu nedenle $0$ tek köktür.

</details>

## 5. Dördüncü dereceden denklemin kök sayısı

<details><summary>Varlık ve üst sınır için iki ayrı adım</summary>

$f(x)=x^4+x^2+x-10$ süreklidir. $f(-2)=8$, $f(0)=-10$, $f(2)=12$ olduğundan $(-2,0)$ ve $(0,2)$ aralıklarının her birinde bir kök vardır.

Öte yandan $f''(x)=12x^2+2>0$ olduğundan $f'$ kesin artar ve en çok bir kez sıfır olabilir. Üç farklı kök olsaydı Rolle teoremi, ardışık iki kök çiftinin arasına iki farklı $f'$ kökü yerleştirirdi. Bu çelişki kök sayısının **tam iki** olduğunu gösterir.

</details>

## 6. Verilen dört noktadan $f''(c)=0$ sonucu

<details><summary>Uç nokta varsayımı ve amaçlanan kanıt</summary>

Föy, türevlerin $(0,8)$ üzerinde var olduğunu söylüyor. Son adımda $8$'de soldan süreklilik gerekir. Yalnız yazılı varsayımlarla sonucun neden çıkmadığını şu örnek gösterir. $0\le x<8$ için

$$
f(x)=-2+\frac72(x-1)-\frac56(x-1)(x-3)
$$

alın ve $f(8)=20$ atayın. Bu fonksiyon $f(1)=-2$, $f(3)=5$, $f(4)=6$ koşullarını sağlar. Üç türevi de $(0,8)$ üzerinde vardır, ancak her yerde $f''=-5/3$.

**$f$ ayrıca $8$'de soldan sürekli ise** $[1,3]$, $[3,4]$, $[4,8]$ aralıklarındaki kiriş eğimleri sırasıyla $7/2$, $1$, $7/2$ olur. Ortalama Değer Teoremi ilk ve son aralıkta $1<u<3<4<v<8$ ve $f'(u)=f'(v)=7/2$ verir. $f'$ bu iç aralıkta türevlenebilir olduğundan Rolle teoremi bir $c\in(u,v)$ için $f''(c)=0$ verir.

</details>

## 7. Ortalama eğimden küçük türev mümkün mü?

<details><summary>Ortalama Değer Teoremi ile çelişki</summary>

$[-1,3]$ üzerinde türevlenebilirlik (uçlarda tek taraflı) sürekliliği de verir. Uç değerlerin belirlediği kirişin eğimi $(6-2)/(3-(-1))=1$. Ortalama Değer Teoremi bir $c\in(-1,3)$ için $f'(c)=1$ gerektirir. Her iç noktada $f'(x)<1$ şartı bunu dışlar. Böyle bir fonksiyon yoktur.

</details>
