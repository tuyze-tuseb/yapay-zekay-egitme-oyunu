# Yapay Zekâyı Eğit — TÜSEB

Çocuklara yapay zekânın örneklerden öğrendiğini anlatan, dokunmatik ekranlar için tasarlanmış eğitici bir oyun.

## Nasıl çalışır

**1. Bölüm — Öğretme:** Sağlık durumu kartları yukarıdan düşer. Çocuk kartı yakalayıp hasta ise sola, sağlıklı ise sağa fırlatır. 20 kart öğretilince eğitim tamamlanır.

**2. Bölüm — Sınav:** Hiç görülmemiş kartlar gelir. Önce çocuk tahmin eder, sonra yapay zekâ cevabını açıklar. İkisinin skoru karşılaştırılır.

Kartlar dört zorluk kademesine ayrılmıştır (kolay, orta, zor, çok zor). Çok zor kartlar, hastalık gibi görünen normal vücut tepkilerini içeren kelime oyunlarıdır.

## Teknik

- Tek dosyalık statik HTML (`index.html`) — kurulum, derleme veya sunucu gerektirmez
- Bağımlılık yok: ikonlar satır içi SVG, logo base64 olarak gömülü
- Tek harici kaynak: Google Fonts (Plus Jakarta Sans)
- Ses efektleri Web Audio API, sesli anlatım Web Speech API ile
- 32 inç dokunmatik ekran için ölçeklenebilir arayüz

## Çalıştırma

Dosyayı bir tarayıcıda açmak yeterlidir. Yayın için herhangi bir statik barındırma servisi kullanılabilir.
