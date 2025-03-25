# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Balázs Bálint  
**A mérés tárgya:** Frekvencia vs. moduláció mérés


**A mérés száma:** 4. mérés  
**A mérés dátuma:** 2024. 11. 27  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

# Mérési Jegyzőkönyv

## 1. Mérés Célja
A mérés célja a **Johansson 8202 DVB-T modulátor** működésének megismerése, konfigurációjának tesztelése, valamint a METEK HD spektrum- és jelszintanalizátor használatával a modulátor által generált jel paramétereinek mérése. A mért paraméterek: **jelszint**, **bitsebesség**, **MER (Modulation Error Rate)**.

---

## 2. Használt Eszközök

| Eszköz                     | Típus                       | Funkció                                           |
|----------------------------|-----------------------------|---------------------------------------------------|
| Johansson 8202             | DVB-T modulátor            | Bitsebesség és jelminőség vizsgálata              |
| RF kábel                   | Koaxiális kábel            | Modulátorok és spektrumanalizátor összekötése     |
| Metek HDD                  | Spektrum/jelszint analizátor| Frekvencia, moduláció, sávszélesség, jelszint, MER és bitsebesség mérése |

---

## 3. Beállítások
- **Frekvencia**: 594 MHz  
- **Sávszélesség**: 8 MHz  
- **Modulációs típusok tesztelése**:  
  - QPSK  
  - 16QAM  
  - 64QAM  

---

## 4. Mérési Eredmények
Az alábbi táblázatban összefoglaljuk a mérések eredményeit különböző modulációs beállítások mellett.

| **Moduláció** | **Jelszint [dBm]** | **Bitsebesség [Mbps]** | **MER [dB]** |
|---------------|---------------------|------------------------|--------------|
| QPSK          | -12.5 dBm          | 3.3 - 4.9 Mbps        | 39.9 dB      |
| 16QAM         | -12.4 dBm          | 6.2 - 9.6 Mbps       | 35.8 dB      |
| 64QAM         | -14.2 dBm          | 13.7 - 14.6 Mbps      | 40.0 dB      |

---

## 5. Lépések
1. **Modulátor konfigurációja**:
   - A Johansson 8202 DVB-T modulátoron beállítottuk a kívánt frekvenciát (594 MHz) és a sávszélességet (8 MHz).  
   - A modulációs típusokat egyesével módosítottuk: QPSK, 16QAM, 64QAM.

2. **Jel vizsgálata METEK HD analizátorral**:
   - Az RF kábellel csatlakoztattuk a METEK HD spektrum/jelszint analizátort a modulátor kimenetéhez.  
   - Minden egyes modulációs típus esetén elvégeztük a jelszint, bitsebesség és MER mérést.  

---

## 6. Következtetések

A modulációs típus növelésével (QPSK → 64QAM) a bitsebesség jelentősen megnövekedett, de a MER (Modulációs Hiba Arány) értékek nem mutattak egyértelmű tendenciát.

A mérések a DVB-T elméleti követelményeinek megfelelő eredményeket adtak.




---

## 7. Megjegyzések
-A méréseket zavartalan környezeti feltételek között, zavarforrásoktól mentes, kontrollált helyiségben végeztük, biztosítva ezzel a pontos és megbízható eredményeket.

-Az adatok alapján egyértelműen megfigyelhetőek voltak a különböző modulációs technikák közötti eltérések, különösen a bitsebesség és a jel/zaj viszony tekintetében, ami alátámasztotta a modulációs rendek hatását a rendszer teljesítményére.





---


## 8. Diagramm
mérési diagram 
<img src="https://github.com/user-attachments/assets/273fd5e1-7825-488c-9aeb-4f2d756d3d7e"/>


---

## 9. Záró Összegzés

-A modulációs típus növelésével (QPSK → 64QAM) a bitsebesség jelentősen emelkedett, míg a MER értékek nem mutattak egyértelmű trendet.

-A különböző modulációs technikák közötti eltérések jól megfigyelhetők voltak, különösen a bitsebesség és a jel/zaj viszony tekintetében.

-Az eredmények a DVB-T elméleti követelményeinek megfelelően alakultak, megerősítve a rendszer megfelelőségét.

---

## 10. Mért Képek

<details>
<summary>Kattins a részletekért</summary>

<br>

<img src="https://github.com/user-attachments/assets/51f72b17-a5ec-49cc-a80b-c8b0cdf96a61"/>

<br>

<img src="https://github.com/user-attachments/assets/52f96f4b-f96c-40f8-9935-25e565455934"/>

<br>

<img src="https://github.com/user-attachments/assets/05516812-0421-4d1c-814e-06d08416e90c"/>

<br>

<img src="https://github.com/user-attachments/assets/00ec0d27-c911-4389-9bc9-bf826b170bbd"/>

<br>

<img src="https://github.com/user-attachments/assets/ed92dc9a-a7da-4c8d-9a95-79f5ad706cf6"/>

<br>

<img src="https://github.com/user-attachments/assets/27e537f4-0962-4efc-8c76-b9389efa1510"/>

<br>

<img src="https://github.com/user-attachments/assets/dd5c841d-5108-46ee-b11c-eb30b44fe819"/>

<br>



<br>

</details>

**Aláírás:** Balázs Bálint

**Dátum:** 2024. 11. 27.
