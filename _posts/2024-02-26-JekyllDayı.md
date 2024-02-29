---
layout: post
title:  "Jekyll dayı ve GitHub'la dövüşler"
date:   2024-02-26
categories: Hikayeler
---
Bu akşamki mesaimizde madem bir şeyler karalamaya karar verdik, bari doğru düzgün olsun diye, Jekyll tabanlı bir blog kurmaya kalktım.

Jekyll, metin dosyalarını işleyerek statik web sayfaları yaratan bir framework. Kurması, anlaması çok vakit almadı. Güzel tutorialları da var.

Bir de GitHub Pages ile sorunsuz çalışması gerekiyor. Onu bu yazıyı yayınlamaya kalktığımda göreceğim.

Asıl vaktimi yiyip biteren github'a basit bir __iteleme__ işlemi yapmak oldu. Epey bir süre kişisel tokenimi kabul ettiremedim github'a. Sonunda anladım ki ana bilgisayarımdan, sanal makineye (Jekyll'ı ana makineme kurmaktansa bir linux VM açıverdim) şifrenin içindeki _ karakteri - buna dönüşüvermiş. Anlayabilen beri gelsin.

Bu sepeble de bugün oyuna birşeyler eklemek, bakmak, dokanmak nasip olmadı. Bakalım eğer blog daha fazla sorun çıkarmazsa birşeyler karalarız belki...

### Yatmadan once karalamalar

Tam beklediğim gibi ilk güncellemeden sonra güncellemeler çalışmamaya başladı bile. Bu ufak notu düşüyorum ki bakalım şimdi çalışacak mı.

### Bugün neler yaptık
1. Vukuat resimlerini güzel gösterebilmek için bir kaç ayar yaptık. Bunların en önemlisi resimleri Clamped Sampler'a almaktı. Anladığım kadarıyla bu resmin altının üstüne akmasını engelliyor. Eğer bu yapılmazsa resimlerin tepesinde salak bir çizgi oluşuyor.

2. Vukuat lara girerkenki bakış olayını biraz daha toparladım. Dışardan bir fonksiyonla nasıl çağıralabileceğini gördük. BP'de fonksiyonlar hemen dönüş yaptığından dolayı, fonksiyonun içerisnden dışarıdaki bir event çağırmamız gerekiyor.

Kendime not, buralara artık yavaştan ekran görüntüleri koymak lazım.