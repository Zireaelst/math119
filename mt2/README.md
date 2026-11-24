# MT2 çalışma rehberi

[210 sorunun konu ve çözüm dizini](cikmis-dizini.md) · [Teoremle ispat örnekleri](teoremle-ispat.pdf) · [Haftalık çözümler](../recitations/README.md)

Duyuru ve kapsam görselindeki 12 başlık. Çıkmış numaraları PDF içindeki Item numaralarıdır.

[210 çıkmış soru ve çözümleri](210-cikmis.pdf) · [Resmî kapsam görseli](kapsam.png)

[Çevrimdışı çalışma defteri](../defter.html) · [Süreli deneme ve çözümler](deneme.md)

## 2.8 Mean-Value Theorem

Sürekliliği [a,b] üzerinde, türevlenebilirliği (a,b) içinde kontrol et. Sekant eğimi bir noktadaki türeve eşittir. Rolle için uç değerlerin eşit olması da gerekir.

**Örnek.** x³+x=4 denkleminin tam bir gerçek çözümü olduğunu kanıtla.

**Çözüm.** g(x)=x³+x−4 için g(1)<0<g(2). Süreklilik bir kök verir. İki kök olsaydı Rolle aralarında g′=0 gerektirirdi. Oysa g′=3x²+1>0.

**Pekiştirme.** [H04](../recitations/hafta-04.pdf) Q3–7 · [Çıkmış banka](210-cikmis.pdf), **1, 3, 4**

## 2.9 Implicit Differentiation

y içeren her terimi x’e göre türetirken zincir kuralını uygula. F(x,y)=0 için Fᵧ≠0 olduğunda y′=−Fₓ/Fᵧ.

**Örnek.** x²+xy+y²=7 eğrisinde (1,2) noktasındaki teğeti bul.

**Çözüm.** 2x+y+(x+2y)y′=0. Nokta denklemi sağlar ve payda 5’tir. Eğim −4/5, teğet y−2=−4(x−1)/5.

**Pekiştirme.** [H05](../recitations/hafta-05.pdf) Q1 · [Çıkmış banka](210-cikmis.pdf), **2, 5, 8**

## 3.1 Inverse Functions

Önce bire birliği ve görüntü kümesini bul. Tersin b noktasındaki türevi için f(a)=b denklemini çöz ve 1/f′(a) al.

**Örnek.** f(x)=x³+2x için (f⁻¹)′(3) nedir?

**Çözüm.** f′=3x²+2>0 ve uç limitler ±∞ olduğundan f, ℝ üzerinde terslenir. f(1)=3 ve f′(1)=5, dolayısıyla sonuç 1/5.

**Pekiştirme.** [H05](../recitations/hafta-05.pdf) Q3–5 · [Çıkmış banka](210-cikmis.pdf), **57, 61, 64**

## 3.3 Natural Logarithm and Exponential

Değişken taban ve üst bir aradaysa pozitif tabanda logaritma al. ln y’yi türetince y′/y elde edilir.

**Örnek.** x>0 için y=x^(sin x) fonksiyonunun x=π/2 noktasındaki türevi nedir?

**Çözüm.** ln y=sin x·ln x, dolayısıyla y′=y(cos x·ln x+sin x/x). Noktada y=π/2, parantez 2/π, sonuç 1.

**Pekiştirme.** [H05](../recitations/hafta-05.pdf) Q6–8, [H06](../recitations/hafta-06.pdf) Q1–2 · [Çıkmış banka](210-cikmis.pdf), **51, 53, 54**

## 3.5 Inverse Trigonometric Functions

arcsin’in değer aralığı [−π/2,π/2], arccos’un [0,π], arctan’ın (−π/2,π/2). İç fonksiyonun türevini çarp.

**Örnek.** g(x)=arcsin(2x) için tanım kümesini ve g′(1/4) değerini bul.

**Çözüm.** −1≤2x≤1 verir: [−1/2,1/2]. İçeride g′=2/√(1−4x²), dolayısıyla g′(1/4)=4/√3. Uçlarda bu türev formülü tanımsızdır.

**Pekiştirme.** Çıkmışlardan başla · [Çıkmış banka](210-cikmis.pdf), **50, 52, 55**

## 4.1 Related Rates

Bağıntıyı zamanın fonksiyonlarıyla yaz, zamana göre türet, sonra anlık değerleri koy. İşaret ve birim cevabın parçasıdır.

**Örnek.** Yarıçapı 5 cm iken kürenin hacmi dakikada 12 cm³ azalıyor. r′ nedir?

**Çözüm.** V=4πr³/3 verir: −12=4π·25·r′. Yarıçapın değişim hızı −3/(25π) cm/dk.

**Pekiştirme.** [H06](../recitations/hafta-06.pdf) Q3–5 · [Çıkmış banka](210-cikmis.pdf), **79, 84, 89**

## 4.3 Indeterminate Forms

L’Hôpital için önce 0/0 veya ∞/∞ biçimini göster. Üstel belirsizlikte pozitif ifadeye logaritma uygula ve sonunda üstel fonksiyona dön.

**Örnek.** x→0⁺ iken x^x limitini bul.

**Çözüm.** ln(x^x)=ln x/(1/x). Pay ve payda büyüklükçe sonsuza gider. Türevlerin oranı −x→0, böylece x^x→e⁰=1.

**Pekiştirme.** [H06](../recitations/hafta-06.pdf) Q6, Q8 · [Çıkmış banka](210-cikmis.pdf), **81, 86, 94**

## 4.4 Extreme Values

Kapalı aralıkta sürekli fonksiyonun uçlarını, içerideki türevi sıfır olan ve türevsiz noktaları karşılaştır.

**Örnek.** f(x)=x^(2/3) için [−1,8] üzerinde mutlak ekstremumları bul.

**Çözüm.** x≠0 için f′=2/(3∛x). Adaylar −1,0,8 ve değerler 1,0,4. Minimum 0, maksimum 4. Türevsiz nokta minimumu verdi.

**Pekiştirme.** [H07](../recitations/hafta-07.pdf) Q1–2 · [Çıkmış banka](210-cikmis.pdf), **82, 88, 90**

## 4.5 Concavity and Inflections

f″ işaret tablosunu kur. Büküm noktasında grafiğin konkavlığı yön değiştirir.

**Örnek.** f=x⁴ ve g=x³ için x=0 noktasını karşılaştır.

**Çözüm.** f″=12x² iki tarafta pozitif olduğundan büküm yok. g″=6x negatiften pozitife geçer, (0,0) büküm noktasıdır.

**Pekiştirme.** [H07](../recitations/hafta-07.pdf) Q3–4 · [Çıkmış banka](210-cikmis.pdf), **107, 195**

## 4.6 Sketching the Graph

Tanım kümesi, kesişimler, asimptotlar, f′ ve f″ işaretlerini aynı eksen üzerinde birleştir.

**Örnek.** f=x²/(x−1) grafiğini çizmek için gerekli bilgileri çıkar.

**Çözüm.** f=x+1+1/(x−1). Düşey asimptot x=1, eğik asimptot y=x+1. f′=x(x−2)/(x−1)²; artış (−∞,0),(2,∞), azalış (0,1),(1,2). Yerel maksimum (0,0), minimum (2,4). f″=2/(x−1)³; sol dal aşağı, sağ dal yukarı konkav. x=1 grafikte yoktur.

**Pekiştirme.** [H07](../recitations/hafta-07.pdf) Q3–4 · [Çıkmış banka](210-cikmis.pdf), **83, 87, 93**

## 4.8 Extreme-Value Problems

Amaç fonksiyonunu ve kısıtı ayrı yaz. Tek değişkene indir, fiziksel aralıkta iç ve sınır adaylarını karşılaştır.

**Örnek.** Duvar boyunca üç kenarı 60 m tel ile çevrilen dikdörtgenin en büyük alanı nedir?

**Çözüm.** Duvara dik kenar x, paralel kenar 60−2x. A=60x−2x², 0≤x≤30. A′=60−4x=0 için x=15, diğer kenar 30. Uçlarda alan sıfır, maksimum 450 m².

**Pekiştirme.** [H08](../recitations/hafta-08.pdf) Q2–3 · [Çıkmış banka](210-cikmis.pdf), **85, 92, 99**

## 4.9 Linear Approximations

Yakındaki kolay merkez a için L(x)=f(a)+f′(a)(x−a). Konkavlık, teğetin eğrinin hangi tarafında kaldığını söyler.

**Örnek.** √4,1 için doğrusal tahmin yap ve hatanın yönünü bul.

**Çözüm.** a=4, f(4)=2, f′(4)=1/4. Tahmin 2+0,1/4=2,025. Karekök pozitif eksende aşağı konkavdır, teğet değeri gerçek değerden büyüktür.

**Pekiştirme.** [H08](../recitations/hafta-08.pdf) Q1 · [Çıkmış banka](210-cikmis.pdf), **80, 91, 96**
