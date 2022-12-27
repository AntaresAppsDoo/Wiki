# Antares Apps doo – Antares Payroll Help - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili Antares Payroll na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.payroll%7CPAPPID.82ed9411-e456-4ed9-848d-035fead71575).

## Uloga za Zarade
Posle instalacije možete promeniti vašu ulogu na ulogu za Zarade koristeći sledeću putanju:<br/>
Moja podešavanja -> Uloga -> Obračun zarada

## Demonstracioni podaci
Da biste instalirali osnovne demonstracione podatke pokrenite proces pozivajući akciju:<br/>
Podešavanje -> Podešavanje zarada -> Inicijalizuj podešavanja

## Pokretanje obračuna zarada
1. Kreirajte novog zaposlenog iz liste zaposleni
1. Unesite Ime, prezime, JMBG, adresu i broj bankovnog računa
1. Otvorite ugovore za zaposlenog pozivajući akciju Zaposleni -> Ugovori
1. Unesite početak trajanja ugovora, Šifru ugovora o radu, Radno mesto, Obrazac za radne sate, Vrstu iznosa i iznos
1. Ponovite postupak za šifru ugovora o radu za prevoz
1. Kreirajte novi obračun iz liste obračuna
1. Unesite šifru ugovora o radu na kartici obračuna
1. Pozovite akciju "Kreiraj zaposlene u obračunu"
1. Izvezite obračun u XML kako biste mogli da podnesete poresku prijavu koristeći akciju "Izvezi obračun u XML"
1. Izvezite obračun u nalog knjiženja koristeći akciju "Izvoz u nalog knjiženja"
1. Zatvorite obračun kako biste sprečili dalje menjanje obračuna
1. Plaćanje se vrši kroz Nalog plaćanje pozivom akcije "Predloži isplate po obračunu zarada"

## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
