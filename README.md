# kevgirmachine
#   KEVGİR SANAL  MAKİNASININ/SENARYOSUNUN   ÇÖZÜMÜ
> NOT: KevgirIP  = KVIP , LİNUX2021 = L21 , 
- Öncelikle  kevgir nedir onun tanımını bir yapalım  kevgir makinası [canyoupwn.me](https://canyoupwn.me/) sitesinde  bulunan zaafiyetli  sanal makinalardan bir tanesi  biz üzerinde  bulunan zaafiyetlerden yararlanarak giriş yapacağız .
 
# 1. Adım 
- Ben sanal makinayı çözmek için [VirtualBox](https://www.virtualbox.org/) kullanıyorum .VirtualBox içerisine linux-2021  kurarark bu adımları gerçekleştirdim ,siz isterseniz WMmare Wrokstation kullanarak da çözümleri yapabilirsiniz  
- VirtualBox kurduktan sonra "Dosya>cihazı içe aktar seçeneği" ile ".ova " uzantılı  dosya olarak indirdiğimiz makinamızı içine kurabilirsiniz 
-  [Kevgir](https://canyoupwn.me/kevgir-vulnerable-vm/) 'in linkini bırakıyorum buradan indirebilirsiniz .

# 2.Adım 
- Makinamızı indirdikten sonra ayaklandırıyoruz /  açıyoruz  
- Kevgir bizim hedef makinamız ve onu bulmamız için  L21 i de ayaklandırıyoruz ve terminali açıyoruz  .
- Host  keşif süreci için [nmap](https://www.beyaz.net/tr/guvenlik/makaleler/nmap_nedir_ve_nasil_kullanilir.html) keşif aracını kullanacağız 
> Makina keşif adımlarında ilk adımm host keşfi adımı bunun en çok kullanılan araç olan nmap aracını kullanacağız .nmap hoost keşif aşamasında farklı paramatreler girerek istediğimiz özdellikleri taşıyan makinalar hangisi onları keşfederek önümüze getirir biz de buna bakarak aradğımız makina hangisi ona göre eşleşmeler yaparak doğru hedefi bulmaya çalışırız .
- nmap aracını kullanamak için vereceğimiz parametreler aşağıdaki gibi olmalıdır 
 > sudo nmap -Pn  -vv -O -A 196.168.1.0/24 -sV 

Bazı nmap komutları 
-  -Pn :ping olmadan tarama 
-  -vv: bir sonuç bulduğu zaman direkt ekrana sonucu yazdır 
- -O : işletim sistemi taraması için
- -A :all yani hepsi için 
- -sV : versiyon taraması için 
-  -sU :udp taraması için 
-  -sS :sync/ senkronizasyon taraması için   
- -p :belirtilen port ya da port aralığını tarar
- --top- x: ilk x portu tarar
- sudo : super user do (root yetkisi)
- -sT :TCP taraması 
-  196.168.1.0/24 parametresi irl ağdaki tüm  IPlerin portlarını  tarar 
> bu işlem ilk yaptığımızda uzun sürebilir IPyi  daha doğrusu pc adını  bulduğumuzda IP yi keşfetmiş olacağız ve  işimiz kolaylaşacak 
- aşağıda  satırları okuduğumzda host ismi olarak "canyoupwnme" ismini görüyoruz bu da doğru IPyi bulduğumuzu gösteriyor 
![](https://github.com/shilanbashchi/images/blob/main/VirtualBox_Kali-Linux-2021.%20canyoupwnme.host.png)
- diğer satırlara baktığımızda title olarak KEVGİR VM adını görüyoruz 
![](https://github.com/shilanbashchi/images/blob/main/VirtualBox_Kali-Linux-2021.4-virtualbox-amd64_18_05_2022_17_06_34.png)




            
           
