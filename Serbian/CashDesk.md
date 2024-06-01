# Antares Apps doo – Blagajna - Podešavanje

## Instalacija
[Kliknite ovde da biste pretražili srpske funkcionalnosti na AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.serbianfunctionalities%7CPAPPID.92da857b-0491-42d8-9333-e69b77e879af).

## Kreiranje blagajne
Kako biste kreirali blagajnu, potrebno je da odete na Blagajne i odaberete +Novo. Tada će se otvoriti Kartica blagajne gde treba popuniti odgovarajuća polja.<br/> Obavezna polja koja morate popuniti su Grupa knjiženja blagajne, Konto zaokruživanja dugovanja, Konto zaokruživanja potraživanja, Šifra metoda zaokruživanja, Limit za uplatu i Limit za isplatu. <br/>
U sekciji Numerisanje potrebno je za polje Brojčana serija za uplatu odabrati CASH-DESK-RECEIPT, a za polje Brojčana serija za isplatu CASH-DESK-WITHDRAWAL. Time je završen proces kreiranja blagajne.

## Kreiranje obrazaca blagajne
Kako biste kreirali obrasce blagajne, potrebno je da odete na podešavanja, Moja podešavanja i odaberete ulogu Računovođa. U sekciji Blagajna idite na Obrasci blagajne i kada se otvori kartica Obrasci blagajne idite na +Novo i kreirajte obrazac blagajne popunjavajući odgovarajuća polja uz obavezno popunjavanje polja Br. blagajne i polja Tip gotovinskog dokumenta. Za svaku blagajnu možete proveriti da li ima kreirane obrasce tako što ćete kliknuti na Povezano, odabrati Setup i kliknuti na Obrasci blagajne. Ukoliko želite da koristite Obrasce blagajne prilikom kreiranja novog gotovinskog dokumenta, u sekciji Redovi, kliknite na Obrazac blagajne i odaberite željeni obrazac. 

## Kreiranje gotovinskog dokumenta
Kako biste kreirali gotovinski dokument, potrebno je da kliknete na broj blagajne i kada se otvori kartica blagajne idite na opciju Novi Dokument, Gotovinski Dokument.<br/>
U sekciji Opšte potrebno je popuniti obavezna polja Vrsta dokumenta i Svrha uplate/isplate.<br/>
U sekciji Linije, potrebno je popuniti polje Vrsta entiteta odabirom neke od ponuđenih opcija (u zavisnosti od Vrste dokumenta i Svrhe uplate), Br.entiteta i Iznos. Time je gotovinski dokument kreiran i automatski mu je dodeljen status Otvoreni.

## Izdavanje dokumenta
Kako biste promenili status dokumenta u Izdati, potrebno je otići na karticu Izdaj i odabrati opciju Izdaj.<br/>
Ako dokument već ima satus Izdato, ukoliko odaberete opciju Ponovo otvori, vratićete ga na status Otvoreni. 

## Knjiženje gotovinskog dokumenta
Ukoliko želite da proknjižite gotovinski dokument idite na karticu Proknjiži i potvrdite da želite da proknjižite odgovarajući dokument.<br/> 
Dokument će promeniti status u Proknjiženo i automatski će se smestiti u proknjižene gotovinske dokumente.<br/>
Za svaki proknjiženi dokument možete otiči na karticu Pronađi stavke i dobiti prikaz svih stavki i dokumenata vezanih za taj dokument i datum knjiženja.

## Štampanje gotovinskog dokumenta
Štampanje gotovinskog dokumenta možete izvršiti tako što ćete označiti odgovarajuću blagajnu, kliknuti na karticu Povezano, odabrati opciju Dokumenti i izabrati jednu od tri ponuđene grupe dokumenata (Otvoreni gotovinski dokumenti, Izdati gotovinski dokumenti, Proknjiženi gotovinski dokumenti).<br/> 
Tada će se otvoriti lista gotovinskih dokumenata, gde je potrebno kliknuti na željeni dokument kako biste ga otvorili.<br/> 
Kada otvorite određeni gotovinski dokument, potrebno je otići na karticu Štampaj i odabrati opciju Štampaj.

## Podešavanje načina plaćanja
Kako biste podesili način plaćanja preko blagajne, potrebno je da odete na podešavanja, Moja podešavanja i odaberete ulogu Računovođa. U prozoru za pretragu, kucajte Načini plaćanja i otvorite stranu Načini plaćanja.<br/>  
Iz liste ponuđenih načina, odaberite CASH DESK, u koloni Šifra blagajne odaberite blagajnu preko koje će se vršiti plaćanje, a u koloni Gotovinski dokument Akcija, odaberite jednu od ponuđenih opcija.<br/> 
Ukoliko odaberete opciju Kreiraj, gotovinski dokument će biti kreiran i imaće status Otvoreni. Ukoliko odaberete opciju Izdavanje, gotovinski dokument će imati status Izdati, ukoliko odaberete opciju Proknjiži, dokument će automatski biti proknjižen i imaće status Proknjiženi, dok opcije Izdaj i štampaj i Proknjiži i štampaj imaju i mogućnost automatskog štampanja.

## Knjiženje prodajnog ili nabavnog dokumenta
Ukoliko kreirate nabavnu fakturu za nekog dobavljača i odaberete u polju Šifra načina plaćanja CASH DESK, u zavisnosti od podešene akcije na načinu plaćanja, dokument će biti kreiran, izdat ili proknjižen uz mogućnost i automatskog štampanja.<br/> 
Ukoliko kreirate prodajnu fakturu za nekog kupca i odaberete u polju  Šifra načina plaćanja CASH DESK, u zavisnosti od podešene akcije na načinu plaćanja, dokument će biti kreiran, izdat ili proknjižen uz mogućnost i automatskog štampanja. 

## Prijava problema
Ukoliko naiđete na problem molimo Vas da prijavite slučaj na sledećem linku:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
