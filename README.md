# Taiko-Hekla-Kontrat-Deploy
Taiko Hekla Kontrat Deploy İşlemi
Taiko Kontrat Deploy Etme

Sunucu Gereksinimleri: Nefes alsın yeter

Github codespace üzerinden sunucusuz da yapabilirsiniz

Sunucuyu güncelliyoruz

```
sudo apt update -y && sudo apt upgrade -y
```

Foundry'yi indirip çalıştırıyoruz

```
curl -L https://foundry.paradigm.xyz | bash
```

```
foundryup
```

Foundry ile proje oluşturma

```
forge init hello_foundry && cd hello_foundry
```

Burada hata alırsanız cd hello_foundry kodunu girebilirsiniz. Hata almazsanız devam

Deploy işlemi için satırları tek tek girin

```
forge create src/Counter.sol:Counter \
--rpc-url https://rpc.hekla.taiko.xyz \
--private-key CÜZDAN_ÖZEL_ANAHTARI
```

Söyle bir çıktı alırsanız işlem tamam

![Ekran görüntüsü 2024-04-26 152417](https://github.com/mcyucel/Taiko-Hekla-Kontrat-Deploy/assets/106594298/f58d6665-3f1b-480c-87a2-098667dbe004)
