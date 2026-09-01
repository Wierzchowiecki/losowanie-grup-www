# 🎲 Losowanie Grup

Aplikacja internetowa napisana w Pythonie, służąca do automatycznego i losowego podziału uczestników na **4 grupy**.

🌐 **Działająca aplikacja:**
https://losowanie-grup-www.onrender.com/

👉 **[OTWÓRZ APLIKACJĘ – LOSOWANIE GRUP](https://losowanie-grup-www.onrender.com/)**

---

## 📖 O projekcie

**Losowanie Grup** to aplikacja internetowa stworzona w Pythonie przy użyciu frameworka Flask.

Jej zadaniem jest automatyczny podział uczestników na **4 grupy** zgodnie z określonymi zasadami.

Program uwzględnia dwa rodzaje uczestników:

* 👤 osoby pojedyncze,
* 💑 małżeństwa.

Małżeństwa podczas losowania **zawsze pozostają razem** i nigdy nie są rozdzielane pomiędzy różne grupy.

---

# 🎯 Zasady tworzenia grup

Aplikacja została zaprojektowana tak, aby grupy były możliwie równomierne.

Przy obecnej liczbie uczestników:

* **9 małżeństw**
* **11 singli**
* łącznie **29 osób**

tworzone są **4 grupy**.

### 💑 Małżeństwa

Każda z czterech grup otrzymuje **co najmniej 2 małżeństwa**.

Przy 9 małżeństwach podział wygląda:

* jedna grupa – 3 małżeństwa,
* trzy grupy – po 2 małżeństwa.

O tym, która grupa otrzyma dodatkowe małżeństwo, decyduje losowanie.

### 👤 Single

Do podziału dostępnych jest 11 singli.

Dlatego przy czterech grupach podział wygląda:

* trzy grupy – po 3 singli,
* jedna grupa – 2 singli.

O tym, która grupa otrzyma 2 singli, również decyduje losowanie.

Gdy w przyszłości liczba singli wzrośnie do minimum 12, możliwe będzie zapewnienie **co najmniej 3 singli w każdej grupie**.

---

# 🎲 Jak działa losowanie?

Po kliknięciu przycisku:

## 🎲 Losuj Grupy

program:

1. pobiera listę wszystkich uczestników,
2. rozpoznaje singli i małżeństwa,
3. losowo miesza uczestników,
4. tworzy 4 grupy,
5. rozdziela małżeństwa pomiędzy grupy,
6. zapewnia minimum 2 małżeństwa w każdej grupie,
7. rozdziela singli możliwie równomiernie,
8. pilnuje, aby małżeństwa pozostały razem,
9. wyświetla gotowe grupy na stronie.

Każde kolejne kliknięcie **Losuj ponownie** tworzy nową konfigurację uczestników.

---

# 🌐 Korzystanie z aplikacji

Aplikacja dostępna jest pod adresem:

👉 **https://losowanie-grup-www.onrender.com/**

Nie trzeba instalować:

* Pythona,
* PyCharma,
* bibliotek,
* ani żadnego dodatkowego programu.

Wystarczy przeglądarka internetowa.

Aplikacja działa zarówno na komputerze, jak i na telefonie.

---

# 📊 Eksport do Excela

Po wykonaniu losowania można kliknąć:

## 📥 Pobierz do Excela

Aplikacja automatycznie tworzy plik:

`wylosowane_grupy.xlsx`

Każda grupa znajduje się w osobnej kolumnie:

| GRUPA 1   | GRUPA 2   | GRUPA 3   | GRUPA 4   |
| --------- | --------- | --------- | --------- |
| uczestnik | uczestnik | uczestnik | uczestnik |
| uczestnik | uczestnik | uczestnik | uczestnik |
| uczestnik | uczestnik | uczestnik | uczestnik |

Plik Excel posiada:

* kolorowe nagłówki,
* osobną kolumnę dla każdej grupy,
* obramowania komórek,
* odpowiednią szerokość kolumn,
* czytelne formatowanie,
* obsługę polskich znaków.

Do tworzenia plików `.xlsx` wykorzystywana jest biblioteka **openpyxl**.

---

# 🛠 Technologie

Projekt wykorzystuje:

### Backend

* Python
* Flask
* Gunicorn

### Frontend

* HTML
* CSS
* Jinja2

### Excel

* openpyxl

### Kod źródłowy

* Git
* GitHub

### Hosting

* Render

---

# 📁 Struktura projektu

```text id="vrmfxq"
losowanie-grup-www/
│
├── app.py
├── requirements.txt
│
└── templates/
    └── index.html
```

### `app.py`

Główny plik aplikacji.

Odpowiada za:

* listę uczestników,
* podział na singli i małżeństwa,
* algorytm losowania,
* tworzenie 4 grup,
* obsługę Flask,
* zapamiętywanie aktualnego losowania,
* generowanie pliku Excel.

### `templates/index.html`

Odpowiada za wygląd aplikacji.

Zawiera:

* ekran startowy,
* przycisk **Losuj Grupy**,
* prezentację czterech grup,
* przycisk **Losuj ponownie**,
* przycisk **Pobierz do Excela**.

### `requirements.txt`

Lista bibliotek potrzebnych do działania aplikacji:

```text id="okyp0f"
Flask
gunicorn
openpyxl
```

---

# 💻 Uruchomienie lokalne

Instalacja wymaganych bibliotek:

```bash id="j8c4nz"
pip install -r requirements.txt
```

Uruchomienie aplikacji:

```bash id="0ywk6j"
python app.py
```

Aplikacja będzie dostępna lokalnie pod adresem:

`http://127.0.0.1:5000`

---

# ☁️ Hosting

Aplikacja została wdrożona jako Web Service na platformie Render.

### Build Command

```text id="d2g9ml"
pip install -r requirements.txt
```

### Start Command

```text id="n15p7x"
gunicorn app:app
```

---

# 🔮 Możliwości dalszego rozwoju

Aplikację można w przyszłości rozbudować o:

* dodawanie uczestników z poziomu strony,
* usuwanie uczestników,
* osobne zarządzanie singlami i małżeństwami,
* wybór liczby grup,
* automatyczne sprawdzanie minimalnej liczby singli i małżeństw,
* historię wcześniejszych losowań,
* panel administratora,
* zabezpieczenie strony hasłem,
* edycję uczestników bez zmieniania kodu.

---

# 🚀 Gotowa aplikacja

## 🎲 Losowanie Grup

👉 **[URUCHOM APLIKACJĘ](https://losowanie-grup-www.onrender.com/)**

🌐 https://losowanie-grup-www.onrender.com/

Wystarczy wejść na stronę i kliknąć:

**🎲 Losuj Grupy**
