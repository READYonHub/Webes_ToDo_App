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
### 01 Összefoglaló
- 
