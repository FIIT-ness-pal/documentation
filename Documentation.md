# Zadanie 2 (Míľnik 1) - Jakub Abrahoim, Adam Blahovič

# Obsah

---

# Návrh databázy

![Navrh DB MTAA-v02.drawio.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Navrh_DB_MTAA-v02.drawio.png)

# Wireframy

## Registrácia

![Registration.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Registration.png)

## Prihlásenie

![Login.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Login.png)

## Domovská stránka

![Homepage.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Homepage.png)

## Profil

![Profil.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Profil.png)

## Vyhľadávanie

![Vyhľadávanie.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Vyhadvanie.png)

## Vytvorenie jedla

![Vytvoriť jedlo (1).png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Vytvori_jedlo_(1).png)

## Detail jedla

![Detaily jedla.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Detaily_jedla.png)

## Detail potraviny

![Detaily potraviny.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Detaily_potraviny.png)

## Vytvoriť potravinu

![Vytvoriť potravinu.png](Zadanie%202%20(Mi%CC%81l%CC%8Cnik%201)%20-%20Jakub%20Abrahoim,%20Adam%20Blah%20a3495ea0271b4acba13e9e1a0077f78f/Vytvori_potravinu.png)

# Testy

## Frontend

### Kladné

1. **Úspešné prihlásenie**
    
    
    | Vstupné podmienky: | Používateľ má otvorenú aplikáciu na stránke s prihlásením a je pripojený na Internet |
    | --- | --- |
    | Výstupné podmienky: | Používateľ sa presunie na domovskú stránku aplikácie |
    | Postup: | 1. Používateľ klikne na tlačidlo Prihlásiť sa 
    2. Zobrazí sa prihlasovací formulár
    3. Používateľ vyplní pole pre e-mailovú adresu
    4. Používateľ vyplní pole pre heslo
    5. Používateľ klikne na tlačidlo Prihlásiť sa |
    | Výsledok: | PASS |
2. **Vytvorenie receptu**
    
    
    | Vstupné podmienky | Používateľ je prihlásený a nachádza sa na domovskej stránke. Aplikácia je pripojená na Internet. |
    | --- | --- |
    | Výstupné podmienky | V aplikácii pribudne nové jedlo, ktoré sa uloží do databázy. |
    | Postup | 1. Používateľ stlačí tlačidlo Vytvoriť a presunie sa na obrazovku pre vytvorenie
    2. Používateľ zvoli možnosť Vytvoriť receptu kliknutím na príslušné tlačidlo
    3. Zobrazí sa obrazovka na vytvorenie receptu, kde používateľ vyplní názov receptu a pridá popis
    4. Používateľ klikne na tlačidlo Pridať surovinu
    5. Zobrazí sa obrazovka s vyhľadávaním surovín
    6. Používateľ vyhľadá požadovanú surovinu, zadá množstvo a klikne na tlačidlo Pridať
    7. Opäť sa zobrazí obrazovka na vytvorenie receptu
    8. Používateľ opakuje kroky 4. až 7., kým nepridá všetky suroviny.
    9. Používateľ klikne na tlačidlo Uložiť |
    | Výsledok | PASS |
3. **Log jedla**
    
    
    | Vstupné podmienky | Používateľ je prihlásený a nachádza sa na domovskej stránke. Aplikácia je pripojená na Internet. |
    | --- | --- |
    | Výstupné podmienky | Do používateľovho logu pribudne nové jedlo a prepočíta sa príjem jeho kalórií za daný deň |
    | Postup | 1. Používateľ stlačí tlačidlo Pridať a presunie sa na obrazovku pre Pridanie
    2. Používateľ klikne na tlačidlo Pridať jedlo
    3. Zobrazí sa obrazovka s vyhľadávaním
    4. Používateľ napíše do vyhľadávača názov jedla
    5. Používateľ vyberie jedlo, vpíše množstvo a klikne na tlačidlo Pridať
    6. Zobrazí sa domovská stránka |
    | Výsledok | PASS |

### Záporné

1. **Neúspešná registrácia**
    
    
    | Vstupné podmienky | Používateľ má otvorenú aplikáciu na stránke s prihlásením a je pripojený na Internet |
    | --- | --- |
    | Výstupné podmienky | Používateľovi sa nepodarí zaregistrovať a zostane na obrazovke s registráciou |
    | Postup | 1. Používateľ klikne na tlačidlo registrovať sa a zobrazí sa obrazovka s registráciou
    2. Používateľ vyplní polia pre email, meno a heslo
    3. Používateľ do poľa pre kontrolu hesla zadá nesprávne heslo
    4. Používateľ klikne na tlačidlo Registrovať sa
    5. Zobrazí sa červený text “Heslá sa nezhodujú” |
    | Výsledok | FAIL |
2. **Neúspešné vyhľadávanie**
    
    
    | Vstupné podmienky | Používateľ sa nachádza na stránke pre vytvorenie receptu a aplikácia je pripojená na Internet |
    | --- | --- |
    | Výstupné podmienky | Používateľovi sa nepodarí vyhľadať surovinu a zostane na obrazovke s vyhľadávaním |
    | Postup | 1. Používateľ klikne na tlačidlo Pridať surovinu
    2. Zobrazí sa obrazovka vyhľadávania
    3. Používateľ do poľa na vyhľadávanie zadá surovinu, ktorá sa nenachádza v databáze
    4. Na mieste, kde sa bežne zobrazujú výsledky vyhľadávania, sa vypíše “Nenašla sa žiadna zhoda” |
    | Výsledok | FAIL |
    

---

---

## Backend

### Kladné

1. **Prihlásenie do aplikácie**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | Server verifikoval používateľa a vrátil jeho dáta |
    | Postup | 1. Na server príde požiadavka POST s prihlasovacími údajmi
    2. Server autentifikuje používateľa
    3. Server vráti status kód 200
    4. Na server prídu 2 požiadavky GET s dopytom na používateľov príjem a jeho históriu
    5. Server odpovie s danými údajmi |
    | Výsledok | PASS |
2. **Pridanie jedla do logu**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | Do databázy sa pridá záznam s jedlom |
    | Postup | 1. Na server príde požiadavka GET s názvom jedla
    2. Server odpovie zoznamom jedál z databázy, ktoré sa zhodujú s daným názvom
    3. Na server príde požiadavka POST s ID jedla
    4. Do databázy sa uloží nový záznam
    5. Server vráti status kód 200 |
    | Výsledok | PASS |

1. **Upravenie používateľovej hmotnosti**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | V databáze sa zmení záznam s váhou |
    | Postup | 1: Na server príde požiadavka GET na používateľove údaje
    2. Server odpovie s danými údajmi
    3. Na server príde požiadavka PUT s upravenými údajmi
    4: Do databázy sa vloží upravená hodnota
    5. Server odpovie kódom 200 |
    | Výsledok | PASS |

### Záporné

1. **Neúspešná registrácia - email už existuje**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | Server vráti chybový status kód |
    | Postup | 1. Na server príde požiadavka POST s registračnými údajmi
    2. Server skontroluje, či sa v databáze nachádza používateľov e-mail
    3. Server vráti kód 409 (Conflict) |
    | Výsledok | FAIL |
2. **Neúspešné prihlásenie - nesprávne heslo**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |  |
    | --- | --- | --- |
    | Výstupné podmienky | Server vráti chybový status kód |  |
    | Postup | 1. Na server príde požiadavka POST s prihlasovacími údajmi
    2. Server skontroluje, či prijaté údaje súhlasia s údajmi v databáze
    3. Server vráti kód 401 (Unauthorized) |  |
    | Výsledok | FAIL |  |
3. **Prázdne pole pri úprave receptu**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | Server vráti chybový status kód |
    | Postup | 1. Na server príde požiadavka GET s ID receptu
    2. Server vráti údaje o danom recepte a kód 200 (OK)
    3. Na server príde požiadavka PUT s ID receptu a dátami, ktoré sa majú zmeniť. Jedno z polí je prázdne
    4. Server vráti kód 400 (Bad Request) a údaje v databáze sa nezmenia |
    | Výsledok | FAIL |
4. **Nesprávny formát pri úprave používateľských údajov**
    
    
    | Vstupné podmienky | Server je spustený a pripojený na databázu |
    | --- | --- |
    | Výstupné podmienky | Server vráti chybový status kód |
    | Postup | 1. Na server príde požiadavka GET s ID používateľa
    2. Server vráti údaje o používateľovi a kód 200 (OK)
    3. Na server príde požiadavka PUT s novými údajmi o používateľovi, parameter váha nie je číslo
    4. Server vráti kód 400 (Bad Request) a údaje v databáze sa nezmenia |
    | Výsledok | FAIL |
    

# Rest API

## Vyhľadať jedlo - GET

### Request

```
[GET endpoint] /meals
[Príklad] /meals?name=spagety
```

### Parameters

- **name** (string) - text, ktorý bol zadaný do vyhľadávacieho poľa

### Response

```json
{
    "meals": [
        { 
            "id": 1, 
            "name": "spagety",
            "calories": 486,
            "carbs": 80,
            "protein": 20,
            "fat": 10
        },
        {
            "id": 44, 
            "name": "spagety alfredo",
            "calories": 486,
            "carbs": 80,
            "protein": 20,
            "fat": 10
        }
    ]
}
```

---

## Vyhľadať potravinu - GET

### Request

```
[GET endpoint] /foods
[Príklad] /foods?name=flakes
```

### Parameters

- **name** (string) - text, ktorý bol zadaný do vyhľadávacieho poľa

### Response

```json
{
    "foods": [
        { 
            "id": 1, 
            "name": "Frosted flakes",
						"brand": "Kellogs",
            "calories": 486,
            "carbohydrates": 80,
            "protein": 20,
            "fat": 10
        },
        {
            "id": 44, 
            "name": "Corn flakes",
						"brand": "Kellogs"
            "calories": 486,
            "carbohydrates": 80,
            "protein": 20,
            "fat": 10
        }
    ]
}
```

---

## Zobraziť log - GET

### Request

```
[GET endpoint] /log
[Príklad] /log?userId=1&date=2022-03-10
```

### Parameters

- **userId** (integer) - ID používateľa
- **date** (timestamp) - dátum

### Response

```json
{
		"totalCalories": 650,
		"totalProtein": 50,
		"totalFat": 30,
		"totalCarbs": 50,
    "logs": [
        {  
            "name": "jahodový jogurt",
						"amount": 150,
						"time": "7:30",
            "calories": 150
        },
        {
            "mealName": "špagety",
						"amount": 300,
						"time": "12:00",
            "calories": 300
        },
				{
            "mealName": "šalát",
						"amount": 200,
						"time": "16:30",
            "calories": 200
        }
    ]
}
```

---

## Zobraziť detaily jedla - GET

### Request

```
[GET endpoint] /meal
[Príklad] /meal?id=31
```

### Parameters

- **id** (integer) - ID jedla

### Response

```json
{
	"id": 31,
	"name": "Špagety",
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10,
	"description": "Moje skvelé špagety",
	"amount": 300,
	"ingredients": [
		{
			"id": 1,
			"name": "cestoviny",
			"brand": "K-classic",
			"amount": 20
		},
		{
			"id": 2,
			"name": "morca-della",
			"brand": "Hame",
			"amount": 20
		}
	]
}
```

---

## Zobraziť detaily suroviny - GET

### Request

```
[GET endpoint] /food
[Príklad] /food?id=2
```

### Parameters

- **id** (integer) - ID potraviny

### Response

```json
{
    "id": 2,
		"name": "morca-della",
		"brand": "Hame",
		"amount": 20,
		"calories": 486,
	  "carbs": 80,
	  "protein": 20,
	  "fat": 10,
}
```

---

## Zobraziť používateľove informácie - GET

### Request

```
[GET endpoint] /user
[Príklad] /user?id=3
```

### Parameters

- **id** (integer) - ID používateľa

### Response

```json
{
	"firsName": "Peter",
	"lastName": "Zdravý",
	"email": "peter.zdravy@pokec.sk",
	"weight": 100,
	"height": 185,
	"birthday": 1995-10-5,
	"caloriesGoal": 2200,
	"photo": "https://petkovafotka.com/petko"
}
```

---

## Pridať jedlo - POST

### Request

```
[POST endpoint] /meal
```

### Request body

```json
{
	"name": "Ivkove špagety",
	"description": "Moje mňam mňam špagetky",
	"userId": 3,
	"amount": 20,
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10,
	"isPublic": true,
	"ingredients": [
		{
			"id": 4,
			"amount": 20,
		},
		{
			"id": 5,
			"amount": 10,
		}
	]
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Pridať potravinu - POST

### Request

```
[POST endpoint] /food
```

### Request body

```json
{
	"name": "Jablko",
	"description": "Jablko červené",
	"userId": 3,
	"brand": "Veselé jablko zo Žitného ostrova",
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10,
	"isPublic": true,
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Pridať jedlo do logu - POST

### Request

```
[POST endpoint] /log
```

### Request body

```json
{
	"userId": 3,
	"name": "Pizza Hawaii",
	"date": 2022-03-10 15:30,
	"amount": 400,
	"calories": 800,
  "carbs": 80,
  "protein": 20,
  "fat": 300
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Prihlásiť sa - POST

### Request

```
[POST endpoint] /login
```

### Request body

```json
{
	"email": "marek.parek@oharek.com",
	"password": "123styri"
}
```

### Responses

```json
{
	"status": 200,
	"message": "OK"
}

{
	"status": 401,
	"message": "Unauthorized"
}
```

---

## Registrovať - POST

### Request

```
[POST endpoint] /register
```

### Request body

```json
{
	"email": "marek.parek@oharek.com",
	"password": "123styri",
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 409,
	"message": "Conflict"
}
```

---

## Upraviť jedlo - PUT

### Request

```
[PUT endpoint] /meal
```

### Request body

```json
{
	"id": 7,
	"name": "Ivkove špagety",
	"description": "Moje mňam mňam špagetky",
	"userId": 3,
	"amount": 20,
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10,
	"isPublic": true,
	"ingredients": [
		{
			"id": 4,
			"amount": 20,
		},
		{
			"id": 5,
			"amount": 10,
		}
	]
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Upraviť potravinu - PUT

### Request

```
[PUT endpoint] /food
```

### Request body

```json
{
	"id": 5,
	"name": "Jablko",
	"description": "Jablko červené",
	"brand": "Veselé jablko zo Žitného ostrova",
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10,
	"isPublic": true,
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Upraviť položku v logu - PUT

### Request

```
[PUT endpoint] /log
```

### Request body

```json
{
	"id": 3,
	"name": "Pizza Hawaii",
	"date": 2022-03-10 14:25,
	"amount": 20,
	"calories": 486,
  "carbs": 80,
  "protein": 20,
  "fat": 10
}
```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Upraviť používateľove informácie - PUT

### Request

```
[PUT endpoint] /user
```

### Request body

```json
{
	"id": 10,
	"firsName": "Peter",
	"lastName": "Zdravý",
	"email": "peter.zdravy@pokec.sk",
	"weight": 100,
	"height": 185,
	"birthday": 1995-10-5,
	"caloriesGoal": 2200,
	"photo": "https://petkovafotka.com/petko"
} 

```

### Responses

```json
{
	"status": 201,
	"message": "Created"
}

{
	"status": 422,
	"message": "Unprocessable Entity"
}
```

---

## Vymazať jedlo - DELETE

### Request

```
[DELETE endpoint] /meal
```

### Parameters

- **id** (integer) - ID jedla

### Responses

```json
{
	"status": 200,
	"message": "OK"
}

{
	"status": 404,
	"message": "Not Found"
}
```

---

## Vymazať potravinu - DELETE

### Request

```
[DELETE endpoint] /food
```

### Parameters

- **id** (integer) - ID potraviny

### Responses

```json
{
	"status": 200,
	"message": "OK"
}

{
	"status": 404,
	"message": "Not Found"
}
```

---

## Vymazať položku v logu - DELETE

### Request

```
[DELETE endpoint] /log
```

### Parameters

- **id** (integer) - ID položky

### Responses

```json
{
	"status": 200,
	"message": "OK"
}

{
	"status": 404,
	"message": "Not Found"
}
```

---

## Vymazať používateľa - DELETE

### Request

```
[DELETE endpoint] /user
```

### Parameters

- **id** (integer) - ID používateľa

### Responses

```json
{
	"status": 200,
	"message": "OK"
}

{
	"status": 404,
	"message": "Not Found"
}
```

---