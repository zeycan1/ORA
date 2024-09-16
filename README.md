# ORA
![image](https://github.com/user-attachments/assets/fd448aaf-8731-4e25-ae87-b3e6fad81d54)

SİSTEM GEREKSİNİMLERİ:

EN az 8GB RAM
Önerilen 12GB RAM



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
### Alchemy den mainnet ve sepolia rpc ve wss lerinizi alıp onlarıda ekleyin

![image](https://github.com/user-attachments/assets/b6841021-c169-4bcf-8703-240a985208d4)

### Bilgileriniz kaydettiğinize göre ctrl x ve sonra y ile çıkın
### Artık başlatalım
```
docker compose up -d
```
### Bu kısımbiraz uzun sürüyor. Sunucunuzun özelliklerine bağlı 5-10 dakika sürüyor

### Şekildeki gibi loglarınız görüyorsanız nodeniz çalışıyor demektir

![image](https://github.com/user-attachments/assets/ae8654cc-1c9e-42d9-b6ec-a2b0a12fb2c0)


#### Artık loglarımıza bakabiliriz
```
docker logs -f ora-tora -n 100
```

