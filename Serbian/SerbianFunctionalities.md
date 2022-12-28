# Antares Apps doo – Serbian Functionalities Help - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili srpske funkcionalnosti na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.serbianfunctionalities%7CPAPPID.92da857b-0491-42d8-9333-e69b77e879af).

## Podešavanje lokalne valute na RSD
Podesite RSD kao lokalnu valutu u podešavanju glavne knjige. Ovo polje se koristi u sistemu kako bi se odredilo da li su srpske funkcionalnosti aktivne u trenutnom preduzeću.<br/>
Podešavanje glavne knjige -> Šifra LVT

## Podešavanje ažuriranja kurseva valute
Valute -> Servis za kurseve valuta -> Servisi za kurseve valuta<br/>
Nakon zvanja akcije "Servisi za kurseve valuta" veza za Narodnom bankom Srbije je inicijalizovana.<br/>
Otvorite karticu Servisa za kurseve valuta i unesite korisničko ime, šifru i ID licence.<br/>
Uključite servis za kurseve valut i odaberite parametre za pokretanje u red čekanja za posao<br/>
Predloženo podešavanje: Pokretati jednom dnevno u 8:30

## Podešavanje sinhornizacije bankovnih računa dobavljača na osnovu PIB-a
Podešavanje nabavke i dugovanja -> Inicijalizuj sinhronizaciju bankovnih računa<br/>
Nakon zvanja akcije "Inicijalizuj sinhronizaciju bankovnih računa" unesite korisničko ime, šifru i ID licence.

## Podešavanje uvoza i izvoza izvoda
Podešavanje bankovnog izvoza/uvoza -> Inicijalizuj Office Banking<br/>
Podešavanje bankovnog izvoza/uvoza -> Inicijalizuj Halcom Banking<br/>
Kreirati novu račun u banci i uneti vrednost u polje "Format uvoza izvoda iz banke" i u polje "Format izvoza plaćanja"<br/>
Obrasci naloga knjiženja -> kreirati novi obrazac naloga knjiženja npr. PLAĆANJA. Vrsta = Plaćanje<br/>
Obrasci naloga knjiženja -> Povezano -> Obrazac -> Grupe -> Kreirati novu grupu naloga npr. IZVOZ. "Vrsta protivkonta" = Bankovni račun, uneti broj banke u polje "Br. protivkonta"<br/>
Obrasci naloga knjiženja -> Povezano -> Obrazac -> Grupe -> Kreirati novu grupu naloga npr. UVOZ. "Vrsta protivkonta" = Bankovni račun, uneti broj banke u polje "Br. protivkonta"

## Avansi
**1. Podešavanje grupe knjiženja kupaca:**
![image](https://user-images.githubusercontent.com/42636293/202931396-a8ad1a62-8349-4618-a442-70752e979b77.png)

**2. Podešavanje grupe knjiženja dobavljača:**
![image](https://user-images.githubusercontent.com/42636293/209876637-290ef15c-d60c-4ac3-8440-2d63e09ced79.png)

**3. Podešavanje knjiženja za PDV:**
![image](https://user-images.githubusercontent.com/42636293/209876436-d43ac787-0c1b-4436-bb1c-8fc4693cb098.png)

**4. Podešavanje konta:**
![image](https://user-images.githubusercontent.com/42636293/209876779-d443c313-69c3-4c86-aa52-30e28049413b.png)
![image](https://user-images.githubusercontent.com/42636293/209876820-9ac0d3a7-4270-479f-bbb9-249736a00f3e.png)
![image](https://user-images.githubusercontent.com/42636293/209876878-dec1683a-5a79-40eb-8bbd-acb7ab0cf8e4.png)
![image](https://user-images.githubusercontent.com/42636293/209876925-5ffb57b8-4948-418d-b43b-2df28b0ae99a.png)


## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
