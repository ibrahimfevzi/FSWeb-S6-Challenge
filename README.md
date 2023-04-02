# React Sprint Challenge

**Talimatları dikkatlice okuyun.Sprint Challenge için tam olarak neler istendiğini iyice anlamadan başlamayın.**

Bu challenge, geçmiş sprint boyunca öğrenilen kavramları ve teknikleri uygulamanıza ve bunları somut bir projede uygulamanıza olanak tanır. Bu sprint boyunca **React'a giriş** yaptık. Bu sprint sırasında **React bileşenleri ve gelişmiş stilleme** üzerinde çalıştınız.

Bu Challenge'da, bir API'den alınan verileri kullanarak **bir Star Wars sayfası** oluşturarak bu becerilerdeki ustalığınızı göstereceksiniz.

Bu tek başına yapılması gereken bir projedir. Tüm çalışmayı tek başınıza yapacaksınız.

### Proje Kurulumu

- [ ] Forklayarak bir kopyasını oluşturun
- [ ] Forkunuzu klonlayın
- [ ] main branch üzerinde çalışın
- [ ] Push commits: `git push origin main`

## Proje Talimatları

### Giriş

Bu challenge'da, bir API'den elde edilen stilize edilmiş bir karakter listesi sunan bir web sayfası oluşturacaksınız. Verileri bir web sayfasına aktarabilmek, JavaScript geliştiricilerinin yaptığı işin büyük bir bölümünü oluşturur; bu meydan okuma, böyle bir görevi başarabilitenizi sınar.

Minimum Uygulanabilir Ürünü oluşturmak için (MVP) gereklilikler aşağıda sıralanmıştır, projeniz aşağıdaki çıktılara benzemelidir:

[Örnek](/ornek/ornek1.png)

[Diğer örnek](/ornek/ornek2.png) [çalışan hali]https://ergineer.com/assets/materials/as7fwyf-star-wars/

### Talimatlar

Bitmiş projeniz aşağıdaki tüm özelliklere sahip olmalıdır:

- [ ] Karakterleri çağırmak için şu endpointi(uç noktası) kullanın `[GET] https://swapi.dev/api/people/` ([msw](https://github.com/mswjs/msw)).
- [ ] Çekilen karakter listesini bir state e yazın.
- [ ] Karakterlerinizi DOM'a aktarın:

  1. Her bir karakteri render etmek için 'Karakter' isminde bir React bileşeni oluşturun.
  1. map metoduyla statedeki verileri listeleyin, ve tüm karakterleri Karakter bileşenini kullanarak sayfaya yazdırın.
  1. Tüm yazdırılan karaklerlerin ismi DOM'da mutlaka yer almalıdır (örnek. "Luke Skywalker").
  1. Karakterlerin isimleri HTML'ye sabit olarak yazılamaz. Bu veriler mutlaka API'den çekilmelidir.
  1. Bileşenler **styled-components** kullanılarak stillenmelidir.

  **Notlar:**

- Tarayıcı tarafından JavaScript kullanılarak uç noktadan elde edilen veriler, [msw](https://github.com/mswjs/msw). MSW'nin yaptığı her şeyi anlamanız şu an için gerekli değildir, yalnızca şimdilik axios'u `https://swapi.dev/api/people/` adresine istek göndermek için kullandığınızda gerekli verileri nasıl çekeceğinizi bilmeniz yeterlidir.
- Uç noktayı HTTPie veya Postman kullanarak test ederseniz, MSW isteği engellemeyeceğinden farklı sonuçlar elde edersiniz.
- Ek dosyalar oluşturabilirsiniz ancak **mevcut dosyaları veya klasörleri taşımayın veya ismini değiştirmeyin**.
- Ekstra kitaplıklar kurmak dışında `package.json` dosyanızı değiştirmeyin.
- "start" işlemi bazen yeni bağımlılıklar eklendikten sonra tıkanabilir ve yeniden başlatılması gerekebilir.
- Çözümünüzde en iyi yöntemleri kulanmanız, temiz ve profesyonel sonuçlar üretmeniz önemlidir.
- Yazım denetimi ve syntax denetimi de dahil olmak üzere çalışmanızı gözden geçirmek için zaman planlayın.
- MVP'yi karşılayan bir meydan okuma göndermek, çok fazla detay içerip de sonuç içermeyenbir meydan okuma göndermekten daha iyidir.

### Ek Hedefler

Gerekli şeyleri bitirdikten sonra çalışmanızı daha da ileri götürebilirsiniz. Bu hedefler, bu modülde öğrendiğiniz şeyler olabilir veya olmayabilir, ancak az önce çalıştığınız proje üzerine inşa edilirler. Zaman tanıyın, sınırlarınızı zorlayın ve aşağıdaki isteğe bağlı hedeflerden herhangi birini gerçekleştirip gerçekleştiremeyeceğinize bakın:

- [ ] Karakter bileşenini daha karmaşık hale getirin ve birkaç alt bileşene bölün.
- [ ] Karakterlerle işlenecek film bilgilerini elde etmek için `[GET] https://swapi.dev/api/films/` (msw) uç noktasını kullanın.
- [ ] State'e eklemeden önce API verilerinden gereksiz bilgileri kaldırmak için ayrı bir modülde bir yardımcı fonksiyon oluşturun.
- [ ] Stil bileşenleri ile effektler veya animasyonlar oluşturun.
- [ ] Bir dizi promise'ini çözmek için Promise.all'ı kullanın.

## Esnek Mülakat Soruları

1. React JS nedir ve hangi sorunları çözer? Yanıtınızı sınıfta tanıtılan kavramlarla ve web'deki kişisel araştırmanızla destekleyin.

React JS, Facebook tarafından geliştirilen bir JavaScript kütüphanesidir ve özellikle web uygulamalarının kullanıcı arayüzlerinin geliştirilmesinde kullanılır. React JS, birçok sorunu çözmek için tasarlanmıştır. Bunlardan bazıları şunlardır:

Karmaşık UI yönetimi: Web uygulamalarının kullanıcı arayüzlerinin yönetimi genellikle karmaşıktır ve React JS, UI bileşenlerinin modüler ve yeniden kullanılabilir bir şekilde tasarlanmasına olanak tanır. Bu, kodun daha kolay bakımını sağlar ve geliştirme sürecini hızlandırır.

Performans sorunları: Web uygulamalarının kullanıcı arayüzlerinin performansı, özellikle büyük ve karmaşık uygulamalarda sorun olabilir. React JS, sanal DOM (Document Object Model) kullanarak sadece değişen bileşenlerin güncellenmesine izin verir, bu da uygulamanın performansını artırır.

Karmaşık veri akışı: Web uygulamaları, genellikle farklı bileşenler arasında veri alışverişi yapar. React JS, veri akışını kolaylaştıran tek yönlü bir veri bağlama modeli kullanır. Bu, uygulamanın karmaşıklığını azaltır ve hata ayıklamayı kolaylaştırır.

Component encapsulation: React, her bileşenin kendi bağımsız bağlamında çalışmasına izin vererek bileşen sarmalama (component encapsulation) sağlar. Bu, her bileşenin kendi özelliklerini ve durumunu korumasına yardımcı olur ve uygulamanın daha güvenli hale gelmesini sağlar.

Kolay test edilebilirlik: React JS, bileşenlerin tek başına test edilebilmesine izin verir. Bu, yazılım geliştiricilerinin kodlarını daha kolay test edebilmelerine ve hataları daha kolay tespit edebilmelerine olanak tanır.

2. Bileşen statelerini tanımlayın.

React JS'teki bileşenler, bir kullanıcının bir web uygulamasında etkileşimde bulunduğu UI öğeleridir. Bileşen stateleri, bir bileşenin durumunu, özelliklerini ve davranışını yönetmek için kullanılır.

Bir bileşenin durumu, bileşenin içindeki verilerin anlık değeridir. Durum, bileşenin ilk oluşturulduğunda veya herhangi bir kullanıcı etkileşimi nedeniyle güncellendiğinde değişebilir. Bir bileşenin durumu, setState() yöntemi ile güncellenebilir.

Bir bileşenin özellikleri, bileşene sağlanan değerlerdir. Özellikler, genellikle bileşenin özelliklerini ve davranışını özelleştirmek için kullanılır. Bir bileşenin özellikleri, bileşenin oluşturulduğu ana bileşenden aktarılabilir ve genellikle bileşenin işlevleri tarafından kullanılabilir.

Bir bileşenin davranışı, bileşenin etkileşimleri sonucu gerçekleşen eylemleri tanımlayan kod bloklarıdır. Bileşen davranışları, kullanıcıların uygulama ile etkileşim kurduğunda veya uygulama içinde herhangi bir etkileşim gerçekleştirdiğinde gerçekleştirilebilir. Örneğin, bir düğmeye tıklandığında, bir bileşenin davranışı bu tıklama eylemine tepki vermek olabilir.

Bileşen stateleri, bir bileşenin durumunu, özelliklerini ve davranışını yönetmek için kullanılır ve React uygulamalarının ölçeklenebilir ve yeniden kullanılabilir olmasını sağlar.

3. Propları açıklayın.

React JS'teki bileşenlerin propları, bir bileşenin dış dünyadan alabileceği verilerdir ve bileşenin özelliklerini ve davranışını özelleştirmek için kullanılır. Proplar, bir bileşenin üst bileşeninden veya ana uygulamadan aktarılabilir.

Proplar, sadece okunabilir (read-only) olmalıdır ve bir bileşenin durumunun değiştirilmesi gerektiğinde setState() yöntemi kullanılmalıdır. Bir bileşen, aldığı propların değişmesi durumunda yeniden render edilebilir.

Proplar, bileşenlerin genellikle tekrar kullanılabilir ve özelleştirilebilir olmasını sağlar.

4. Side effektler nelerdir ve bir React bileşenindeki efektleri belirli state veya prop değişiklikleriyle nasıl senkronize edersiniz?

Side effect'ler, bir fonksiyonun dış dünyada bir etkileşimde bulunması sonucu gerçekleşen davranışlar veya değişikliklerdir. Örnek olarak, bir API isteği yapmak, bir dosyaya yazmak veya DOM elementlerinde bir değişiklik yapmak side effect örnekleri olabilir.

React bileşenleri, kullanıcı etkileşimleri veya bileşen durumlarındaki değişiklikler nedeniyle yeniden render edildiğinde side effect'lerin gerçekleştirilmesi için React tarafından sağlanan useEffect() kancası kullanılabilir. useEffect() kancası, bileşenin her render edilmesinden sonra çalışır ve belirli bir state veya prop değiştiğinde tekrar çalıştırılmasını sağlayabilir.

Örneğin, bir bileşen, bir API'den veri alarak bir liste oluşturuyorsa, useEffect() kancası, bileşenin ilgili props veya state değiştiğinde yeniden API isteği yapmasını ve listenin güncellenmesini sağlayabilir.
