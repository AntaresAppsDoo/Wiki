# Antares Apps doo – Antares Payroll Help - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili Antares Payroll na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.payroll%7CPAPPID.82ed9411-e456-4ed9-848d-035fead71575).

## Dozvole za Zarade
U modulu za zarada predviđena su tri nivoa pristupa:
* Administrator za zarade
  * Ima neograničena prava u modulu za zarade
  * preporučeni skup dozvola za Cloud okruženje: SUPER ili neki drugi skup dozvola sa administratorskim pravima u kombinaciji sa "ANTPAYROLLADMIN" skupom dozvola.
  * Globalna Pretraga -> Podešavanje korisnika -> Korisnik zarada -> Administrator<br/>
* Referent za obračuna zarada
  * U odnosu na prava administratora nema prava da menja opšta podešavanja u modulu.
  * preporučeni skup dozvola za Cloud okruženje: "D365 READ", "D365 HR, EDIT" i "ANTPAYROLLOFFICER" 
  * Globalna Pretraga -> Podešavanje korisnika -> Korisnik zarada -> Referent za obračun<br/>
* Menadžer ugovora za zarade
  * Može da menja Ugovore zaposlenih kao i njihove obustave i bonuse.
  * preporučeni skup dozvola za Cloud okruženje: "D365 READ", "D365 HR, EDIT" i "ANTPAYROLLCONTRMAN" 
  * Globalna Pretraga -> Podešavanje korisnika -> Korisnik zarada -> Menadžer ugovora<br/>
  
Nakon instalacije potrebno je da barem jedan korisnik bude podešen kao administrator zarada u podešavanju korisnika. Ukoliko to nije slučaj nije moguće inicijalno podešavanje zarada.<br/>
U slučaju potrebe korišćenja sigurnosnih filtera kako bi se npr. menadžer ugovora ograničio na pristup samo određenim ugovorima, potrebno je uraditi sledeću proceduru:<br/>
Skupovi dozvola -> pozicioniranje na skup dozvola "ANTPAYROLLCONTRMAN" -> Kopiraj skup dozvola -> Kopiranje po referenci -> Otvaranje novokreiranog skupa dozvola i dodavanje samo željenih tabela sa sigurnosnim filterima.

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
1. Štampa rekapitulacije obračuna i platnog spiska se može pozvati sa kartice obračuna ili sa liste obračuna
1. Isplatnih listići se mogu odštampati i poslati svakom zaposlenom pojedinačno ili automatski za ceo obračun korišćenjem e-pošte. Više informacija: [Isplatni listići](https://github.com/AntaresAppsDoo/Wiki/blob/main/Serbian/PaySlips.md).    

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

## Podešavanje izveštaja
Sa modulom za zarade isporučuju se sledeći izveštaji:
* Isplatni list
* Rekapitulacija obračuna
* Potvrda o plaćenim porezima i doprinosima po odbitku
* Platni spisak za obračun
* Platni spisak za obračun sa raspodelom po projektima

Ove izveštaje je moguće zameniti korisnički definisanim izveštajima korišćenjem stranice za izbor izveštaja za modul zarade:
![image](https://github.com/user-attachments/assets/5ca31c1a-8435-4015-8b8c-dcc6902dfb9c)  


Na primeru platnog spiska moguće je odabrati jedan od dva izveštaja. Običan platni spisak je pojednostavljena lista primanja zaposlenih dok drugi sadrži više detalja po kategorijama rada i omogućuje pregled sa raspodelom po projektima u Excel formati.
![image](https://github.com/user-attachments/assets/efec6654-5cd7-4317-9e29-810d3429d275) 
![image](https://github.com/user-attachments/assets/bdd509f7-48b3-465c-a6a4-ea89b9decf93)

![image](https://github.com/user-attachments/assets/990ffa54-a948-43b8-b4ea-2e0858047eec)  
  
![image](https://github.com/user-attachments/assets/87e0e2fe-8db3-4764-b29e-3e14d7e6978d)



## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
