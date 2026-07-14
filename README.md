<!-- ZGDATA_TOOLKIT_CHANGELOG_START -->
## ZgData Toolkit - verzije

### 1.1.0 - Multi-cloud izdanje (14.07.2026.)

**Multi-cloud konfiguracija**
- Dodani Alwyzon i Hetzner kao aktivni cloud targeti.
- DataBox je pripremljen u konfiguraciji i ostaje neaktivan do podizanja virtualke.
- SQL test ostaje zaseban i nije vezan uz odabrani cloud target.

**NaÄini rada**
- Dodani `Single target` i `Compare cloud targets`.
- Ping prema viÅ¡e targeta prati se paralelno.
- iPerf upload/download testovi izvode se strogo sekvencijalno kako se mjerenja ne bi meÄ‘usobno zaguÅ¡ivala.
- Extended i Burn-In rotiraju periodiÄna iPerf mjerenja meÄ‘u odabranim targetima.

**Rezultati i report**
- Dodana zajedniÄka Results tablica sa svim odabranim providerima.
- Dodane side-by-side tablice za Internet Quality, ping, iPerf, DNS i traceroute.
- Dodana oznaka `Best measured network path`; ona opisuje samo izmjereni put u konkretnom testu, a ne ukupni poredak providera.
- Detaljni grafovi po targetu ostaju dostupni, ali su sklopljeni radi lakÅ¡eg pregleda.
- Dodani internet provider klijenta, public IP, ASN i pribliÅ¾na lokacija javne IP adrese.

**Pouzdanost i UI**
- Dodani warm-up pingovi koji ne ulaze u packet loss, availability, grafove ni incidente.
- Stvarni prekidi nakon poÄetka mjerenja i dalje se uredno biljeÅ¾e.
- Status i postotak premjeÅ¡teni su unutar progress bara radi boljeg prikaza na manjim ekranima.
- Ispravljen je odrezani tekst `Compare cloud targets`.
- Quick report jasno navodi da traceroute nije dio Quick profila.

**Infrastruktura**
- Dodane Linux instalacijske i verifikacijske skripte za dijagnostiÄke nodeove.
- Postavljen i provjeren Hetzner Falkenstein node na `diag-hetzner.zgdata.hr:5201`.
- Alwyzon ostaje primarni i centralni node na `diag.zgdata.hr:5201`.
- DataBox Ä‡e se ukljuÄiti naknadno na `diag-databox.zgdata.hr:5201`.

### 1.0.0 - PoÄetno izdanje
- Windows WPF aplikacija na .NET 8.
- Quick, Standard, Extended i Burn-In profili.
- Internet Quality, continuous ping, opcionalni SQL TCP monitoring, iPerf3, DNS i traceroute.
- STOP s djelomiÄnim HTML reportom.
- Informacije o raÄunalu i mreÅ¾i, incident timeline i inline SVG grafikoni.
- Self-contained Windows x64 publish paket.
<!-- ZGDATA_TOOLKIT_CHANGELOG_END -->

