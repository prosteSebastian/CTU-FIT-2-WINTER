# CTU-FIT-2-WINTER
## Základní příkazy pro používání repozitáře.
### Přidání souboru a jeho následné poslání
* Naklonovat si repo: ```git clone git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git```
* pridani souboru: ```git add <soubor>``` a nasledně ```git commit -m "prefix dle predmetu: <message>"```
*Ukázkový případ:
```
git clone git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git
cd CTU-FIT-2-WINTER/MA2
git add poznamky.pdf
git commit -m "MA2: Notes from first 6 chapters."
git push
```
### Aktualizování forku
* Pokud to u vás vypadá aktuálně takto:
```
git remote -v
origin	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (fetch)
origin	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (push)
```
* Tak použijte toto:
```
git remote add upstream origin git@github.com:prosteSebastian/CTU-FIT-1_SUMMER.git
git remote -v
origin	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (fetch)
origin	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (push)
upstream	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (fetch)
upstream	git@github.com:prosteSebastian/CTU-FIT-2-WINTER.git (push)
```
* Pokud tam již něco budete mít, tak jen použijte místo  ```add``` ```remove```.

* Pro zjištění změn: `git fetch upstream`
* A jejich následná aktualizace.
```
git merge upstream/main
