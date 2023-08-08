# Webes_ToDo_App
A Netakadémia * "Az első webes C# projektem: TO-DO alkalmazás készítése (classic) " -ból származik minden
## A tanfolyam Privát, csak megosztott emberek számára elérhető.

## 01_Bevezetés és template kialakítása 1

* a .gitignore állomány az abban segit, hogy ne minden állományt, amit generálunk szoftverfejlesztés közben, ne minden állomány kerüljön fel ebbe a github kódtárba, mert nincs semmi értelme, hogy felkerüljön.
* például: a Visual Studio készít olyan állományokat, amely a felhasználónak a paramétereit tárolja, hol vannak az ablakok, mi volt utoljára megnyitva, ezeket nem kell a kódtárba betenni, hiszen ha valaki másholvá lehuzza másik gépen, akkor egyáltalán nem kell, hogy a saját beállitásaim esetleg a többi fejlesztő számára is ugyanolyan beállitások legyenek. Sőt ha ő át állit valamit, akkor az ő beállitásai lejöjenek hozzám, összekeverednek ezek a dolgok semmi értelme.
* Tehát vannak olyan állományok amik a fejlesztőkhöz tartoznak és érdemes őket kivenni.
* szerencsére nem kell már a nulláról beállitani a github-on ezt az állomány, amiben fel van sorolva azok a szábályok, ami szerint kell kihagyni egyes állományokat a kódtárból.
* ilyen pl. a bináris állományok, hogyha leforditjuk a projektünket, akkor nem kell a végeredményt berakni, hiszen itt csak a fejlesztési kódok vannak.
* nyilt forráskódú fejlesztésekhez van kitalálva ez a github, ezért nem tudunk license-t adni, ez egy tanfolyam, szabadon fel lehet használni a tanfolyam hallgatóinak a kódokat, ezért nem tudunk license-t megadni, legyen The Unlicense-s.
* Hozzuk létre a kódtárat. Create repository.

* a kódtár elkészült, szeretném ha én gépemen meglegyen ennek a másolata.
* ez az egész dolog röviden úgy megy, hogy van a server és van az én saját gépem, és majd az én saját géepem is ez a kódtár majd szépen ott lesz. Ezen beül én dolgozgatok.
* és ha én majd elkészülök valamivel, akkor én ezt felküldöm a szerverre és ennyi az egész workflow. Az egész fejlesztési folyamat az ennyi.
* ha szeretnénk a saját gépünkön is látni ezeket a kódokat, akkor van egy a létrehozott repository-n belül egy Clone or download tész, és ott található egy url-cím.
* amit majd később felhasználva tudjuk összekötni a gépünkkel a kódtárat.
* nyissuk meg a Visual Studio-nkat, és megmutatom, hogyan tudjuk ezt ezzek a kódszerkesztővel lemásolni.
* amikor megnyilt a Visual Studio-nk, ha nem látszik akkor felül a View -> Team Explorer-ben tudunk kódtárat másolni a saját gépünkre.
* muszáj megismerkedni a GitHub-bal, ha valaki fejlesztő akar lenni
* nyissuk meg a Team Explorer-t, ha megtaláltuk, kattintsunk a kis házikó ikonra
* utána a Git Changes gombra, majd megjelenik a Clone Repository... gomb, erre van szükségünk
* ha rá kattintottunk és megjelent egy új ablak, a Repository location mezőjébe másoljuk be a linket
* a Path-nél a számitógépen lévő helyet kell kiválasztanunk a repository-nk számára, itt tároljuk majd lokálisan a github-on lévő fájlokat
* egy üres mappát válasszunk ki célmappának
* majd kattintsunk a Clone-ra
* ezzel leklónoztuk ezt a könyvtárat a saját gépünkre
*
* két fajta fejlesztéssel fogunk megismerkedni alapvetően, és ez a két fejlesztés mód, ez meglehetősen sokféle módszertant magába foglal
* az egyik fejlesztési mód esetén, a felhasználó ül a gép előtt, amin fút egy alkalmazás és ez az alkalmazás egy desktop számítógépen fút, tipikusan eu az XAML ez egy ilyen fejlesztési környezet, hogy a számítógépen lévő alkalmazást fejleszük (Xamarin nevű Microsoft-os fejlesztési környezet XAML fejlesztési környezetet ad mobiltelefonos fejlesztésekre. Az XAML-es fejlesztés ez egy az egyben nem használható mobiltelefonokra, azonban a Xamarin-os környezettel, maga az XAML-s tudás az átemelhető, meg kell hozzá temészetesen tanulni a telefonos környezet sajátoságait, de alapvetően a maga az XAML-es fejlesztés az arra szolgál, hogy van egy fizikai eszközünk és a fizikai eszközön egy alkalmazást szeretnék futtatni, amin ablakok vannak, gombok, listák vannak ilyesmik. Tehát ez erre mondhatjuk at, hogy ez egy hagyomásnyos desktop alkamazás fejlesztés).
* a mobil is ide tudjuk venni, hiszen a mobilalkamazások is valami ilyesmit csinálnak, egy alkalmazást telepitünk ami ablakokat nyit, szöveget ir az ablakokba, gombokat ad és nem egérrel, hanem az ujjunkkal ugyanazt tudjuk csinálni.
                                      
                                    
                                                                ┌──────────────────────────┐
                                                                │                          │
                                                                │   Desktop számitógép     │
                                      ┌───────────────┐         │                          │
                                      │               │         │                          │
                                      │  Felhasználó  │         │  ┌───────────────────┐   │
                                      │               │         │  │                   │   │
                                      └───────────────┘         │  │    Alkalmazás     │   │
                                                                │  │                   │   │
                                                                │  └───────────────────┘   │
                                                                │                          │
                                                                └──────────────────────────┘

* ez az alfája és imegája minden fejlesztésnek, nem nagyon lehet elkerülni.
* a mi esetünkben kicsit keiegészül ez a kép, ugyanis az alakalmazásunkat úgy hivják, hogy böngésző
* és az alakalmazásfejlesztésünk nem a desktop számítógépről szól,
* hanem mi egy olyan alkalmazást fogunk készíteni, amit egy böngésző segitségével fogunk tudni használni.
* a webes fejlesztés amire mi most kisérletet teszünk és olyan megoldás
* ami hálózati kapcsolatot használ a kliens gép és a, kliens gépen futó alkalmazás böngésző között
* és a mi számítógépünk ami a server számítógép az úgy dolgozik, hogy az alkalmazásunk a böngészőben, mi elinditunk mindenféle kéréseket a server felé és a server fog nekünk válaszolni, méghozzá a serveren futó alkalmazásunk.  
* ez már így elsőre is láthatjuk, hogy ez egy összetettebb feladat, minthogy itt a felhasználó elé kirakjunk egy alkalmazást és majd azt a gombnyomogatást lekezeljük,
* mert itt azon kivül, hogy szeretnénk valamit megjeleniteni és a felhasználó számára gombokat, emg mindenféle dolgokat elé tenni
* azon kivül még van itt egy hálózati forgalom amit meg kell oldanunk
* és azért is jó ezzel folytatni az alkalmazás fejlesztésünket, mert hálózati kapcsolat a desktop számítógépen is lehet 
* még két fogalmat muszáj bevezetni, az egyik a HTML, a HTML egy jelölőnyelv ez a jelölőnyelv azt jelenti, hogy egy közös családból leszármazó dologról van szó ez a XML családjához tartozik, erre egy példa az XAML ez is egy jelölőnyelv, a lényeg, hogy tagek vagy önmagukban jelentenek valamit vagy nyitnak zárnak valamit és kettőjük közé kell valamit irni. Ezt majd gyakorlatban megfogjuk nézni.
* a másik fogalom amit használni fogunk azt pedig a HTTP, ez pedig az a protokolnak hivott dolog, amivel elérjük, hogy a böngésző és a server számítógép tudjon egymással beszélni. A protokol az ilyen kérdéseket és válaszokat tartalmaz, leírja, hogy milyen kérdéseket lehet a server felé küldeni és milyen válaszokat tudd a server adni, ahhoz hogy ezen a HTTP-n belül tudjon maradni, erről is lesz szó.
* a server alkalmazásunk egy úgynevezett MVC környzetben fejlődik,
* ami a lényeg, hogy egy olyan alkalmazást fogunk fejleszteni a webszerveren, ami nem a webszervern fog a felhasználókkal találkozni, hanem egy köztes alkalmazással ez a böngésző alkalmazás és a böngészőből kérdések fogok megfogalmazni a webszerver felé, a szerver válaszolni fog a válassza az HTTP-n keresztül fog megérkezni és általában HTML formátumban jön, és ezeket a HTMl formátumu válaszokat a böngészőnk értelmezi és megjeleniti.
                                                                          +--------------------------+
                                                                          |  Szerver számítógép      |
                               +------------------------+                 |                          |
                               |   Desktop számítógép   |                 |                          |
                               |    Mobil eszköz        |    Hálózati     |                          |
                               |                        |    kapcsolat    | +----------------------+ |
+---------------+              |                        |                 | |                      | |
|               |              |    +-------------+     +---------------> | |  Szerver alkalmazás  | |
|  Felhasználó  |              |    | Alkalmazás  |     |                 | |  (WebSzerveren futó  | |
|               |              |    | (Böngésző)  |     | <---------------+ |  app)                | |
|               |              |    +-------------+     |                 | |                      | |
+---------------+              |                        |        ^        | +----------------------+ |
                               +------------------------+        |        |                          |
                                                                 |        |              ^           |
                                            ^                    |        |              |           |
                                            |                    |        |              |           |
                                            |                    |        |              |           |
                                            |                    |        +--------------------------+
                                            |                    |                       |
                                            +                    +                       +
                                          HTML                 HTTP                     MVC



                                               Webes Alkalmazásfejlesztés

* Röviden egy ilyen alkalmazás a cél. Nem azt fogjuk programozni, amit a felhasználó a szerveren lát, az alkalmazásunkban. Hanem az alkalmazásunk gyárt egy olyan dolgot, amit a hálózaton átküldve majd a böngésző fog megjeleniteni
* épitünk egy nagyon egysszerű alkalmazást és átfogjuk nézni, hogy ezek a kérés válaszok, ezek hogy néznek ki, hogyan épül fel egy ilyen alkalmazás, mire kell figyelni az alkalmazás fejlesztése közben.
* megfogunk ismerkedni egy fontos környezettel ez a webes alkalmazásfejlesztés.
* commit-nak hivjuk azokat a csomagokat, amikor elkészültünk valami kóddal, azt becsomagoljuk és azt felküldjük erre a kódtárra. Azért, hogy a munkánkat később könnyebb legyen visszanézni, azért ezt a kódtárat, mi egy kicsit szervezni is tudjuk, ilyen például a GitHub-on az Issue kártyák használata, az issue kártyák azok arra vonatkoznak, hogy ha az eggyes problémköröket azokat ha megnevezzük, akko a kis commit csomagjainkat, ami az eggyes munkarész, hozzá tudjuk kapcsolni ezekhez a kártyákhoz.
* például menjünk a GitHub-ra, a kódtárba amit létrehoztunk Webes_ToDo_App-ba New Issue gomra katt, a Title-hez beirjuk a "problémakört", pl. bevezetés, alapbeállitások és dokumentáció, és keressük meg a Submit New Issue gombot, ezzel ha rákattintunk létrehoztuk ezt az Issue kártyát.
* és a visual studio-ban az eddig módosításainkat küldjük fel úgy, hogy felküldjük a kódtárba a webszerverre
* ehhez menjünk a Visual Studio-ba, Team Explorer -> Git Changes itt fogja megmutatni a Git-nek a kliensrésze, hogy mi változott az én munkakörnyvtáramban és ezt a változást egy megjegyzéssel fel tudom küldeni
* amikor létrehoztuk a kártyát akkor valószinüleg a #1-es sorszámot kapta, ha az első kártyánkat hoztuk létre
* az Enter message <Required>-hez irjuk meg ezt a sorszámot
* #1: alapok lefektetése 1
* a Commit All-al tudom az összes módosítást feltölteni és ezt most a sajátgépemen csomagolta be ezt az egészet amit módosítottam, és ez addig nem fog a szerverhez kimenni, amíg én azt nem mondom, hogy ezeket töltse fel,
* tehát két lépésből áll az első a commit-olás (Commit All) és a felküldés a szerverre a második lépés (Sync) és (Fetch), ezzel feltöltöm a szerverre. 

### 01 Összefoglaló

## 02_Bevezetés és template kialakítása 2



















