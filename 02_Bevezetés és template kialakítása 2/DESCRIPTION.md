#2: 02_Bevezetés és template kialakítása 2
* a következő lépésünk az az lesz,, hogy csinálunk egy alkalmazást
* szeretném felhivni a figyelmeteket egy tanfolyamra, vagyis többre
## ajánlott tanfolyamok
#### LENYÜGÖZŐ WEBLAPOK KÉSZÍTÉSE tanfolyam
* egy HTMl tanfolyam ezzel foglalkozni kell, gyakorolni, mert kell hozzá idő amíg az ember megszokja
#### HÁLÓZATI ALAPISMERETEK tanfolyam
* mert a HTTP-vel ajánlott megismerkednünk, mert egy webesprogramozónak kötelező megismerkednie vele
## az első webes alkalmazásunk létrehozása
* tudni kell hogy különböző keretrendszerek vannak a világon, ezek a keretrendszerek különböző módon, de ugyanugy ugyanarra a célra épültek a webes alkalmazás fejlesztés világában, viszont
* maga a webes alkalmazásfejlesztés azt akármennyire megpróbáljuk körbe bástyázni azért ő egy meglehetősen bonyolult dolog
* ezt úgy értem, hogy amíg egy desktop alkalmazásunk van és nincs hátsó hálózati kapcsolat, addig eldöntöm, hogy hogyan reagálok az egyes gombokra
* abban a pillanatban, hogy több számítógépen vannak az adatok, abban a pillanatban nekem már úgy kell szerveznem a munkámat, hogy rendben, most a felhasznló rányomott egy gombra, nekem most kérdeznem kell valamit a szervertől, a szervernek válaszlnia kell számomra, és ezt az egész dolgot nekem valami értelmes módon kell megszerevezni, mert nekem majd megkell kapni azt a választ és megkell mutatnom és nem ugyanabban a függvényben vagyok
* tehát programozás technikailag azt hogy egy másik szerver válaszát megvárom és azt nekem fel kell dolgoznom az azt jelenti, hogy két szálon fút a történet
* az egyik szál a böngésző
* a másik szál pedig ami majd vissza jön az adatokkal, amit majd meg kell nekem mutatnom
* és ez technikai szempontból jelentős megváltztatja a programozónak a nézőpontját
* még van egy git tanfolyam is amit érdemes megnézni
#### FEDEZÜK FEL A GITET  EZT AJÁNLOM MÉG 
* EZ A TANFOLYAM MÉG HASZNOS LEHET HOGY ISMERJÜK MEG JOBBAN KICSIT Az szközeink eszközeit bőverbbrn, hatalmas verseny előnyt tudd jelenteni ezek a dolgok folyék használata a munkánk során vagy akár még egy állásinterjún is
* a bonyolultságra visszatérrve, mindjárt létrehozzunk egy webes projektet és ez a webes projekt, ha kézzel kéne létrehoznunk,a kkkor bizony jó sok munkát venne igénybe
* Mivel a környezet és a fejlesztési munkafolyamat az ilyen  típusu fejlesztéseknél összetett, így nem kézzel hozzunk létre hanem a VS segitségével.
* hozzuk létre
* File -> New Project -> ASP .NET Web Application (.NET Framework)
* adjunk neki egy nevet a Name: -nél, ugyanez lesz automatikusan a Solution Name is
* egy olyan mappába "browzoljuk" (Browse), ami üres
* és ezzel a template-l menjünk tovább
* katt az OK-ra
* ezután kapunk egy varázslót, ez sokféle alkalmazástipust felajánl ezekből nekünk az MVC-re van szükségünk
* válasszuk ki az MVC-t és Create
* most létrehozzan nekünk ezt a projektet , illetve azt tudni kell , hogy ezekből a projektekből egy saját megoldást tudunk gyártani, ez azt jelenti, hogy a sját megoldásunk az több projektet tartalmaz most itt nekünk a ToDOApp az egy projekt lesz
* és ha megnézzük, hogy a Solution Explorer-ben mennyi dolgott berakott, azt hiszem ha ezt átnézzük, akkor mindenki érzi hogy ezt/ezeket itt kézzel létehozni a világn semmi értelme nincsen.
* ez be van építve a Visual Studioba és nekünk ezt madj szépen létrehozza azt a webes alkalmazást amivel  majd webes környezet tudunk majd teremteni és böngésző kéréseket tudunk majd kiszolgálni
* 
