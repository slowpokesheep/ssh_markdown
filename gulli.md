#### Tenging á milli biðlara og vefþjóns með SSH

![](http://m.quickmeme.com/img/b0/b06da8c574e952e26317cd138399665cb06d64396a2f00a9921f5eb7280a4758.jpg)

---

### Þrjú skref:

1. Biðlarinn auðkennir þjóninn.

2. Búinn til lotulykill (session key) til að dulkóða og afkóða skilaboð.

3. Þjónninn auðkennir biðlarann.

---

#### Skref 1 (biðlarinn auðkennir þjóninn)

* Ef biðlarinn er að tengjast þjóninum í fyrsta skiptið er hann beðinn um að auðkenna lykilinn handvirkt.

* Ef biðlarinn samþykkir er lyklinum bætt við í *~/.ssh/known_hosts* skránna.

----

![](https://i.imgur.com/vIwKlF8.png)

----

* Gert til að muna hvaða þjónum biðlarinn hefur tengst áður. 

* Verst t.d. DNS árásum.

* Ef biðlarinn þekkir ekki lykilinn fær hann kærkomna villumeldingu.

---

#### Skref 2 (lotulykill)

* lotulykil nauðsynlegur til að dulkóða og afkóða skilaboð.

* Samhverfir (symmetric) lyklaalgoriðmar nota einn lykil til að dulkóða og afkóða, ósamhverfir (asymmetric) tvo.

* Diffie-Helmann mjög algengur ósamhverfur algoriðmi.

* Notum Diffie-Helmann til að búa til sameiginlegt, samhverft leyndarmál á milli biðlara og þjóns.

----

#### Einfalt litadæmi

![](https://i.imgur.com/UBDlMhs.png)

----

![](https://i.imgur.com/1HBglSw.png)

----

![](https://i.imgur.com/zDHBsyJ.png)

----

![](https://i.imgur.com/ey7bz3V.png)

---

#### Skref 3 (þjónninn auðkennir biðlarann)

* Einfaldasta aðferðin að nota lykilorð. 

* Ekki mælt með vegna takmarkana á flækjustigi lykilorða.

* Mælt með að nota SSH lyklapör.

----

<img src="https://i.imgur.com/kuE5K6R.png" width=1000 />

----

<img src="https://i.imgur.com/NUtPve6.png" height=650 />

----

<img src="https://i.imgur.com/a1bXcmp.png" height=650 />

----

#### Ósamhverfir lyklaalgorðmar

Án þess að vita neina stærðfræði á bakvið lyklaalgoriðma þurfum við að treysta þessu tvennu um ósamhverfa lyklaalgoriðma:

----

1. Öll skilaboð sem eru dulkóðuð með lyklinum hjá aðila geta einungis verið afkóðuð með einkalykli aðilans.

2. Aðili með aðgang að almenna lyklinum hjá aðila getur staðfest ef skilaboð voru send af einhverjum með aðgang að einkalykli aðilans.

----

### Auðkennisskref

1. Biðlarinn sendir auðkennisskilaboð um hvaða lyklapar hann vill nota til að tengjast við þjóninn.

2. Þjónninn skoðar authorized_keys skránna, ef hann finnur almennan lykil fyrir þetta auðkenni þá sendir þjónninn skilaboð til biðlarans, dulkóðuð með lyklinum.

----

3. Skilaboðin geta einungis verið afkóðuð með samsvarandi einkalykli, ef biðlarinn er með hann afkóðar hann skilaboðin.

4. Biðlarinn sendir skilaboð til þjónsins, dulkóðuð með nýafkóðuðu skilaboðunum sem og lotulyklinum.

5. Þjónninn framkvæmir sömu dulkóðunina og ber saman við gildið frá biðlaranum, ef gildin stemma sannar það að biðlarinn er með einkalykilinn og er því auðkenndur.
