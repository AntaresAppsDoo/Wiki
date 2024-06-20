# Antares Apps doo – Antares Payroll Help - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili Antares Payroll na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.payroll%7CPAPPID.82ed9411-e456-4ed9-848d-035fead71575).

## Dozvole za Zarade
Nakon instalacije potrebno je da barem jedan korisnik bude podešen kao administrator zarada:<br/>
Globalna Pretrage -> Podešavanje korisnika -> Korisnik zarada -> Administrator<br/>
Ukoliko je korisnik podešen kao Referent za obračun za naknadno otvaranje zatvorenih obračuna moraće da se obrati administratoru.

## Uloga za Zarade
Posle instalacije možete promeniti vašu ulogu na ulogu za Zarade koristeći sledeću putanju:<br/>
Moja podešavanja -> Uloga -> Obračun zarada

## Demonstracioni podaci
Da biste instalirali osnovne demonstracione podatke pokrenite proces pozivajući akciju:<br/>
Podešavanje -> Podešavanje zarada -> Inicijalizuj podešavanja
1. Odabirom opcije "Zemlje i poštanski brojevi" u Business Central-u će biti kreiran zapis za Srbiju u tabeli "Države/regioni" kao i sve opštine iz Srbije u tabeli "Poštanski brojevi". Postojeći zapisi u ove dve tabele mogu biti ažurirani. Zemlja i poštanski broj se nakon toga mogu dodeliti na kartici zaposlenog.
2. Odabirom opcije "Kalendar i obrasci za radne sate" u Business Central-u će biti kreiran zapis za Srbiju u tabeli "Lista osnovnih kalendara" sa svih praznicima u tekućoj i godini posle tekuće. Takođe biće kreiran 40-časovni obrazac za radne sate. Kalendar i obrazac za radne sate se mogu dodeliti prilikom kreiranja ugovora zaposlenog.
3. Odabirom opcije "Podešavanja obračuna" kreiraju se sve trenutno podržane vrste obračuna u modulu za zarade sa svim pripadajućim podešavanjima vezano za poreze i doprinose.
![image](https://github.com/AntaresAppsDoo/Wiki/assets/42636293/49ae92b1-4c9e-484d-a34f-3832cf5e35dc)

## Pokretanje obračuna zarada
1. Kreirajte novog zaposlenog iz liste zaposleni
1. Unesite Ime, prezime, JMBG, adresu i broj bankovnog računa
1. Otvorite ugovore za zaposlenog pozivajući akciju Zaposleni -> Ugovori
1. Unesite početak trajanja ugovora, Šifru ugovora o radu, Radno mesto, Obrazac za radne sate, Vrstu iznosa i iznos
1. Kreirajte novi obračun iz liste obračuna
1. Unesite šifru ugovora o radu na kartici obračuna
1. Pozovite akciju "Kreiraj zaposlene u obračunu"
1. U slučaju da se radi o vrsti ugovora za istraživanje i razvoj potrebno sa kartice obračuna pozvati karticu zaposlenog i uneti sate koje je zaposleni proveo na poslovima istraživanja i razvoja.
1. Izvezite obračun u XML kako biste mogli da podnesete poresku prijavu koristeći akciju "Izvezi obračun u XML"
1. Izvezite obračun u nalog knjiženja koristeći akciju "Izvoz u nalog knjiženja"
1. Zatvorite obračun kako biste sprečili dalje menjanje obračuna
1. Plaćanje se vrši kroz Nalog plaćanje pozivom akcije "Predloži isplate po obračunu zarada"

## Neophodni podaci prilikom generisanja poreske prijave u XML formatu
1. Podaci o preduzeću -> Ime
1. Podaci o preduzeću -> Adresa
1. Podaci o preduzeću -> PIB
1. Podaci o preduzeću -> Matični broj
1. Podaci o preduzeću -> Poštanski broj -> Sedište prebivališta odgovara polju "Šifra plaćanje za opštinu" poštanskom broju
1. Podešavanje korisnika -> E-adresa
1. Podešavanje korisnika -> Br. telefona
1. Zaposleni -> Poštanski broj -> Oznaka prebivališta odgovara polju "Šifra plaćanje za opštinu" poštanskom broju
1. Broj zaposlenih se generiše na osnovu svih aktivnih redovno zaposlenih posmatrano na prvi dan obračuna

## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
