# Final denemesi

Özgün karma çalışma seti · önerilen 100 dakika · 100 puan. Geometri sorularında dilimi göster, uygunsuz integrallerde limiti yaz.

1. **12 puan.** (a) f(x)=ln(1+x) fonksiyonunun x=0 merkezli doğrusallaştırmasını bul. (b) x→0 için [ln(1+x)−x]/x² limitini hesapla.
2. **12 puan.** limₙ→∞ Σᵢ₌₁ⁿ (2/n)√(1+2i/n) toplamını belirli integrale dönüştürerek hesapla.
3. **12 puan.** F(x)=∫ₓ^(sin x) e^(t²) dt için F′(x) ve F′(0) nedir?
4. **16 puan.** (a) ∫ x ln x dx, x>0. (b) ∫ (x+3)/(x²+x−2) dx.
5. **16 puan.** (a) ∫₀² 1/√(4−x²) dx yakınsar mı? Değerini bul. (b) ∫₋₁¹ 1/x dx için aynı incelemeyi yap.
6. **16 puan.** y=√x ile y=x arasında kalan sınırlı bölgenin alanını ve y=−1 etrafında döndürüldüğünde oluşan hacmi bul.
7. **16 puan.** (a) x=t², y=t³, 0≤t≤1 eğrisinin uzunluğunu bul. (b) r=2 sin θ hangi çemberdir? Eğriyi bir kez tarayan açı aralığını ver.

<details><summary>Çözümleri aç</summary>

1. f(0)=0, f′(0)=1 ⇒ L(x)=x. Limit 0/0 biçimindedir. Türev oranı [1/(1+x)−1]/(2x)=−1/[2(1+x)]→−1/2.
2. Δx=2/n, xᵢ=2i/n. ∫₀²√(1+x)dx=[(2/3)(1+x)^(3/2)]₀²=(2/3)(3√3−1).
3. Zincir kuralı ve FTC ile F′=e^(sin²x) cos x−e^(x²), F′(0)=0.
4. (a) u=ln x, dv=x dx seç. Sonuç (x²/2)ln x−x²/4+C. (b) Payda (x−1)(x+2). Katsayılar 4/3 ve −1/3. Sonuç (4/3)ln abs(x−1)−(1/3)ln abs(x+2)+C, her tanım aralığında.
5. (a) Üst sınırı b<2 ile değiştir. x=2 sin θ ile integral arcsin(b/2) olur. b→2⁻ iken π/2. (b) Sıfırda ayır. Soldaki limit −∞, sağdaki +∞; uygunsuz integral ıraksar.
6. Kesişimler 0,1. Alan ∫₀¹(√x−x)dx=1/6. Dış yarıçap 1+√x, iç yarıçap 1+x. Hacim π∫₀¹(2√x−x−x²)dx=π(4/3−1/2−1/3)=π/2.
7. (a) Hız √(4t²+9t⁴)=t√(4+9t²). u=4+9t² ile uzunluk (13√13−8)/27. (b) r²=2r sin θ ⇒ x²+(y−1)²=1. θ∈[0,π] bir tam tur verir.

</details>
