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

## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
