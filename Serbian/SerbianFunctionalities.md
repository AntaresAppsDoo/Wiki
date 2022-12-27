# Antares Apps doo – Serbian Functionalities Help - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili srpske funkcionalnosti na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.serbianfunctionalities%7CPAPPID.92da857b-0491-42d8-9333-e69b77e879af).

## Podešavanje lokalne valute na RSD
Podesite RSD kao lokalnu valutu u podešavanju glavne knjige. Ovo polje se koristi u sistemu kako bi se odredilo da li su srpske funkcionalnosti aktivne u trenutnom preduzeću.
Podešavanje glavne knjige -> Šifra LVT

## Podešavanje ažuriranja kurseva valute
Valute -> Servis za kurseve valuta -> Servisi za kurseve valuta
Nakon zvanja akcije "Servisi za kurseve valuta" veza za Narodnom bankom Srbije je inicijalizovana.
Otvorite karticu Servisa za kurseve valuta i unesite korisničko ime, šifru i ID licence.
Uključite servis za kurseve valut i odaberite parametre za pokretanje u red čekanja za posao
Predloženo podešavanje: Pokretati jednom dnevno u 8:30

## Podešavanje sinhornizacije bankovnih računa dobavljača na osnovu PIB-a
Podešavanje nabavke i dugovanja -> Inicijalizuj sinhronizaciju bankovnih računa
Nakon zvanja akcije "Inicijalizuj sinhronizaciju bankovnih računa" unesite korisničko ime, šifru i ID licence.

## Podešavanje uvoza i izvoza izvoda
Podešavanje bankovnog izvoza/uvoza -> Inicijalizuj Office Banking
Podešavanje bankovnog izvoza/uvoza -> Inicijalizuj Halcom Banking
Kreirati novu račun u banci i uneti vrednost u polje "Format uvoza izvoda iz banke" i u polje "Format izvoza plaćanja"
Obrasci naloga knjiženja -> kreirati novi obrazac naloga knjiženja npr. PLAĆANJA. Vrsta = Plaćanje
Obrasci naloga knjiženja -> Povezano -> Obrazac -> Grupe -> Kreirati novu grupu naloga npr. IZVOZ. "Vrsta protivkonta" = Bankovni račun, uneti broj banke u polje "Br. protivkonta"
Obrasci naloga knjiženja -> Povezano -> Obrazac -> Grupe -> Kreirati novu grupu naloga npr. UVOZ. "Vrsta protivkonta" = Bankovni račun, uneti broj banke u polje "Br. protivkonta"

## Avansi
**1. Podešavanje grupe knjiženja kupaca:**
![image](https://user-images.githubusercontent.com/42636293/202931396-a8ad1a62-8349-4618-a442-70752e979b77.png)

**2. Opšte podešavanje knjiženja:**
![image](https://user-images.githubusercontent.com/42636293/202930974-e63c6b6f-877d-4587-8407-e1cc6f02477d.png)

**3. Podešavanje knjiženja za PDV:**
![image](https://user-images.githubusercontent.com/42636293/202931140-7850580c-d41b-4be3-afb0-af21d34afc68.png)
**4. Podešavanje konta:**
![image](https://user-images.githubusercontent.com/42636293/202931194-c1c71e92-3d57-40c3-9c3f-4ed195bfd4d5.png)
![image](https://user-images.githubusercontent.com/42636293/202931215-15cc0cee-b043-4a92-a881-1a35cc942424.png)


## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
