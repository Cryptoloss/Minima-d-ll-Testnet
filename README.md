# Minima Node Testnet Katılım

_Ücretsiz Sunucuyla Minima Node Testnet Katılım_

**Sosyal Medya Hesaplarımız**

[Youtube](https://www.youtube.com/channel/UCKIpdWDFJN59nkVQHn5xfZA) [Twitter](https://twitter.com/Cryptoloss1) [Telegram](https://t.me/LossNode)

Minimayı Telefondan Kurmak Ve Ödülün Detaylarını Öğrenmek İsteyenler için [Link](https://medium.com/@klayc973/arkada%C5%9Flar-selam-bug%C3%BCn-minima-ile-node-kuraca%C4%9F%C4%B1z-ve-herg%C3%BCn-1-adet-token-kazanaca%C4%9F%C4%B1z-kurulum-%C3%A7ok-7bb93d90e74f)

Selam dostlar bugün sizlerle Amazon AWS ücretsiz sanal sunucusu ile Minima Node testnetine katılacağız

![minima](https://user-images.githubusercontent.com/98783018/177717740-1752922c-823d-4972-9804-dd4319f56a32.png)

Öncelikle [AWS'ye](https://aws.amazon.com/) ücretsiz kayıt olalım. Bu ücretsiz sanal sunucu bize yeter de artar bile minima kurmak için.

Hesabı açtından sonra biraz aşşağıya gelip launch a virtual machine butonuna basıyoruz.

![image](https://user-images.githubusercontent.com/98783018/177721801-0aca2d43-d3fd-4481-a427-42d5a82ae0bf.png)

Resimdeki işlemlerin aynısını yapalım.(Ubuntu 20.04 seçiyoruz)

![image](https://user-images.githubusercontent.com/98783018/177722532-a85ef6bd-e8ed-4f0a-90e9-1b8e7bc43fe7.png)

Daha sonra create a keypair diyoruz ve keypair name belirleyip bir dosya indiriyoruz daha sonra hiçbirşey değiştirmeden sağ tarafda bulunan launch an instance butonuna basıyoruz

![image](https://user-images.githubusercontent.com/98783018/177722863-5554b492-86c1-4736-8bf5-c4744320f728.png)

Yukarıdaki işlemler bittikten sonra sol üstt tarafda kırmızı ile çizdiğim yerde 3 nokta olacak onu basıp intances paneline geliyoruz

![image](https://user-images.githubusercontent.com/98783018/177723642-04dad557-b057-4165-897d-e1cc61b16020.png)

Instance state kısmı running olana kadar bekliyoruz. Ardından okla gösterdiğim ID kısmına tıklayıp sunucunun içine giriyoruz

![image](https://user-images.githubusercontent.com/98783018/177723921-566fdb49-80d5-4345-90f0-1f91fe20f08c.png)

Şimdi tek yapmamız gereken connect butonuna basıyoruz

![image](https://user-images.githubusercontent.com/98783018/177724188-00691029-1a39-4afc-82ac-0e672f14454c.png)

Açılan menü içerisinden tekrar connecte basarak terminale geçiş yapıyoruz

![image](https://user-images.githubusercontent.com/98783018/177728626-bfde19b4-e368-4640-ad90-c273272f8bde.png)

**İlk Komutumuzla başlayalım.(kopyalayıp yapıştıralım)**

```
wget -O minima_setup.sh https://raw.githubusercontent.com/minima-global/Minima/master/scripts/minima_setup.sh && chmod +x minima_setup.sh && sudo ./minima_setup.sh -r 9002 -p 9001
```

Yükleme işlemi arkada devam ederken size vereceğim link ile kaydolup ıncentive ID alalım. Kopyalayın hazır bulunsun elimizin altında

Link:https://incentive.minima.global/account/register?inviteCode=IRJ2IFPH

![image](https://user-images.githubusercontent.com/98783018/177730398-d0553b0d-dab5-45a4-9696-a2e68cac91fc.png)

işaretlediğim yerden önceki komutları görmeye başladığınızda kurulumun bittiğini anlıyoruz ve CTRL + C tuşlarına basıyoruz.

![image](https://user-images.githubusercontent.com/98783018/177732286-3bcb74e3-1a15-44a8-9366-48f1200d64bc.png)

**Şimdi verdiğim koddaki XXXX yazan yere kendi incentive adresinizi yazıp daha sonra komutun hepsini kopyalayıp yapıtıştırıyorsunuz**

```
curl 127.0.0.1:9002/incentivecash+uid:XXXXXXXXXXX
```

**Örnek**

```
curl 127.0.0.1:9002/incentivecash+uid:ba8sf28e-axb9-4d30-a24d-745b762
```

Fotoğraftaki last ping panelinden nodenin çalışıp çalışmadığını kontrol edebilirsiniz.

![image](https://user-images.githubusercontent.com/98783018/177734428-cbb9fc41-7b67-4301-8399-30c536453c53.png)

