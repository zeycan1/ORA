# ORA

### SİSTEM GEREKSİNİMLERİ



### Docker Compose'u Yükleyin
```
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
### Docker Compose'a Çalıştırma İzni Verin
```
sudo chmod +x /usr/local/bin/docker-compose
```
### Yüklene versiyonu kontrol edin
```
docker-compose --version
``` 
### Aaşağıdaki gibi görünmelidir
```
docker-compose version 2.20.2, build xyz
```
### Artık kurulumun-muzu yapalım
```
cd
git clone https://github.com/ora-io/tora-docker-compose
cd tora-docker-compose
cp .env.example .env
nano .env
```
### Açılan env dosyasının içinde bazı değişiklikler yapacağız
### Kullanacğınız cüzdanın private keyini ekliyorsunuz
### Alcemy den mainnet ve sepolia rpc ve wss lerinizi alıp onlarıda ekleyin

![image](https://github.com/user-attachments/assets/b6841021-c169-4bcf-8703-240a985208d4)

### bilgileriniz kaydettiğinize göre ctrl x ve sonra y ile çıkın
### Artık başlatalım
```
docker compose up -d
```
### Bu kısımbiraz uzun sürüyor. Sunucunuzun özelliklerine bağlı 5-10 dakika sürüyor
#### Artık loglarımıza bakabiliriz
```
docker logs -f ora-tora -n 100
```

