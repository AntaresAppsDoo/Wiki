# Antares Apps doo – Efakture i fiskalni računi

# Opis funkcionalnosti
Podržana je integracija sa državnim portalima:
1. Efakture: https://www.efaktura.gov.rs/
1. Fiskalni računi: https://suf.purs.gov.rs/ 

## Podešavanje servisa za edokumente
Uveriti se da su uvezene definicije za razmenu podataka. Ukoliko navedene definicije nisu prisutne potrebno je uvesti ih sa Cronus baze.
![image](https://github.com/user-attachments/assets/57419b62-6321-4db3-b828-3ad203a16ba7)  
U globalnoj pretrazi potrebno je naći stranicu za podešavanje servisa za edokumente:  
![image](https://github.com/user-attachments/assets/44446fef-46c7-4bda-894d-2da5e8f70d57) 
Nakon toga potrebno je inicijalizovati podešavanje servisa:  
![image](https://github.com/user-attachments/assets/eb1ed3d4-ddf8-419c-bdb1-aacb91df9dc6)  
Za integraciju sa efakturama potrebno je podešavanje prema pristupnom ključu na portal:  
![image](https://github.com/user-attachments/assets/b91823b5-383e-4576-87cf-45139140ed43)  

## Podešavanje podataka o preduzeću koje prima efakture
Prilikom primanja dokumeata sa portala sistem proverava da li se PIB preduzeća slaže sa e-dokumentom. PIB je u formatu dokumenta naveden sa prefiksom RS.
Primer: RS100000000
Ukoliko se u bazi PIB brojevi čuvaju bez prefiksa zemlje "RS" potrebno je da se za servis za edokumente isključi provera PIB-a.  
![image](https://github.com/user-attachments/assets/5b130c91-0d39-4e6b-b4b3-196ae27278f8)  

## Podešavanje dobavljača
Da bi dokument za dobavljača mogao biti konvertovan u nabavni dokument potrebno je za dobavljača uneti PIB broj kao i podešavanje željenog nabavnog dokumenta:  
![image](https://github.com/user-attachments/assets/e0e1898f-59ea-4d1e-817c-afd7fa0b73bc)  

## Podešavanje jedinica mera
Jedinice mere koje u sistemu moraju da odgovaraju onima koje se nalaze u e-dokumentima. Ukoliko prilikom obrade dokumenata dobijete grešku da jedinica mere ne postoji u sistemu, potrebno je kreirati odgovarajuću jedinicu mere u sistemu.  
![image](https://github.com/user-attachments/assets/9ab92194-7db5-44af-891b-db39f590299e)  

## Podešavanje mapiranja teksta u konto
Na dobavljaču kao i na primljenom e-dokumentu dostupna je akcija pod nazivom "Mapiranje teksta u konto". Pozivom ove akcije realizuje se poslednji korak neophodan kako bi primljeni E-dokument automatski bio konvertovan u nabavni dokument u okviru Business Central-a.  
![image](https://github.com/user-attachments/assets/2c773615-c993-4f99-90ed-84ec630cc389)  

## Primanje dokumenata sa portala za efakture:
Primanje dokumenata moguće je izvršiti na:
1. Datum rada
2. Proizvoljno uneti datum
3. Za period  
![image](https://github.com/user-attachments/assets/f2ef6b53-80d5-46a2-91cf-e3d5114666e4)  




