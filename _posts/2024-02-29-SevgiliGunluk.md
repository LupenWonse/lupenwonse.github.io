---
title: Sevgili günlük
author: Lupen Wonse
---
Bugün ancak kısa birşeyler yapabilirim gibi görünüyor.

Plan'a eklenecek bazı şeyler var.
- Ses ve konuşmalar için test mahiyetinde birşeyler
- Level'a giriş çıkışı anlamak için, ana menü ve ordan demoya atlayış.

Bunları plana eklerken gördüm ki geçen seferden kalma ve önemli bir iş öylece duruyor. Event'lere kitlenmeyi yapmıştık ama şu anda burdan çıkmanın bir yolu yok. Önce bunu halletmek gerekiyor sanırım.

Hala genel olarak bütün hikaye nasıl yönetilecek bilemiyorum, ama şimdilik en azından oyuncunun nasıl davranması gerektiğini kestirebiliriz. Hem de ilerde test yaparken takılıp kalmayız.

Bu arada hala nasıl postlara resim ekleniyor denemedim... Bi deneyeyim

![imageTitle]({% link /assets/images/BP_Pusula_Screenshot_01.png %})

Biraz fazla vakit aldi ama sonunda becerdim... :)

Bugün kısa bir sürede açılıp kapanan bi kapı yaptım. Zaten her UE kursu konuya bunla başladığı için, biraz vakit ayırmış herkes ezbere biliyor sayılır.

![BP_Door]({% link /assets/images/BP_Door_Screenshot_01.png %})

BP'nin üç temel bileşeni var.

- Açma metodu:
Açma metodu tamamen dışarden açma komutunu vermek için kullanılıyor. Bunun için en basit haliyle oyuncudan dışarı bir Tarama alıp, kapı görürsek bu metodu çağırıyoruz. Açma metodu kapıya hangi konuma gitmesi gerektiğini söyleyip, bir de Tick'i etkin hale getiriyor

- Tick:
Burda kapının açılma hareketeini tamamlıyoruz. İstenen hedef ve şu anki dönme arasında bir interpolasyon yapıp (FInterp to Constant, sabit hız için), dönmeyi gövdeye uyguluyoruz. En sonunda ise kapı istediğimiz konuma geldiyse, 5 saniye sonra kapanacak şekilde saat kurup Tick'i tekrar kapatıyoruz.

- Kapama metodu: Burası da tıpkı açma gibi, yalnızce bir hedef seçmek yerine kapıyı hep ilk konumuna gönderiyor, yani 0'a.

Böylece günün sonunda, hep kitlenen oyuncumuzu kurtarmış hem de harita için çok gerekli şeyler'den biri olan kapıyı halletmiş olduk. Bu günlük bu kadar.