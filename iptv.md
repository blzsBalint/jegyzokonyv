# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Balázs Bálint    
**A mérés tárgya:** DVB-T jel fejállomásba küldése és IPTV rendszeren való kiadása  
**A mérés dátuma:** 2025. 02 .05   
**A mérést vezette:** Sándor Péter    

**Évfolyam:** 13. E  
**Csoport:** GYAK 1  
**Helyszín:** V3 Labor  
---

## 1. Feladatunk
   A feladat során ki kell építeni egy földfelszíni digitális TV vételi rendszert, amely az Avasi adótorony jelét használva. Először a jel erősségét és a fogható multiplexeket kell ellenőrizni egy jelszintmérő segítségével. Ezt követően a DVB-T jel bevezetésével és az IPTV stream létrehozásával kell konfigurálni a rendszert, figyelembe véve a multicast IP tartomány és a set-top-box beállításokat.

## 2. Alkalmazott eszközök

| Eszköz/Műszer neve                    | Típus                                                               |                                    
|---------------------------------------|---------------------------------------------------------------------|
| Antenna                               |  Beltéri vagy kültéri antenna                                       |                                                
| Fejállomás                            | LEMCO SCL-824CT 8 × DVB-S/S2/T/T2/C to 4 × DVB-T/C & IP (FTA)       |                                              
| Set-top box                           | MAG IPTV                                                            | 
| Hálózati eszköz                       |  IGMP protokollt támogató és DHCP képes router internet kapcsolattal|    
| Mérőműszer                            | METEK HDD digitális TV jelmérő                                      |      
| Koaxiális kábelek és csatlakozók      | :(                                                                  |                                                
| Jelosztó                              | :(                                                                  |                                              
| UTP kábelek az IPTV jel továbbításához| MAG IPTV                                                            | 
| Szerelési eszközök                    |  csavarhúzó, villáskulcs, kábelvágó, iránytű, dőlésszögmérő         |    
                           



  ## 3. Eszköz beállítások

| Eszköz/Műszer neve                    | Beállítása/ip/jelszó                                                |                                    
|---------------------------------------|---------------------------------------------------------------------|
| Lemco ip                              | 192.168.1.200                                                       |   
| R SSID password iptv                  | 12345678                                                            | 
| Lemco iptv stream                     | 239.1.1.1-39                                                        |
|                                                                                                             |
| Router (elérés)                       | 192.168.50.1                                                        | 
| Router login admin                    | admin12345678                                                       |    
| R SSID password iptv                  | 12345678                                                            | 

## 5.Lemco portok
| Port                                  |                          |                                    
|---------------------------------------|--------------------------|
| Input1                                | Multiplex B ch35         |                                                
| Input2                                | Miskolci Városi TV ch41  |                                              
| Input3                                | Multiplex A ch45         | 
| Input4                                | Multiplex E ch48         |    


  
  ## 6.Router portok
| Port                                  |                              |                                    
|---------------------------------------|------------------------------|
| Lan1                                  | Lemco control 1Gbps          |                                                
| Lan2                                  | ures                         |                                              
| Lan3                                  | Lemco ip stream 1Gbps        | 
| Lan4                                  | set top box 100Mbps          |

## 7.Mások számára is elérhető legyen ehhez szükséges információk
| Linkek                                                           |                                    
|------------------------------------------------------------------|
| http://192.168.1.1:8888/udp/239.1.1.1:1234                       |                                                
| ffmpeg -i http://192.168.1.1:8888/udp/239.1.1.1:1234 -f null -   |                                              
|ffplay -i http://192.168.1.1:8888/udp/239.1.1.1:1234 -sn          | 
  


## 8.Imputokon mért értékek
![input1](https://github.com/user-attachments/assets/7111c0ac-2ad6-4c2f-8573-5ed34a561baf)
![input2](https://github.com/user-attachments/assets/cb72e597-a218-4ddd-8ee9-6e1a419c42e7)

## 9.Mért eredmény
![cigány1](https://github.com/user-attachments/assets/af99768d-ee27-45e9-b553-065755e3510f)

## 10.Hitelessítés a vett jelről és minőségéről

![kep5](https://github.com/user-attachments/assets/cb12dc12-b780-421d-8407-cdf219b5dec7)

## 11.Vizuálisan bemutatva

![kep6](https://github.com/user-attachments/assets/28f0b367-0561-4940-af5f-a80ffa21c329)

## 12.Rövid élménybeszámolás
Egy komplex IPTV rendszer telepítése során a Miskolc, Avasi adótorony multiplexének vételére és streamelésére kaptam feladatot. Az antennát kültéri tripodra rögzítettem, majd iránytű és dőlésszögmérő segítségével precízen beállítottam az adótorony irányába. A METEK HDD mérőműszerrel finomhangoltam az antenna pozícióját, miközben spektrum analizátorral mértük a jelszinteket és a jelminőséget. A fejállomás konfigurálásakor a megfelelő multiplexeket hozzárendeltem a bemenetekhez, és multicast IP tartományt állítottam be a streamelt csatornákhoz. A végső tesztelés során a stream stabilitása és a hálózati paraméterek, mint a késleltetés és csomagvesztés is kiváló eredményeket mutattak.A stream stabil és a jelek kiváló minőségben érkeztek



**Aláírás:** Balázs Bálint

**Dátum:** 2025. 02. 05.







