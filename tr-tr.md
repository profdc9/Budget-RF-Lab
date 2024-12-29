# Bütçe RF Laboratuvarı

Türkiye'deki ev yapımı radyo frekansı (RF) laboratuvarı için bütçe dostu bir rehber. Bu sayfa, `Bilgi Sistemleştirme (SoK)` makalesi olarak tasarlanmıştır.

*Lütfen bu listenin yardımcı olmak amacıyla derlendiğini ve bu makalede yer alan herhangi bir satıcı veya bağlantının ticari bir onayı olmadığını unutmayın.*

## Ekipman Listesi

| Sıra No | Adı                                                                                 | Montaj Süresi (dakika) | Maliyet (TRY)                                                                                                 | Yorumlar                                                                                                                                                               | Bağlantılar                                                                                                                                                                                                                                                           |
|--------|--------------------------------------------------------------------------------------|------------------------|---------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1      | Topraklama                                                                           | 2                      | ~0                                                                                                            | Düzenli bir 220v (Türkiye'deki standart hat voltajı) LED ampulü Canlı ve Toprak arasında kontrol etmek için kullanın.                                                  |                                                                                                                                                                                                                                                                 |
| 2      | RF Prob                                                                              | 60 dakika              | <200                                                                                                          |                                                                                                                                                                        | [Bu makaleyi](https://n5ese.com/rfprobe1.htm) takip ederek bir tane yapın.                                                                                                                                                                                          |
| 3      | Frekans jeneratörü (VFO)                                                             |                        | 500-700                                                                                                       |                                                                                                                                                                        | Detaylar: https://github.com/kholia/pico-hf-oscillator, Alternatif: Si5351 modülü kullanarak bir VFO yapmak için https://github.com/kholia/EasyVFO'yu kullanın ve bir hack olarak Raspberry Pico 2 kullanarak kısa dalga için bir VFO yapın                                                 |
| 4      | Frekans sayacı                                                                       | 2                      | 500-800                                                                                                       | Birçok kullanım durumunda, AF ve RF sinyallerinin frekansını kontrol etmek için bir osiloskop kullanılabilir. Not: Pico 2'nin birçok 5v toleranslı pini vardır, bu çok kullanışlı bir özelliktir! | DIY kullanarak Raspberry Pi Pico 2 ve şu projeleri takip ederek: https://github.com/kholia/pico_ft8_xcvr/tree/main/PicoFrequencyCounter-v2, https://github.com/kholia/pico_ft8_xcvr/tree/main/PicoFrequencyCounter, https://github.com/richardjkendall/rp2040-freq-counter |
| 5      | Ticari Frekans Sayacı                                                                |                        | 1100                                                                                                          | 9V Frekans Metre 500 MHz Yüksek Hassasiyetli Okuyucu RF                                                                                                                | İlgili: HF için bir RF frekans sayacı tamponu yapın https://www.nutsvolts.com/magazine/article/build-an-rf-frequency-counter-buffer-for-hf                                                                                                                      |
| 6      | Frekans referansı                                                                    | 15                     |                                                                                                               |                                                                                                                                                                        | DIY kullanarak https://github.com/kholia/uBlox7_TimePulse projesi                                                                                                                                                                                                    |
| 7      | Lehimleme Demiri                                                                     | NA                     | BABA i12 Lehimleme demiri - 4200, IKO Mikro Lehimleme Demir İstasyonu– 12V - 350, Soldron 25W - 350           | İyi lehimleme uçlarına (uçlar) ve seramik uçlara yatırım yapın! Daha düşük fiyatlı olanlar ısınmak için zaman alır ama bu sorun değil.                      |                                                                                                                                                                                                                                                                 |
| 8      | Multimetre                                                                           | NA                     | UNI-T UT33D+ - 800, Mastech MAS830L Dijital Multimetre - 700                                                  |                                                                                                                                                                        |                                                                                                                                                                                                                                                                 |
| 9      | Doğrusal güç kaynağı seçenekleri                                                     | NA                     | SUGON 3005D Ayarlanabilir DC Güç Kaynağı (30V~5A) - 5300, SUGON 3010PM Ayarlanabilir Güç Kaynağı (30V~10A) - 9000 | CC CV işlevselliği, deneyleri güvenli bir şekilde yürütmek için gereklidir!                                                                                                          |                                                                                                                                                                                                                                                                 |
| 10     | Kapasitans metre                                                                     | NA                     | MS8910 Mastech SMD Ölçüm Cımbızları - 2000                                                                  | VU2ESE de Mastech MS8910 kullanıyor                                                                                                                                         |                                                                                                                                                                                                                                                                 |
| 11     | Osiloskop                                                                           | NA                     | ~Bir kez al, bir kez ağla~                                                                                          | Herhangi bir >= 100 MHz Siglent osiloskop bütçenize uygundur. En azından bir DSO alın. Rigol osiloskoplar da iyidir. Owon osiloskoplar düşük bütçe için uygundur.                  |                                                                                                                                                                                                                                                                 |
| 12     | NanoVNA                                                                              | NA                     |                                                                                                               |                                                                                                                                                                        |                                                                                                                                                                                                                                                                 |
| 13     | TinySA (Ultra)                                                                       | NA                     |                                                                                                               | Synergy Telecom - Delhi'den zayıflatıcılar alın. Bir demet alın ve karıştırın.                                                                                    |                                                                                                                                                                                                                                                                 |
| 14     | RF güç + SWR metre                                                                   | NA                     | Diamond SX20C Güç Metre                                                                                     | RF çalışmaları için çapraz iğne güç ve swr metre çok kullanışlıdır.                                                                                                        |                                                                                                                                                                                                                                                                 |
| 15     | RF Dummy yük                                                                        | 30                     | 500-700                                                                                                       | 50 ohm RF flanş direnci + uygun bir alüminyum ısı emici kullanarak DIY                                                                                                |                                                                                                                                                                                                                                                                 |
| 16     | Sıcak hava istasyonu seçenekleri                                                    | NA                     | Bütçenize göre                                                                                         |                                                                                                                                                                        |                                                                                                                                                                                                                                                                 |
| 17     | SDR Seçenekleri                                                                      | NA                     | RTL-SDR v3 / v4, Airspy HF+ Discovery                                                                         | Airspy muhtemelen en iyi HF alıcısıdır(?)                                                                                                                   |                                                                                                                                                                                                                                                                 |
| 18     | Jumper kabloları                                                                     | NA                     |                                                                                                               | Yüksek kaliteli olanları satın alın, zaman kazandırır.                                                                                                                                     |                                                                                                                                                                                                                                                                 |
| 19     | Lehim sökme örgüsü (fitil)                                                           |                        |                                                                                                               | Chemtronics markalı olanları Otovon satıcısından satın alın                                                                                                                        |                                                                                                                                                                                                                                                                 |
| 20     | Büyütme                                                                             | NA                     | Bütçenize göre                                                                                          | Sıkışık bir durumda, 300 TRY'den başlayan ve ihtiyaçlarınıza göre yükseltebileceğiniz LED aydınlatmalı temel bir büyütme düzeni seçin.                               |                                                                                                                                                                                                                                                                 |
| 21     | Yerel WSPR / FT8 / CW 10mW RF kaynağı                                                | 2                      | ~500                                                                                                          |                                                                                                                                                                        | https://github.com/kholia/Easy-Digital-Beacons-v1, https://github.com/kholia/Pico-FT8-TX                                                                                                                                                                        |
| 22     | Yerel SSB sinyal kaynağı                                                             | 15                     |                                                                                                               | Sadece bir tel lehimlemek / takmak yeterlidir                                                                                                                           | https://github.com/kholia/rpitx                                                                                                                                                                                                                                 |
| 23     | Lehim teli                                                                          | NA                     |                                                                                                               | 22 SWG "60/40" karışımı rosin çekirdekli, daha ince SMD bileşenleri lehimlemek için 0.3mm lehim teli (2UUL veya Mechanic markalı) kullanın.                             |                                                                                                                                                                                                                                                                 |
| 24     | Hat Test Cihazı                                                                      | NA                     | ~100                                                                                                          | 400V'a kadar ölçüm aralığı                                                                                                                                           |                                                                                                                                                                                                                                                                 |
| 25     | Mengene / PCB Mengenesi                                                              | NA                     | 300-8000                                                                                                      | Taparia, vb. yerel bir hırdavatçıdan temel mengene                                                                                                               |                                                                                                                                                                                                                                                                 |
| 26     | Donanım araçları: ESD güvenli cımbız, burun pensesi, tornavida seti, yan kesiciler, kelepçe | NA                     |                                                                                                               | Taparia, Stanley ve bazı Miniso markalı setler genellikle iyi şeylerdir.                                                                                                 |                                                                                                                                                                                                                                                                 |
| 27     | LCR metre DE-5000                                                                    | NA                     | eBay (JP'den ithalat vergileri ile birlikte gelir)                                                                       | Oldukça iyi incelenmiş ve güvenilir                                                                                                                                    |                                                                                                                                                                                                                                                                 |
| 28     | Lehim Akısı                                                                          | NA                     | ~200                                                                                                          | Soldron iyi kaliteli akıdır                                              |                                                                                                                                                                        |                                                                                                                                                                                                                                                                 |

## RF güvenlik genişletilmiş listesi

- HackRF One

- CC1101 SPI modülü (iki)

- Mantık analizörü seçenekleri

  - DIY kullanarak Raspberry Pi Pico

    https://github.com/pico-coder/sigrok-pico

  - [Alternatif 1] DIY kullanarak Raspberry Pi Pico

    https://github.com/gusmanb/logicanalyzer

  - [Alternatif 2] https://robu.in/product/usb-logic-analyze-24m-8ch-mcu-arm-fpga-dsp-debug-tool/

- Hata enjeksiyonu

  - https://github.com/MKesenheimer/fault-injection-library

## Yazılım (Ücretsiz / FOSS)

- LTspice - Fikirlerinizi LTspice kullanarak kontrol edin

- Elsie (https://tonnesoftware.com/elsie.html) filtreler için - en iyi yazılım?

- http://www.ke5fx.com/aadeflt.htm - AADE Filtre Tasarımı V4.5

- https://www.dl0hst.de/mini-ringkern-rechner.htm#en

- https://coil32.net/ - bobin endüktans hesaplama uygulaması

- KiCad EDA (EAGLE öldü, diğer tescilli yazılımların da ölmesini bekliyoruz...)

## Eğlenceli Aktiviteler

- 30 dakika içinde HF'ye başlamak istiyorum? Bana nasıl olduğunu söyle!

  Bir Raspberry Pi Pico 2 MCU kartı kullanarak 10m bandı için 10mW WSPR işaretçisi yapın.

  https://github.com/kholia/Easy-Beacons-STEM kullanın.

  Alternatif: Zaten bir Raspberry Pi SBC'ye mi sahipsiniz? O zaman https://github.com/JamesP6000/WsprryPi'yi deneyin.

- Bugün HF trafiğini almaya başlamak istiyorum - bana nasıl olduğunu söyle!

  - RTL-SDR v3 + rastgele tel / aktif anten

  - CD2003 alıcı (< 500 TRY) + rastgele tel / aktif anten

    Daha fazla ayrıntı için bkz. https://github.com/kholia/ConsensusBasedTimeSync