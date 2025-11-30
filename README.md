# Műszakbeosztás-ellenőrző

## Név
Szilárdi Roland (VFOFMH)

## Rövid leírás

Egyszerű grafikus Python alkalmazás, amellyel a műszakbeosztást lehet rögzíteni és ellenőrizni.  
A felhasználó megadhat egy dátumot és kiválaszthatja a műszak típusát (Reggel, Délután, Éjszaka, Szabadnap).  
A program listázza a felvitt műszakokat, kiszámolja az összes ledolgozott órát az aktuális hónapra, és statisztikát készít a műszakok számáról.

## Fájlok

- `main.py`  
  - A program belépési pontja
  - Létrehozza a `tkinter` fő ablakot (`root`) és az alkalmazás objektumot (`SzRMuszakApp`).

- `logic_SzR.py`  
  - Saját modul (SzR monogrammal).  
  - Tartalmazza a `SzRMuszak` és `SzRMuszakNaplo` osztályokat.  
  - A `SzRMuszakNaplo` tárolja a műszakbejegyzéseket, és metódusai kiszámolják a havi ledolgozott órákat és a statisztikát
  - Saját függvények: `szr_datum_strbol`, `szr_datum_formaz`, `szr_honap_eleje`

- `gui_SzR.py`  
  - A grafikus felület (GUI) megvalósítása `tkinter`-rel
  - `SzRMuszakApp` osztály: kezeli az ablakot, a vezérlőelemeket és az eseményeket (gombnyomások)

## Használt modulok

- `tkinter` – grafikus felület és eseménykezelés (gombok, listbox, label-ek).  
- `datetime` – dátumok kezelése (string → dátum, mai nap lekérdezése, formázás).  
- Saját modul: `logic_SzR.py` (SzR monogrammal).

## Futatás

```bash
python main.py
