
# Návrh funkcionality aplikácie pre bezpečné outdoorové aktivity

## 📌 FUNKCIONALITA 

---

### 1. AI prvá pomoc + rozpoznávanie symptómov + nadväzuje na bod 7
- **Funkcia:** Diagnostika na základe popisu symptómov alebo analýzy z kamery, vec post-bakalárskych updatov, kvôli náročnosti ako sme sa bavili počas konzultácie.
– AI na základe používateľského profilu (vek, pohlavie, skúsenosti, fyzická kondícia, prípadné zdravotné obmedzenia – napr. astma, tlak, diabetes)  vyhodnotí vhodnosť plánovanej trasy alebo aktivity.
---

### 2. SOS funkcia s GPS polohou
- **Funkcia:** Jedno-tlačidlové odoslanie núdzovej správy s polohou.
    - **Live feedback loop na štýl waze – hlásenia od komunity**
    Používateľ po výlete (alebo počas neho) môže nahlásiť aktuálne problémy alebo podmienky na trase. Tieto hlásenia sa okamžite zobrazujú ostatným používateľom plánujúcim trasu.
    Napr. „Padnutý strom blokuje chodník.“ - hlásenie by sa viazalo na GPS polohu a trasu.
    Možnosť vybrať typ incidentu na štýl Waze (bezpečnostné riziko / prírodná prekážka / faunálne riziko).
    Tým by sa komunita stala aktívnym prvkom bezpečnosti a aplikácia sa dynamicky aktualizuje o reálne podmienky v teréne jedinečnosť totožne, ktorou disponuje waze.
---    

### 3. Detekcia pádu a automatické varovanie
- **Funkcia:** AI analyzuje pohybové senzory telefónu na zistenie pádu.
**Náčrt funkcionality :**
- AI analyzuje pohybové senzory (akcelerometer, gyroskop) na detekciu pádu a automaticky vyhodnotí, či došlo k nehode. V prípade nereagovania používateľa po dobu zvolenej časovej zložky napr. 30 sec. spustí SOS režim s odoslaním GPS polohy a aktivuje AI asistenciu.
---

### 4. Záchranný režim s AI asistenciou
- **Funkcia:** Interaktívny AI sprievodca pri nehode, kontaktovanie záchrany.
- **Náčrt funckionality :**
- Po zistení nehody (napr. detekcia pádu, stlačenie SOS) sa textový sprievodca prepne do asistencie:
- „Zhlboka dýchajte, pokúste sa zastaviť krvácanie – nájdite lekárničku.“
- „Vaša poloha bola zaznamenaná, pomoc je na ceste – zvoľte bezpečnú polohu.“
- Znížime tým paniku, poskytuje konkrétne kroky v reálnom čase a zvyšuje šancu na správnu reakciu pri záchrane ľudského života.
---

### 5. Lokalizácia v CHKO (chránených krajinných oblastiach) + od tejto funckionality nadväzujú i nižšie uvedené 
- **Funkcia:** Detekcia polohy používateľa v rámci CHKO pomocou GPS.
- **Výstup:** Informácia o tom, v akom pásme sa nachádza a aké platia pravidlá.
- **Stav fauny:** Zoznam potenciálne výskytových druhov (napr. medveď, vlk).
---

### 6. Bezpečnostné upozornenia na výskyt nebezpečných živočíchov - nadväuje na bod 5
- **Funkcia:** Varovanie pred rizikom pri vstupe do nebezpečnej zóny.
- **Obsah:** Preventívne rady, obranné stratégie, správanie pri útoku.
---

### 7. Záznam trás + export do GPX + + rozšírené varovania a odporúčania
- **Funkcia:** Ukladanie, trasovanie pohybu, export do GPX pre zariadenia ako Garmin navigácia.
- **Rozšírenia:**
  - Zobrazenie varovaní pozdĺž naplánovanej trasy na základe:
    - Očakávaného počasia (napr. búrky, silný vietor, inverzia - zhoršená viditeľnosť).
    - Recenzií a hodnotení od ostatných používateľov, ktorí daný natrasovaný úsek už absolvovali.
    - Odporúčaní na náročnosť na základe napr. (typu povrchu a jeho schodnosti.), odporúčanie pre výbavu na základe aktuálnej       meteorologickej situácie, typu povrchu a jeho schodnosti. (napr. pevná obuv, mačky, trekingové paličky).
    - Subjektívneho hodnotenia obtiažnosti a bezpečnosti od ľudí, ktorí už danú trasu / časť absolvovali.
- **Inteligentné odporúčanie sprievodcu:** 
    - Pokiaľ systém vyhodnotí úsek ako potenciálne nebezpečný pre neskúseného používateľa (na základe poveternostných podmienok, náročnosti terénu a spätnej väzby), aplikácia automaticky odporučí kontakt na registrovaného lokálneho sprievodcu.
    - Používateľ bude mať možnosť sprievodcu priamo kontaktovať prostredníctvom aplikácie (napr. cez chat, volanie alebo e-mail).
    - Hodnotenia sprievodcov môžu byť súčasťou základnej funkcionality – jednoduché hviezdičkové hodnotenie a recenzie od turistov, ktorí už služby využili.
    - Táto funkcionalita zároveň otvára možnosť zapojenia sprievodcov do systému a vytvára pre nich priestor na čiastočnú zárobkovú činnosť, čím sa zvyšuje atraktivita aplikácie pre túto cieľovú skupinu.
**Inteligentné odporúčanie na základe zdravotného stavu nadväznosť na bod 1 :** 
    - Ak je plánovaná trasa nevhodná (napr. vysoké prevýšenie, zlá schodnosť, extrémne počasie), systém automaticky navrhne alternatívne trasy alebo odporučí predĺženie prípravy.
    - Možnosť prispôsobiť odporúčania pre rodiny s deťmi, seniorov, športovcov alebo ľudí s obmedzením pohybu.

---    

### 8. Mapy s označením rizikových úsekov + spája sa s bodom 7
- **Funkcia:** Vizualizácia trás + varovania (lavíny, zlý terén, zlé počasie).
---

### 9. Počasie a meteorologické upozornenia + spája sa s bodom 7
- **Funkcia:** Získanie predpovede a varovania na základe lokality.
---

### 10. Zoznam odporúčaného vybavenia podľa aktivity + spája sa s bodom 7
- **Funkcia:** Automatické odporúčanie výbavy (napr. oblečenie, lekárnička).
- **Implementačný status:** **Voliteľné do BP**
---

### 11. Zdieľanie polohy so skupinou 
- **Funkcia:** Real-time zobrazenie polohy priateľov/skupiny na mape.
- **Implementačný status:** **Voliteľné do BP**
---

### 12. História výletov a export údajov + nadväzuje na bod 1 
- **Funkcia:** Ukladanie a vizualizácia záznamov aktivít.
- **AI analýza denníka z výletu**
- Funkcia: Po absolvovaní výletu systém analyzuje dáta používateľa (trvanie trasy, tepová frekvencia, počet zastavení, zmeny výšky, detekované pády a iné parametre zo senzorov) a poskytne personalizované odporúčania.
- Možnosti výstupu, niečo na tento štýl:
- „Vaša priemerná tepová frekvencia pri výstupe bola 165 bpm – odporúčame spomaliť tempo alebo častejšie prestávky.“
- „Zaznamenali sme prudký pokles energie po 2/3 trasy – odporúčame hydratáciu alebo vyšší kalorický príjem.“
- Prepojenie s predchádzajúcimi výletmi: progresívna analýza výkonu a zlepšenia.
**Na tento bod môže nadväzovať nami prediskutovaná na konzultácií funckionalita opísaná v bode 14**
---

### 13. Monitorovanie vitálnych funkcií cez senzory telefónu
- **Funkcia:** Využitie dostupných senzorov telefónu (napr. kamera + blesk, gyroskop) na sledovanie základných vitálnych funkcií ako tepová frekvencia.
- **Poznámka:** Implementácia závisí od typu zariadenia a dostupnosti senzorov. Môže byť kombinovaná s AI na odhad stavu.
- **Implementačný status:** **Odstránený bod po konzultácií**
---

### 13. Vzdelávací modul (CHKO, fauna, flóra)
- **Funkcia:** Zobrazuje edukačný obsah o prírode podľa aktuálnej polohy používateľa – zameraný na CHKO, miestnu faunu a flóru.
#### Obsah:
- Informácie o chránených druhoch, rastlinách, zvieratách, typoch lesa.
- Popis ochranných zón CHKO a pravidiel v danom území.
- Ilustrované obrázky a stručné zaujímavosti („vedeli ste, že...“).
#### Personalizácia:
- Obsah sa prispôsobuje lokalite.
#### Eventuálny prínos:
- Zvyšuje povedomie o prírode a podporuje ekologicky zodpovedné správanie.
- Modul má nielen praktickú, ale aj vzdelávaciu funkciu – vhodné aj pre rodiny alebo školy.
- **Implementačný status:** **Voliteľné do BP**
---

### 14. Výzvy a súťaže medzi používateľmi nadväzuje na bod 14
- **Funkcia:** Gamifikácia – napr. „nachoď 10 km“, porovnávanie výkonov.
- **Implementačný status:** **Voliteľné do BP**

---


