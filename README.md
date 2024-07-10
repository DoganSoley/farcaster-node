![image](https://github.com/DoganSoley/farcaster-node/assets/110679236/0db04e12-cd8d-4738-94b3-1dcf6d0294ff)

Kurulum videosu : https://youtu.be/4YmhkSM9ncg

# Farcaster Node Sunucu Gereksinimleri

16 GB RAM

4 GB CPU

40 GB SSD

Ben contabo'nun 9.50€'luk 16GB RAM - 6GB CPU - 400GB SSD sunucusunu kullanıcam.

Ben alırken setup fee yoktu ama kaldırmışlar onu sanırım sunucuyu alırken setup fee'ye dikkat edin alternatif olarak hetzneri de kullanabilirsiniz.

Sunucuya bağlandıktan sonra sırasıyla.

Güncellemeler

```
sudo apt update && sudo apt upgrade -y 
``` 

Screen Kurulumu

```
sudo apt install screen -y 
```
Screen açalım
```
screen -S farcaster
```
Node yükleme kodunu girelim 

```
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```

Daha sonra bizden ETH Mainnet ve OP Mainnet rpc isteyecek infura.io sitesinden aldığımız rpcleri girelim.

Daha sonra Warpcast uygulamasındaki Kullanıcı ID numarasını isteyecek Warpcast uygulamasını indirip kayıt olup onu da girelim.(yıllık 5$ kayıt ücreti var)

Yükleme bittikten sonra loglar akmaya başlayacak CTRL + A + D tuşlarıyla screen'den çıkabilirsiniz.

Kurulum bu kadar 

Kontrol etmek için tarayıcıya sunucuipadresi:3000 yazıp node durumunu görebilirsiniz.

Sunucu içerisine girip kontrol etmek için sunucuya bağlandıktan sonra 
```
screen -r farcaster
```
Yazarak kontrol edebilirsiniz.


# Güncelleme

Eğerki güncelleme gelirse güncelleme kodu(sunucuya bağlandıktan sonra)

```
cd ~/hubble && ./hubble.sh upgrade
```
Yükleme bitip loglar akmaya başladıktan sonra CTRL + C yapın veya terminali kapatıp tekrar bağlanın daha sonra ;
```
screen -r farcaster
```
```
cd ~/hubble && ./hubble.sh logs
```

Yazarak logları kontrol edin sorunsuz bir şekilde akıyorsa terminali kapatıp çıkabilirsiniz.

Tarayıcıya sunucuipadresi:3000 yazıp version'u kontrol edebilirsiniz.

Bu şekilde görünüyorsa sorunsuz çalışıyordur(kurduktan yaklaşık 5-6 saat sonra);
![image](https://github.com/DoganSoley/farcaster-node/assets/110679236/cc88de5f-f2ba-45e4-8114-59da93da4122)

