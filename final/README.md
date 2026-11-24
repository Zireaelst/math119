# Final çalışma rehberi

2026–27 güz izlencesindeki integral ve geometri başlıkları. Final için ayrı bir kapsam duyurusu paylaşılmadığından bu sıra çalışma planıdır. Önceki konuları karma çıkmışlarla tekrar et.

[İzlence ve önerilen kitap soruları](../kaynaklar/izlence-2.pdf) · [Çözümlü sınav arşivi](../kaynaklar/cikmis-sinavlar.pdf)

[Çevrimdışı çalışma defteri](../defter.html) · [Süreli deneme ve çözümler](deneme.md)

## 5.1 Sums and Sigma Notation

Aralıktaki genişlik Δx=(b−a)/n, sağ uç xᵢ=a+iΔx. Σi=n(n+1)/2, Σi²=n(n+1)(2n+1)/6.

**Örnek.** Σᵢ₌₁ⁿ (2i−1) toplamını bul.

**Çözüm.** 2Σi−n=n(n+1)−n=n².

**Pekiştirme.** [H08](../recitations/hafta-08.pdf) Q4

## 5.2 Areas as Limits of Sums

Artan bir fonksiyon için sol uç alt toplamı, sağ uç üst toplamı verir. İki limit eşitse alanı sıkıştırırlar.

**Örnek.** f(x)=x², [0,1] için sağ uç toplamının limitini al.

**Çözüm.** Δx=1/n. Toplam Σi²/n³=(n+1)(2n+1)/(6n²)→1/3. Sol toplamla fark (1²−0²)/n→0.

**Pekiştirme.** [H08](../recitations/hafta-08.pdf) Q5

## 5.3 The Definite Integral

Belirli integral işaretli birikimi verir. Eksen altında kalan alan negatif katkı yapar.

**Örnek.** ∫₋₁² x dx değerini geometriyle hesapla.

**Çözüm.** Soldaki üçgenin katkısı −1/2, sağdaki +2. Toplam 3/2; aynı bölgenin geometrik alanı 5/2.

**Pekiştirme.** 10. baskı §5.3 / 5, 11

## 5.4 Properties of the Definite Integral

Aralık bölme, sınır çevirme, lineerlik ve simetriyi hesap yapmadan önce dene.

**Örnek.** ∫₋₂² (x³+3) dx nedir?

**Çözüm.** Tek fonksiyon x³’ün simetrik aralıkta integrali 0. Sabit terim 3·4=12 verir.

**Pekiştirme.** §5.4 / 7, 15

## 2.10 Antiderivatives

Belirsiz integral bir fonksiyon ailesi verir. Başlangıç koşulu sabiti seçer.

**Örnek.** f′(x)=2x+1, f(2)=7 ise f(0) nedir?

**Çözüm.** f=x²+x+C, 7=4+2+C olduğundan C=1 ve f(0)=1.

**Pekiştirme.** Konu defterinde Antiderivatives

## 5.5 Fundamental Theorem of Calculus

Üst sınır g(x) ise türev f(g(x))g′(x). Alt sınır da değişiyorsa onun katkısını çıkar.

**Örnek.** F(x)=∫ₓˣ² cos(t²) dt için F′(x) nedir?

**Çözüm.** Sabit bir noktada integrali iki parçaya böl. Üst sınır 2x cos(x⁴), alt sınır −cos(x²) verir.

**Pekiştirme.** 2025–26 Güz final Q5, arşiv s.230

## 5.6 Substitution

İç fonksiyonu u seç. Belirli integralde her iki sınırı da yeni değişkene dönüştür.

**Örnek.** ∫₀¹ 2x/(1+x²) dx nedir?

**Çözüm.** u=1+x², du=2x dx. Sınırlar 1 ve 2. ∫₁² du/u=ln 2.

**Pekiştirme.** §5.6 / 13, 25

## 5.7 Areas of Plane Regions

Kesişimleri bul ve dilim yönünü seç. Üst ve alt eğri yer değiştiriyorsa integrali böl.

**Örnek.** y=x ve y=x² arasındaki sınırlı alanı bul.

**Çözüm.** Kesişimler 0,1. Bu aralıkta x≥x². Alan ∫₀¹(x−x²)dx=1/6.

**Pekiştirme.** §5.7 / 5, 11

## 6.1 Integration by Parts

∫u dv=uv−∫v du. Türevi basitleşen çarpanı u seç ve sınır terimini koru.

**Örnek.** ∫₀¹ x eˣ dx nedir?

**Çözüm.** u=x, dv=eˣdx. [xeˣ]₀¹−[eˣ]₀¹=e−(e−1)=1.

**Pekiştirme.** §6.1 / 10, 17

## 6.2 Integrals of Rational Functions

Pay derecesi yüksekse önce böl. Tekrarlı doğrusal çarpanda her kuvveti, indirgenemez ikinci derecede doğrusal payı kullan.

**Örnek.** ∫ (3x+1)/(x²−1) dx nedir?

**Çözüm.** Kesir 2/(x−1)+1/(x+1) olur. Sonuç 2 ln abs(x−1)+ln abs(x+1)+C; çözüm ±1 ile ayrılan her aralıkta geçerlidir.

**Pekiştirme.** §6.2 / 9, 15

## 6.3 Inverse Substitutions

√(a²−x²) için x=a sin θ, √(a²+x²) için x=a tan θ seçilebilir. Karekökü açarken açı aralığını belirle.

**Örnek.** ∫₀¹ √(1−x²) dx değerini trigonometrik dönüşümle bul.

**Çözüm.** x=sin θ, 0≤θ≤π/2. İntegral ∫₀^(π/2) cos²θ dθ olur. cos²θ=(1+cos 2θ)/2 ile sonuç π/4.

**Pekiştirme.** §6.3 / 13, 23

## 6.5 Improper Integrals

Sonsuz sınırı veya tekil noktayı tek yanlı limit yap. İç tekillikte iki integral ayrı ayrı yakınsamalıdır.

**Örnek.** ∫₁^∞ x⁻² dx ile ∫₀¹ x⁻¹ dx yakınsar mı?

**Çözüm.** İlki lim(1−1/b)=1. İkincisi lim(−ln ε)=∞. p-integrali sonsuzda p>1, sıfırda p<1 iken yakınsar.

**Pekiştirme.** 2024–25 Bahar final Q3, s.234

## 7.1 Volumes by Slicing

Dönme eksenine dik kesitte V=π∫(R²−r²)dx. Yarıçaplar eksene olan uzaklıklardır.

**Örnek.** 0≤x≤1 aralığında x²≤y≤x bölgesi x ekseni çevresinde dönerse hacim nedir?

**Çözüm.** R=x, r=x². V=π∫₀¹(x²−x⁴)dx=2π/15.

**Pekiştirme.** 2024–25 Bahar final Q1, s.232

## 7.3 Arc Length and Surface Area

y=f(x) için ds=√(1+f′²)dx. Dönel yüzeyde dS=2π·(eksene uzaklık)·ds. Parametrik eğride ds=√(x′²+y′²)dt.

**Örnek.** y=x, 0≤x≤2 için yay uzunluğu ve x ekseni çevresindeki yan yüzey alanı nedir?

**Çözüm.** ds=√2 dx. Uzunluk 2√2, yüzey ∫₀² 2πx√2 dx=4π√2.

**Pekiştirme.** 2024–25 Bahar final Q5, s.235

## 8.5 Polar Coordinates and Polar Curves

x=r cos θ, y=r sin θ. Negatif r karşı ışını gösterir. Eğriyi çizerken simetriyi ve tekrar taranan açıları kontrol et.

**Örnek.** r=2 cos θ eğrisini Kartezyen biçime dönüştür ve bir kez tarayan aralık ver.

**Çözüm.** r²=2r cos θ ⇒ (x−1)²+y²=1. −π/2≤θ≤π/2 seçilirse r≥0 ve çember bir kez taranır.

**Pekiştirme.** §8.5 / 7, 13, 22
