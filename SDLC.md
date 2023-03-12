<h1 style="text-align: center; font-size: larger; font-style: oblique;">Yazılım Yaşam Döngüsü (Software Development Life Cycle)</h1>

Yazılımcının sıfırdan bir yazılım üretirkenki gereksinimlerini bilmesi, analizini yapması bir   taslak oluşturması, yazılımı gerçekleştirme süreci, yazılımı müşteriye teslim etmesi ve teslim ettiği yazılımın gerekli bakımlarının yapılması adımlarını kapsayan döngü şeklindeki çalışma planlarına yazılım yaşam-döngüsü (software development life cycle) adı verilir. Yazılımla ilgili gereksinimler üretim aşamasında sürekli olarak değişebileceğinden bu aşamalar döngü halindedir. Bu çalışma şekillerinin döngü halinde olması oluşabilecek herhangi bir durumda diğer adımlara dönebilmeyi mümkün kılar.

<div style="text-align: center;">

![SDLC](https://cdn-clekk.nitrocdn.com/tkvYXMZryjYrSVhxKeFTeXElceKUYHeV/assets/images/optimized/rev-54b50ac/wp-content/uploads/2021/05/Stages-sdlc.png)

</div>

Yazılımcının üretim aşamasında takip edeceği adımlar şunlardır:

* **Planlama:** Döngünün ilk aşaması olan planlamada üretilecek olan ürün hakkında temel ihtiyaçlar belirlenir, maliyetler hesaplanır ve bir zaman çizelgesi oluşturulur.

* **Analiz:**	Kısaca doküman oluşturma olarak da tanımlayabileceğimiz analiz aşamasında çalışanlar müşterinin istekleri doğrultusunda çalışma planı oluşturur. Gereksinimler detaylı bir şekilde dokümante edilir. Bu aşamada temel UML diyagramları çizilir.

* **Tasarım:** Analiz aşamasından sonra oluşan gereksinimlere dayanarak bu gereksinimleri yerine getirecek temel bir yazılım oluşturmaktır. Gereksinimleri karşılayan bir taslak oluşturulur da denebilir. İki başlık altında incelenir.

    * **Mantıksal Tasarım:** Halihazırda mevcut olan bir sistem yerine önerilen sistem yapısı kabaca oluşturulur.

    * **Fiziksel Tasarım:** Yazılımı oluşturan bileşenler ve bu bileşenlerin ayrıntılarını içerir.

* **Gerçekleştirim:** Tasarım aşamasında oluşturulan taslak bu aşamada detaylanmaya, hayat bulmaya başlar. Bu aşama sonunda yazılım müşteriye teslim edileceği halini alır. Bu aşama da kendi içinde iki bölümden oluşur. Birincisi kodlamayken ikincisi ve en önemli noktalardan bir tanesi de test bölümüdür. Yazılan kod ne kadar sık test edilirse hata payı ve bulunan hatanın düzeltilmesi (debug) de o kadar kolay ve hızlı olur.

* **Teslim ve Bakım:** Ürünün kodlaması ve test aşamaları bitirildikten sonra müşteriye teslim etme vakti gelmiştir. Ürün müşteriye teslim edildikten sonra bakım aşaması başlar. Müşteri geribildirimiyle beraber hata düzeltmeleri, yeni özellikler eklenmesi vs. işlemler bakım aşamasında gerçekleşir ve yeni versiyonlar yayınlanarak bu geribildirimlere cevap verilmiş olur. 

Bakım kısmında bahsedilen versiyon üründe yapılan değişiklikleri belirten ve genellikle üç haneden oluşan sayılardır denebiliriz. Örn: v1.3.7. Burada birinci hane yani 1, major value olarak adlandırılır ve üründeki köklü bir değişikliği simgeler. İkinci hane yani 3, minor value olarak adlandırılır ve üründe yapılan ufak ve ürünün ana işleyişine çok etki etmeyen değişiklikleri temsil eder. Son hane yani 7, ise ürüne hata düzeltmeleri (debug) işlemlerini temsil eder.

Yukarıda bahsettiğim adımları gerçekleştirirken bazı modeller kullanılır. Bunlardan bazıları:

* **Barok Modeli:** 1970’lerde ortaya çıkan ve artık kullanılmayan bir modeldir. Aşamalar arası geri dönüş mantığı belirlenmemiştir. Ayrıca günümüzde proje başında yaptığımız doküman oluşturma işlemini projenin kodlama ve test aşamalarından sonra yapmayı daha uygun görmüştür.

* **Big Bang Modeli:** Bu modelde gereksinimler tespit edildikten sonra çok az bir planlama ile kodlama işine girişilir. Küçük ekipler ve küçük projeler için idealdir. Projenin son çıkış tarihi belli değildir.

* **Şelale/Çağlayan (Waterfall) Modeli:** Günümüzde modası geçmeye başlasa da diğer modellere temel oluşturduğu ve basit olması nedeniyle önemlidir. Şelale modelinde Barok modelin aksine adımlar arasındaki geri dönüş tanımlanmıştır ve doküman oluşturma her adımda yapılır. Önceki adımın dokümanı oluşturulmadan ve testi gerçekleştirilmeden bir sonraki adıma geçilemez. Her adım bir sonraki adımın girdisidir. Ayrıca bu model sık değişiklik yapılmasına çok izin vermez. Bu yüzden müşteri geribildirimleriyle sürekli şekil değiştiren büyük projelerde kullanılması sağlıklı olmaz. 
<div style="text-align: center;">

![Modeller](https://www.w3schools.in/wp-content/uploads/2019/02/SDLC-Waterfall-Model.png?ezimgfmt=rs:411x410/rscb23/ngcb22/notWebP)

</div>
* **Kodla ve Düzelt (Code and Fix) Modeli:** Kontrolsüz, doküman oluşturulmadan, temel bir sürüm oluşturulup sürekli geliştirilmesine dayalı modeldir. Küçük projelerde kullanılır. Bakımı çok zordur çünkü herhangi bir dokuman oluşturulmamıştır. Maliyetlidir. Küçük-tecrübesiz firmalar daha yaygın olarak kullanır.

* **Artırımsal Geliştirme Modeli (Incremental Development):** Bu modelin ana teması, tasarım aşamasından sonra bir sürüm oluşturulur ve sürekli sürüm geliştirilerek yeni sürümler meydana getirilir. Bu geliştirme süreci program hazır olana dek devam eder. Sürekli geliştirilerek yeni sürümler çıkarıldığı için daha çok test imkânı bulur ve başarısızlık riski azdır. 

* **Prototipleme (Prototyping):** Bu modelde gereksinimler iyice kavrandıktan sonra hızlı bir şekilde planlama yapılır. Daha sonra tasarım ve gerçekleştirme aşamalarıyla birlikte bir prototip oluşturulur. Bu prototip müşteriye sunulur. Müşterinin geribildirimleri doğrultusunda yeni prototip tekrar müşteriye sunulur. Bu şekilde döngüye giren model, müşterinin isteklerini en düzgün şekilde karşılayan prototip oluşturulana kadar devam eder. Son prototip üzerine değerlendirmeler yapılır ve ürün son halini almış olur. Böyle hızlı ve müşteriyle sürekli beraber çalışıldığı için hata payı azdır fakat yine hızlı çalışıldığı için doküman oluşturma işi tam olarak yapılmaz.

* **V Modeli:** İki daldan oluşan ve aşağıda birleşerek V şeklini oluşturduğu için bu adı almıştır. Sol dalda üretim adımları ve sağ dalda ise bu üretim adımlarına karşılık gelecek şekilde kontrol adımları vardır. Bu modelin kullanımı ve proje takibi daha kolaydır. Üç temel çıktısı vardır: Kullanıcı modeli, Mimari model, Gerçekleştirim modeli.

<div style="text-align: center;">

![V](https://i0.wp.com/melsatar.blog/wp-content/uploads/2018/08/Screen-Shot-2018-08-28-at-2.19.21-PM.png?resize=768%2C501&ssl=1)

</div>

* **Spiral (Helezonik) Model:** Spiral model dört ana aşamadan oluşur. Planlama; Her adımda oluşturulacak olan ara ürünler için ve bu ara ürünlerin birleştirilmesi için planlama yapılması. Risk Analizi; Oluşabilecek risklerin araştırılması ve bunlara önden bir önlem alınması. Üretim; Ara ürünler üretilmesi. Kullanıcı Değerlendirmesi; Üretilen ara ürünlerin müşteriye sunulması ve müşterinin değerlendirmesinin ardından yaptığı geribildirimler. Bu adımların avantajları ise ara ürünler oluşturulması ve müşteriye sunulması aynı prototipleme modelindeki gibi ana ürüne daha emin adımlarla gidilmesini sağlar. Yapılan risk analizleri ve müşteriden gelen geribildirimler ile hata payı zaten neredeyse sıfıra indirgenir.

<div style="text-align: center;">

![Spiral](https://www.w3schools.in/wp-content/uploads/2019/02/SDLC-Spiral-Model.png?ezimgfmt=rs:559x353/rscb23/ng:webp/ngcb22)

</div>

* **Yeniden Kullanıma Yönelik Geliştirme(Re-used Based Development):** Son yıllarda kullanımı sıklaşan bu modelde daha önceden olan bir sistem yapılacak ürün için kullanılır. Bu model ne kadar zamandan tasarruf ettiriyor olsa da çalışanların daha önceden yapılmış bir sisteme kendi ürünlerini adapte etmeleri zorlu bir süreç. Bu yüzden bu modeli kullanan kuruluş veya grupların tecrübeli yazılımcılardan oluşmuş olması gerekir çünkü başka yerden hazır temin edilen sistem üzerinde değişiklik yapmak için belli bir bilgi birikimine sahip olmak gerek. Maliyeti fazladır.

* **Çevik Yazılım (Agile Programming) Modelleri:** Çevik yazılım modelinin ana teması proje küçük parçalara bölünerek çalışılır. Çevik yazılım müşteriyi her aşamada memnun etmeyi amaçlar bu yüzden sık aralıklarla ürün teslimi yaparak müşterinin değişken taleplerini takip eder. Basitlik ana prensiplerinden biridir. Küçük gruplar şeklinde çalışır.

<div style="text-align: center;">

![Agile](https://miesofficial.com/blog/wp-content/uploads/2021/03/agile-metodolojisi--768x510.png)

</div>

Çevik yazılım geliştirme modellerinden bazıları şunlardır:

* **Extreme Programming (XP):** Kent Beck ve arkadaşları tarafından 1996 yılında kurulan bu yöntem 4 temel kuraldan oluşur:

    1. *Basitlik:* Karmaşıklıktan ve uzun dokümanlardan kurtaran bu kural, yapılan işin sade ve anlaşılır olmasına dayanır.

    2. *Cesaret:* Projede ilerlendikçe yaşanacak karmaşıklıktan ve koddan korkmadan üstüne giderek çalışmaktır. Gerekirse yapılanlar çöpe atılmalıdır ama korkup yarım bırakılmamalıdır.

    3. *Geri Dönüş:* Müşteri ile ekip sürekli beraber hareket eder. Böylelikle erkenden yaşanabilecek hatalardan kurtulunur. Müşterinin değişen istekleri projeye daha rahat entegre edilir. 

    4. *İletişim:* Proje oluşturulurken en önemli ve genellikle zorlanılan kısım ekip içindeki iletişimdir. Bu yüzden XP bu konu üzerinde de durarak ekibin sürekli iletişim halinde bulunmasını kural edinmiştir.

* **Scrum Modeli:** Scrum ürün sahibi, yazılım geliştirme ekibi ve Scrum Master’dan oluşur. Takımın daha özgür çalışması hedeflenerek verimliliği ve yaratıcılığı arttırır. Scrumda kullanılan terimlerden bazıları şunlardır:

    - **Sprint:** Sprintler genellikle 2-4 hafta uzunluğunda olan, bir işin bitirilip üzerine konuşulabilecek duruma getirilene kadar çalışılan zaman dilimidir.

    * **Product Backolog:** Kısaca gereksinim listesi de diyebileceğimiz product backolog, ürün sahibinin müşterinin isteklerini dinleyerek bunları bir önem sırasına sokması ve bunu ekibe iletmesidir. Müşterinin değişen isteklerine göre product backolog üzerinde değişiklikler yapılabilir.

    - **Sprint Backolog:** Ekip product backolog üzerinde çalışacakları sprint boyunca takip edecekleri planlamayı ve zaman çizelgesini oluştururlar.

    - **Sprint Planning:** Girecekleri sprint maratonunda izlenecek yol vs. hakkında yaptıkları toplantıdır.

    - **Daily Scrum:** Gruptaki kişilerin günlük yaptıkları şeyleri konuştuğu, ilerlemenin hızlanmasına yardımcı ayak üstü yapılan konuşmalardır. En fazla 15 dakika sürer.

    - **Sprint Review:** Sprint süresi sonunda ortaya konan ürün, ürün sahibine tanıtılır. Ürün sahibi ürünü kontrol eder. Ayrıca müşteriden de geribildirimler alınır.

    - **Sprint Retrospective (Retro):** Sprint bittikten sonra Scrum Master ve ekibin yaptığı toplantıdır. Bu toplantıda sprint boyunca nelerin doğru nelerin yanlış yapıldığı konuşulur. Daha sonraki projelerde aynı hataların yapılmaması için yanlışlara çözümler üretilir.

<div style="text-align: center;">

![Scrum Cycle](https://a.storyblok.com/f/86602/720x469/a4c059e6ca/scrum-process.jpg/m/)

</div>

**Kullanılan Kaynaklar:**

* https://medium.com/@denizkilinc/yazılım-yaşam-döngüsü-temel-aşamaları-software-development-life-cycle-core-processes-197a4b503696

* https://hayririzacimen.medium.com/yazılım-yaşam-döngüsü-ve-süreç-modelleri-70fdfb2f8f77

* https://medium.com/@batincetin44/yazılım-yaşam-döngü-modelleri-2342547d0840

* https://caglartelef.com/yazilim-yasam-dongusu/

* https://caglartelef.com/cevik-yazilim-gelistirme/

* https://medium.com/@omerharuncetin/yazılım-yaşam-döngü-modelleri-543c7879a742

* https://medium.com/@secilcor/scrum-nedi̇r-6a4326951dd8

* Doç. Dr. Deniz Kılınç, İzmir Bakırçay Üniversitesi, Yazılım Mühendisliğine Giriş Dersi, 2. Hafta Yazılım Yaşam-Döngü Modelleri Sunumu 

<p style=text-align:right;> <b><i>Saner Yeşil</i></b> </p>