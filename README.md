# SoftIto Yazılım ve Bilişim Akademisi - Mobile App Developer (Flutter Eğitimi) Genel Tekrar (30 Haziran - ..)

# 30 HAZİRAN

## CONTAINER
    - Bildiğiniz gibi kutu anlamına gelir. Önemli nokta:
        - Container, eğer çocuğu yoksa parent kadar yer kaplar!!!
        - Eğer çocuk atamıyorsan mutlaka en boy vermek zorundasın. Yani ben gidip bu containera bir tane color verirsem; tüm alanı kaplayacak. Eğer bir çocuk veriyorsanız onun kadar yer kaplar. Ama onun kadar da yer kaplamasını istemiyorsan, en boy vermelisin! 
        - Önemli: bir container içindeki çocuğun konumunu belirtebilirsiniz. alignment!! *
        - DAHA ÖNCE ÖĞRENMEDİN! Ben bu container'a width ve height vermeyeceğim. eğer bir container çocuğu varsa ve alignment varsa artık ÇOCUĞUNU DİNLEMEZ! ***
        - Container vermenin ana amacı bir alanı sınırlamak. Eğer bir alanı sınırlandırmayacaksan CONTAINER'A GEREK KALMAZ! **
        - Peki; ben bu container'ın sadece width ya da height'ını versem yeterli mi? EVET. HEIGHT OLARAK SINIRLANDIRIRR ANCAK WİDTH'İ SINIRLANDIRMAZ EXPANDED GİBİ DAVRANIR! **
        - Container'ın içindeki veri kadar değil ama sabit en boy alan belirlemek istiyorsam constraints özelliğini kullanacağız. bunun min ve max değerleri var.
## MARGIN AND PADDING DIFFERENCES
        - Container'da asla taşma hatası almazsın. TAŞMA HATASINI KESİNLİKLE ROW VE COLUMNDA ALIRSIN
        - padding: içteki elemenaların. container ile arasındaki mesafeyi belirtir. margindeki edge sınıfı hep ortaktır. eğer container in mesela bir width değeri yoksa ve sen yatay eksende padding verirse container bğüyğür ama eğer sınır verdiysen ve sığmıyorsa child in şeklini bozar yine de sığdırır. 
        - bir container 300*300 ise ve color red ise, o containerin child'ı 100*100 ve color blue ise blue kare görünmez. alignment.center dersen görünür. bu, child ve parent ilişkisi ile ilgilidir. alingment dediğin anda child'ın söz hakkı oluyor ve görünüyor! IMPORTANT! ***
    
## CENTER
        - İçine aldığı çocuğu, ortalamaya yarar ama DİKKAT:! Eğer içine aldığı yapı, çocuklar alan bir yapıysa (column, row, listview vs) SADECE YATAYDA YA DA DİKEYDE ORTALAR!

## DECORATION
        - YENİ BİR WIDGET ÖĞRENECEKSİN TEK ÖNEMİ: TASARIM YAPMAK İÇİN ÖNEMLİ BİR ŞEY SADECE.
        -  Container şekillendir:  bunun için decoration parametresi var içine BoxDecoration alır. (decoration: BoxDecoration(^^),)
        - shape: container'ın şeklini belirler. varsayılan rectangle'dır biz bunu circle yapabiliriz. 
        - image: containerın arka planı olarak resim ekleyebilriiz. bunu decorationn içi de yapmak zorundasınız. dikat direkt image vermeezsiniz decorationimage olarak vermelisin.
        - eğer shadow vereceksiniz bir arka plan renginizin olması gerekir.
        - eğer shadow verecekseniz bir bf lazım eğer yoksa shadow rengi arka planı da kaplar. blurradius gölge şiddeti, offset gölge yönü.

        align positioned stack - meriç 255 DAKİKADAN İTİBAREN İZLE
        1. resim ve yazının olduğu bir sunum hazırlanacak. (bol bol yazı olmasın, slayt kurallarına uy.) 2. sunumun dışında 1 tane de word dosyası hazırla. makale kurallarına uygun olarak. sunumda anlattığın her şey wordde de olmalı. 3 sunum yapılacak iyi hazırlan. en az 5 sayfa. 

        pazartesi: sunum hazırla kişilik envanter testini doldur, melek ile toplantı al.
        salı: nft frontendi hallet, mock datalar hazırla. 10 tane user 100 tane nft.
        çarşamba: profil kısımlarını settings'i hallet. sidebar yap. (hocaya tasarımı sun)
        perşembe: mongodb bağla ve admin panel yap. profil sayfalarını tasarla. (tasrım deadline)
        cuma: son kontrolleri yap, yetişmezse perşembedeki taskları yap.
        hafta sonu: bütün eksikleri kapat flutter projesine başlamış ol. 

        gradient: renk geçişi. decoration içerisinde. içine lineargradient alır bunun üç önemli parametresi vardır. colors: renk listesini alır. begin ve end."

        bugünkü plan:
        16.00'da çık evde 18.00'da ol. bi yemek ye 19.00 merter selçuk 19.30 melek 20.00 kişisel envanter 22.00 sunum
        column ve rowda align, stackte position kullan.

Ödev:

snack bar olacak validatorler çalışacak, tasarım basit olmayacak, login ve register anasayfaya yönlendirecek, bottom navigator, tabbar,

## EXPANDED
Expanded'ın mantığı boşlukları doldurmaktır. GREGOR SAMSA GİBİDİR.

## MATERIALAPP
- MaterialApp, uygulamamızı root'a bağlayan widgettır.  Bu yüzden uygulamanın genel bilgilerini içinde barındırır.
- Material'ın en önemli parametresi theme. bu parametre theme data sınıfını alır. ve bunun içerisine, arka plan rengi, özel tasarım yazı fontları, buton tasarımları, appbar ile ilgili tasarımlar, birçok şeyi araştır tabii barındırır.

