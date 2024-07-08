![image](https://github.com/DoganSoley/farcaster-node/assets/110679236/0db04e12-cd8d-4738-94b3-1dcf6d0294ff)
# Farcaster Node Sunucu Gereksinimleri

16 GB RAM

4 GB CPU

40 GB SSD

Ben contabo'nun 9.50€'luk 16GB RAM - 6GB CPU - 200GB SSD sunucusunu kullanıcam.

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
screen -S Farcaster
```
Node yükleme kodunu girelim 

```
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```

Daha sonra bizden ETH Mainnet ve OP Mainnet rpc isteyecek infuradan aldığımız rpcleri girelim.
Daha sonra Warpcast uygulamasındaki Kullanıcı ID numarasını isteyecek onu da girelim.

Yükleme bittikten sonra loglar akmaya başlayacak CTRL + A + D tuşlarıyla screen'den çıkabilirsiniz.

Kurulum bu kadar 

Kontrol etmek için tarayıcıya ipadresi:3000 yazıp node durumunu görebilirsiniz.

Sunucu içerisine girip kontrol etmek için sunucuya bağlandıktan sonra 
```
screen -r farcaster
```
Yazarak kontrol edebilirsiniz.

Eğerki güncelleme gelirse güncelleme kodu(sunucuya bağlandıktan sonra)

```
cd ~/hubble && ./hubble.sh upgrade
```
