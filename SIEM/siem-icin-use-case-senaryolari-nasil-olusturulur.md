

# SIEM için Use Case senaryoları nasıl oluşturulur?

## SIEM Nedir?

Security information and event management (Güvenlik bilgileri ve olay yönetimi SIEM) kısaca kurum/kuruluşa ait ağ, sistem, güvenlik, altyapı vb. sistemler tarafından oluşturulan logları toplayan, bu loglar üzerinden gerçek zamanlı ve geçmişe yönelik analiz yapabilen ve bu yolla siber tehditlerin ve güvenlik olaylarının tespit edilmesine olanak sağlayan teknolojidir. [1]

## Use Case Nedir?
Uygulama kullanıcılarının sistem ile olan etkileşimlerinin modellenmesidir. Kısaca kullanım durumu veya kullanım senaryoları olarak adlandırabiliriz.

_Web uygulaması için hazırlanan örnek bir use case diyagramı;_
	
![](https://miro.medium.com/max/697/1*07UtTjWkE_Z-wC4vxRr9gQ.png)


## Kullanım Senaryosu Nasıl Yazılır?
- Sistemi kimin doğrudan kullanacağını belirleyin. (Bunlar kullanıcılar)
- Bu kullanıcılardan birini seçin.
- O kullanıcının sistemle ne yapmak istediğini tanımlayın. Kullanıcının sistemle yaptığı her şey bir kullanım durumu(use-case) haline gelir.
- Her bir senaryo için, o kullanıcının ne yapması gerektiğine kadar verin.
- Her bir senaryo için, kullanının ne yaptığını ve sistemin kullanıcının davranışına yanıt olarak ne yaptığını açıklayın.
- Diğer tüm kullanıcılar için bu adımları tekrarlayın.[2]

## SIEM için Use Case örnekleri;

_“Bir kullanıcı arada hiç başarılı oturum açmadan 5 dakikada 3 tane oturum açma denesi yapıyor ve başarısız oluyorsa uyar”._

_“Aynı kullanıcı 2 farklı makinada 15 dakika içinde başarısız oturum deniyor ve 2. Başarısız oturumdan sonraki 5 dakika içerisinde bu makinalardan birinden tehdit istihbarat listesindeki bir IP ye erişim isteği oluyor ise uyar.”_

_“Bir kullanıcının günlük başarısız oturum sayısının başarısız oturum sayısına oranı anormal olursa uyar.”_

_“Herhangi bir kullanıcının DNS trafiğinin HTTP trafiğine oranı anormal olursa uyar.”_

_“15 dakikada aynı virüs 3 farklı makinede tespit edilir ve sonraki 5 dakika içerisinde bu makinalardan biri başarısız oturum yaparsa uyar.”_ [3]

Oluşturulacak olan SIEM senaryoları her zaman risklerinize ve önceliklerinize bağlı olmalıdır.

Örneğin, amacınız kullanıcılarınızın oturum bilgilerini nasıl kullandığını veya birileri oturum bilgilerini çaldığında tespit etmekse; Kullanıcılar ile ilgili oturum, erişim ve etkinlik kayıtları vb.. bilgilere sahip olmanız gerekir. Bu bilgiler ile kuruma özel istenilen şekilde korelasyonlar oluşturulup alarm üretilebilir.

Bir kullanıcı 1 dakika içinde 5 defa yanlış oturum açma denemesi yapıyor ve 6. denemesinde başarılı bir şekilde oturum açıyorsa;

- Kullanıcı parolasını unutmuş olabilir.
- Büyük küçük harf duyarlılığına takılmış olabilir.
- Bir başkası kullanıcının parolasını tahmin etmeye çalışıyor olabilir.
- gibi olasılıklar senaryo oluşturulurken göz önünde bulundurulmalıdır.

Aşağıdaki siteden farklı teknolojiler hakkında SIEM kullanım senaryolarını inceleyebilirsiniz.\
https://www.exabeam.com/siem-guide/siem-use-cases/

- - - -
Kaynak:
- https://www.gazikitabevi.com.tr/urun/siber-guvenlik-operasyonlari-merkezi [1]
- http://inform.nu/Articles/Vol7/v7p105-116-175.pdf [2]
- https://medium.com/@eakbas [3]
- https://blogs.gartner.com/anton-chuvakin/2014/05/14/popular-siem-starter-use-cases/
- https://www.researchgate.net/figure/Web-application-use-case-diagram_fig1_328871255
