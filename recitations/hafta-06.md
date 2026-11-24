# Hafta 6 · Değişim hızları ve belirsiz biçimler

**Kapsam.** Q1–Q8, MT2'nin logaritmik türev, bağlı değişim hızları ve belirsiz biçimler başlıklarıyla ilişkilidir. Q7–Q8'de limit ve türev tanımları da kullanılır. [Özgün soru kâğıdı](hafta-06.pdf)

## Q1 · Logaritmik türev ve başlangıç eğimi

$f=(x^2+1)^3(2x+5)^3/(x^2+5)^2$ için $f'$ ve $f'(0)$ bul. Bu haftaki çarpan $2x+5$.

<details><summary>Çözümü aç</summary>

$x\ne-5/2$ için $\ln|f|=3\ln(x^2+1)+3\ln|2x+5|-2\ln(x^2+5)$. Türev alıp $f$ ile çarpınca

$$f'=f\left(\frac{6x}{x^2+1}+\frac6{2x+5}-\frac{4x}{x^2+5}\right).$$

$f(0)=125/25=5$, dolayısıyla $f'(0)=5(6/5)=6$. Eksik noktada $f$ düzgün bir çarpan ile $(2x+5)^3$ çarpımı olduğundan $f'(-5/2)=0$.

</details>

## Q2 · Değişken üs

**(a)** $x^{\sec x}$, **(b)** $(x^2+1)^{\sqrt[3]x}$, **(c)** $x^{\sqrt x}$, **(d)** $(1/x)^{\ln x}$ ifadelerini türet.

<details><summary>Dört çözümü aç</summary>

Genel olarak $y=u^v$ ve $u>0$ ise $\ln y=v\ln u$ ve $y'=y(v'\ln u+vu'/u)$.

**(a)** $u=x,v=\sec x$ ile $y'=x^{\sec x}(\sec x\tan x\ln x+\sec x/x)$, $x>0$, $\cos x\ne0$.

**(b)** $u=1+x^2,v=\sqrt[3]x$ verir. $x\ne0$ iken $y'=y\big(\ln(1+x^2)/(3x^{2/3})+2x\sqrt[3]x/(1+x^2)\big)$. $x=0$'da $y=1$. $w=\sqrt[3]x\ln(1+x^2)$ alındığında $w/x\to0$ ve $(e^w-1)/w\to1$ olduğundan $y'(0)=0$.

**(c)** $\ln y=\sqrt x\ln x$ için $(\ln y)'=\ln x/(2\sqrt x)+1/\sqrt x$. Dolayısıyla $y'=x^{\sqrt x}(\ln x+2)/(2\sqrt x)$, $x>0$.

**(d)** $\ln y=(\ln x)\ln(1/x)=-(\ln x)^2$. Böylece $y'=-(1/x)^{\ln x}\,2\ln x/x$, $x>0$.

</details>

## Q3 · Eriyen küre

Başlangıç yarıçapı 7 cm olan buz küresinin hacmi dakikada 12 cm³ azalıyor. Yarıçap 5 cm iken yarıçapın değişim hızı nedir?

<details><summary>Çözümü aç</summary>

$V=4\pi r^3/3$ ve $dV/dt=-12$. Zamana göre türev $dV/dt=4\pi r^2\,dr/dt$. İstenen anda $dr/dt=-12/(4\pi\,25)=-3/(25\pi)$ cm/dk. Eksi işaret yarıçapın küçüldüğünü gösterir. Başlangıç yarıçapı anlık hızın hesabına girmez.

</details>

## Q4 · Büyüyen dikdörtgenin daralması

Alan saniyede 5 m², yükseklik saniyede 10 m artıyor. Yükseklik 20 m, genişlik 16 m iken genişliğin değişim hızını bul.

<details><summary>Çözümü aç</summary>

$A=hw$ olduğundan $\dot A=h\dot w+w\dot h$. Sayıları türevden sonra yerleştirince $5=20\dot w+16(10)$ ve $\dot w=-155/20=-31/4$ m/s. Kontrol olarak genişlik sabit kalsaydı alan artış hızı $160$ m²/s olacaktı. Verilen $5$ m²/s için genişliğin azalması gerekir.

</details>

## Q5 · Parabol üzerindeki parçacığın orijine uzaklığı

Birinci bölgede $y=x^2$, $\dot x=17$ birim/s. $x=4$ iken uzaklık ne hızla değişir?

<details><summary>Çözümü aç</summary>

$D^2=x^2+y^2$ ve $\dot y=2x\dot x$. Zamana göre türev $D\dot D=x\dot x+y\dot y$. İstenen anda $y=16$, $D=4\sqrt{17}$ ve $\dot y=136$. Böylece $\dot D=(4\cdot17+16\cdot136)/(4\sqrt{17})=33\sqrt{17}$ birim/s. Hızın pozitif olması hareket yönüyle uyumlu.

</details>

## Q6 · Dört limit

**(a)** $\lim_{x\to2^+}\ln(x-2)/\ln(x^2-4)$, **(b)** $\lim_{x\to(\pi/2)^-}\tan x/\ln(\pi/2-x)$, **(c)** $\lim_{x\to0}(\sin x/x)^{1/x^2}$, **(d)** $\lim_{x\to0^+}\sqrt{x}/\sqrt{\sin x}$.

<details><summary>Limitlerin çözümünü aç</summary>

**(a)** $\ln(x^2-4)=\ln(x-2)+\ln(x+2)$. İlk terim $-\infty$'ye giderken ikincisi sonlu kalır. Oranı $\ln(x-2)$ ile sadeleştirince sonuç $1$.

**(b)** $t=\pi/2-x\to0^+$ ile oran $\cot t/\ln t$ olur. $\cot t\sim1/t$ ve $t\ln t\to0^-$ (örneğin $\ln t/(1/t)$ oranına L’Hôpital uygulanır). Dolayısıyla limit $-\infty$; sonlu bir limit yoktur.

**(c)** Taban sıfır yakınında pozitiftir. Logaritma alınca üs $\ln(\sin x/x)/x^2$ olur. $0/0$ biçimine L’Hôpital uygulayarak

$$\lim_{x\to0}\frac{x\cos x-\sin x}{2x^2\sin x}
=\lim_{x\to0}\frac{-x\sin x}{4x\sin x+2x^2\cos x}
=\lim_{x\to0}\frac{-(\sin x/x)}{4(\sin x/x)+2\cos x}=-\frac16.$$

İlk oran logaritmalı ifadenin türev oranıdır, ikinci oran bir kez daha türevle elde edilir. Üstel fonksiyona geri dönünce sonuç $e^{-1/6}$.

**(d)** Sağ tarafta her iki kök tanımlıdır. $\sqrt{x/\sin x}=1/\sqrt{\sin x/x}\to1$. 

</details>

## Q7 · Parçalı fonksiyonun birleşme noktası

$x>0$ için $f(x)=e^{-1/x}$, $x\le0$ için $f(x)=0$. Tüm gerçek sayılarda türevlenebilirliği göster.

<details><summary>Çözümü aç</summary>

Açık yarı eksenlerde türev sırasıyla $e^{-1/x}/x^2$ ve $0$. Birleşme noktasında $f(0)=0$ olduğundan soldan fark oranı sıfırdır. Sağdan $h\downarrow0$ için oran $e^{-1/h}/h$. $u=1/h\to+\infty$ ile $u/e^u\to0$ (L’Hôpital). İki tek yanlı türev çakışır ve $f'(0)=0$ bulunur.

</details>

## Q8 · Salınımlı limitte sıkıştırma

$\lim_{x\to0}x^2\sin^2(1/x)/\sin x$ değerini sıkıştırmayla göster. L’Hôpital ile doğrudan sonuca neden ulaşılamaz?

<details><summary>Sıkıştırmayı ve türev oranı kontrolünü aç</summary>

$\sin x/x\to1$ ve $\sin^2(1/x)\le1$ olduğundan

$$0\le\left|\frac{x^2\sin^2(1/x)}{\sin x}\right|\le |x|\left|\frac{x}{\sin x}\right|\longrightarrow0.$$

Özgün oran $0/0$ olsa da türev oranı $[2x\sin^2(1/x)-\sin(2/x)]/\cos x$ limit taşımaz. Örneğin $2/x=\pi/2+2\pi n$ ile $2/x=3\pi/2+2\pi n$ seçilirse türev oranı sırasıyla $-1$ ve $1$'e yaklaşır. Bu nedenle L’Hôpital teoreminin türev oranının limitiyle ilgili koşulu sağlanmaz.

</details>
