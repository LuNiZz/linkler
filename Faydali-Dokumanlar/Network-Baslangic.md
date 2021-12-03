<h1>Network Temelleri</h1>

Bu dosyada ağ temellerimizi atacağız :)

<h2>Ağ nedir</h2>
<p>Ağ kısaca iki ve ikiden fazla cihazın kurallar içerisinde iletişim kurabilen cihazların oluşturduğu yapıdır.</p>

<h3>Özellikleri</h3>
<p> Cihazların birbirleri ile Dosya paylaşımı yapmasına, donanım paylaşımı yapmasına Kısaca paylaşım yapmasına olanak sağlar.</p>

<h2>Ağ donanımlarına giriş</h2>

<h3>İnternet kartı(NIC)</h3>
<p>Cihazların internete erişmelerini sağlar, IP ve MAC adres bilgilerini tutar.</p>

<h3>Switch</h3>
<p>Birçok cihazın ağa bağlanmasını sağlar, kendi aralarında haberleşmelerine olanak sağlar. OSI katman modelinde ikinci katman olan Veri İletim(Data link) katmanında çalışır yeni dağıtıcılarda OSI 3.Katman olan Ağ(Network) Katmanında da çalışabilir. </p>


<h3>Firewall</h3>
<p>Ağ(Network) Paketlerinin içeriğini okur ve bir tehlike içeriyorsa bloklar. Erişim izinlerini denetlemeden de sorumludur. İki türe ayrılır, Donanımsal Firewall Yazılımsal Firewall(Güvenlik duvarı gibi) </p>

<h2>Temel Network bilgisi</h2>

<h3>LAN(Local Area Network)</h3>

<p>Sınırlı alandaki internete bağlanan cihazları birbirine bağlayan ağdır yani evimizde Bilgisayar, Telefon gibi cihazları tek bir modeme bağladığımız zaman bu LAN ağı olur. </p>
<p>IP Örneği: 192.168.1.1</p>
<p>Modem bunu HOST ID(Birazdan geçiceğiz :)) Numarasını atar. Yani Bilgisayarımız 192.168.1.2 de ise Telefonumuza 192.168.1.3 verir.</p>

<h3>WAN(Wide Area Network)</h3>
<p>Dünya çapındaki cihazların birbirine bağlanmasını sağlayan ağdır.</p>
<p>Wide Area Network IP nizi internette ıp adresim yazarak öğrenebilirsiniz :)</p>

<h3>DNS</h3>
<p>Bilgisayar tarayıcıya girdiğimiz hiçbirşeyi anlamaz bunu anlamaz burda DNS devreye girer ve Bilgisayara adresi verir, her sitenin bir IP Karşılığı vardır örneğin www.google.com arattığımız zaman bilgisayar onu anlamaz burada devreye DNS girer ve google.com a ait IP yi bilgisayara tanıtır. </p>
<p>Örnek vermek gerekirse araba bilgisayar nagivasyonuda DNS sunucusu olarak örneklendirebiliriz.</p>



<h3>OSI Katman modeli</h3>
<p>Cihazların birbirleri ile nasıl iletişim kuracaklarını tanımlar. 7 Katmandan oluşur. Bunlar L-1 Physical(Fiber, Wirelees vb..), L-2 Data Link(Ethernet, Switch vb..), L3-Network(IP,ICMP), L4-Transport(TCP, UDP), L5-Session(API,Sockets) L6-Presentation(SSL,SSH,FTP vb..) L7-Application(HTTP, FTP, IRC, DNS[SSH])</p>
<p>Bu makalelerde de güzel anlatılmış.
https://bidb.itu.edu.tr/seyir-defteri/blog/2013/09/07/osi-katmanlar%C4%B1 - 
https://medium.com/bili%C5%9Fim-hareketi/osi-modeli-ve-7-katman-7c3bb467798c#:~:text=OSI%20modeli%20(Open%20System%20Interconnection,International%20Organization%20for%20Standardization)%20geli%C5%9Ftirmi%C5%9Ftir.</p>

<h3>Port</h3>
<p>Kısaca anlatmak gerekirse her uygulama belirli bir portdan sunulur. Bilgisayarda 65536 Port vardır, Burda bazı port numaraları listelenmiş göz aşinalığı olması iyi olur. https://www.f1teknoloji.com.tr/tcp-udp-port-listesi/ - https://tr.wikipedia.org/wiki/TCP_ve_UDP_ba%C4%9Flant%C4%B1_noktas%C4%B1_numaralar%C4%B1_listesi - https://www.sistemim.com/donan%C4%B1m-makaleleri/116-hangi-port-ne-ise-yarar </p>

<p>Burda da güzel bir kaynak var -> https://forum.donanimhaber.com/bilgisayardaki-baglanti-portlari-ve-gorevleri--31333235</p>

<h3>TCP/IP Paketleri</h3>

<p>Ağdaki en küçük yapılardır</p>

<p>Kaynak hedef gibi bilgiler içerir</p>
<p>Çıkarken her katmanda yeni bir bilgi eklenir</p>
<p>Enkapsülasyon: Bilgi ekleme işlemine denir</p>
<p>Deenkapsülasyon: Bilgi çıkarma işlemine denir</p>

<h2>İletim</h2>

<h3>Unicast</h3>

<p>Cihazdan cihaza yapılan iletim türü</p>

<h3>Multicast</h3>
<p>Cihazdan belli cihazlara yapılan iletim</p>

<h3>Broadcast</h3>
<p>Cihazdan Ağdaki tüm cihazlara yapılan iletim türü </p>

<h2>Network ID Host ID ve IP Sınıfları</h2>

<h3>Network ID</h3>
<p>Evlerimizde kullandığımız IP nin ilk üç kısmı Network IP olarak adlandırılır</p>

<h3>Host ID</h3>
<p>Evlerimizde kullandığımız IP nin son kısmı Host ID olarak adlandırılır.</p>

<p>Burda da güzel bir makale var -> https://www.ugureskici.com/notlarim-makalelerim/ip-sinif-araliklari</p>

<h2> Ağ servislerinden bazıları </h2>

<h3>DHCP</h3>
<p>Ağınızda olan bir network ile çalışan cihazlara otomatik IP ataması ve DNS ataması yapar. Ağa misafir biri geldiğinde ona otomatik olarak 8 günlüğüne yetki verir. Default olarak 8 gündür fakat bu süre artırıp azaltılabilir.

<h3>NAT</h3>
<p>https://medium.com/@gokhansengun/nat-network-address-translation-nedir-ve-nas%C4%B1l-%C3%A7al%C4%B1%C5%9F%C4%B1r-a2c8b6291de8 Burda resimli bir şekilde güzelce anlatılmış. </p>














