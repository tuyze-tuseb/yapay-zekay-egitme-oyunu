# Yapay Zekâyı Eğit — TÜSEB

Çocuklara yapay zekânın örneklerden öğrendiğini anlatan, dokunmatik ekranlar için tasarlanmış eğitici bir oyun.

Canlı sürüm: https://tuyze-tuseb.github.io/yapay-zekay-egitme-oyunu/

## Nasıl oynanır

Oyun açılışta yaş sorar ve iki moddan birini başlatır.

### 10 yaşından küçükler — sınavsız mod

Sağlık durumu kartları yukarıdan sakin bir tempoda düşer. Çocuk kartı parmağıyla yakalar ve hasta ise sola, sağlıklı ise sağa fırlatır. Yapay zekâ her karttan öğrenir. 15 kart öğretilince kutlama ekranı açılır: konfeti, kazanılan unvan ve öğretme istatistikleri. Sınav yoktur.

Bu modda kelime oyunu içeren "çok zor" kartlar devre dışıdır ve kartlar daha yavaş düşer.

### 10 yaşından büyükler — sınavlı mod

Aynı eğitim bölümü, 20 kartla ve giderek hızlanan bir tempoyla oynanır. Ardından sınav başlar: hiç görülmemiş 10 kart gelir, önce oyuncu tahmin eder, sonra yapay zekâ cevabını açıklar. Her sorunun ardından doğru cevap ve nedeni gösterilir. Sonuç ekranında iki skor karşılaştırılır.

## Kartlar

Kartlar dört zorluk kademesine ayrılmıştır: kolay, orta, zor ve çok zor. Çok zor kartlar, hastalık gibi görünen normal vücut tepkilerini içeren kelime oyunlarıdır (acı yemekten ağzın yanması, koşudan sonra kalbin hızlanması gibi). Bazı kartlar Diyarbakır ve Şanlıurfa'ya özgü yerel örnekler içerir.

Yapay zekânın sınavdaki isabet oranı, eğitim sırasında kaç kartın doğru öğretildiğine bağlıdır. Yanlış öğretilen kartlar isabeti düşürür; böylece "yanlış veri, yanlış sonuç" ilkesi oyunun içinde deneyimlenir.

## Teknik

- Tek dosyalık statik HTML (`index.html`) — kurulum, derleme veya sunucu gerektirmez
- Bağımlılık yok: ikonlar satır içi SVG, logo base64 olarak gömülü
- Tek harici kaynak: Google Fonts (Plus Jakarta Sans)
- Ses efektleri Web Audio API, robotun sesli anlatımı Web Speech API ile
- 32 inç dokunmatik ekran için tasarlandı, mobil ve masaüstünde de çalışır

## Çalıştırma ve yayınlama

Dosyayı bir tarayıcıda açmak yeterlidir. Yayın için `index.html` herhangi bir statik barındırma servisine yüklenebilir. Bu depo GitHub Pages üzerinden `main` dalından yayınlanmaktadır; her push sonrası site otomatik güncellenir.

Başlangıç ekranının altındaki sürüm etiketi (örneğin `v1.9`), yayındaki sürümün doğrulanması içindir.
