Această pagină are ca scop aducerea în atenția publicului larg a unor noțiuni de securitate și privacy în mediul virtual.
Nu o sa folosesc "intimitate" sau "confidențialitate" în loc de "privacy" pentru ca lumea o sa se gandeasca la alte chestii si nu e tot timpul cazul :wink:
Pagina asta e destinată publicului larg, nu experților din zona IT/security, așa că nu aruncați cu ouă și roșii stricate pentru că unele lucruri sunt simplificate. :grin:


## Securitate si privacy - de ce ar trebui sa te intereseze ambele

Faptul ca ceva e sigur nu inseamna musai si ca ofera privacy, iar faptul ca ceva ofera privacy nu inseamna ca e si sigur.
Noțiunea de privacy se poate referi la privacy versus marii colectori de date (Facebook, Google, Yandex, tot felul de scraper-e), versus autorități (cum se spune, "agențiile cu acronime din 3 litere") sau versus alte persoane fizice.
Una e să fentezi algoritmii publicitari și de recomandare de conținut ai Facebook, alta e să te ascunzi de un regim opresiv ca dizident/opoziție, și complet alta e să nu afle rudele că joci Dungeons & Dragons. Sau sa nu afle hoții că ai plecat în concediu și stai mult. Alt caz demn de menționat ar fi victimele (de orice gen) violenței domestice. Persoanele cu parteneri abuzivi (zic la masculin ca sa fie mai general, nu e problema de gen aici) au nevoi mai complexe de privacy, mai ales daca au de gand sa iasa din relatie sau au fugit deja de acasa. E cam ca la protecția martorilor.

Când ne gândim la privacy, trebuie să avem în vedere următoarele:
1. Trackers:
- [Google Firebase Analytics](https://firebase.google.com/docs/analytics)
- Microsoft Appcenter Crashes
- [Countly](https://support.count.ly/hc/en-us/sections/360007405211-User-Guides)
- [Bugsnag](https://docs.bugsnag.com/)
- Piwik [Piwik Customer Data Platform](https://piwik.pro/customer-data-platform/)
2. Metadate de toate felurile (istoric de navigare web, timp petrecut pe un site, reclame accesate, obiecte pe care a stat cu mouse-u etc., date EXIF în cazul imaginilor). Toate acestea pot da informații cu privire la interesele și preferințele utilizatorului fără a accesa efectiv date de identificare ale acestuia
3. Date de localizare (în toate formele)
4. Cookies (care pot fi furate prin diverse metode)
5. Postări pe social media sau alte tipuri de platforme: bineinteles, se pot posta diverse pe social media / net în general, la public, cu asumarea de către autor că, o dată ce a fost postat cu setarea "public", acel conținut poate fi accesat si salvat / arhivat de oricine. La fel și în cazul comunicării printr-o aplicație care nu oferă criptare end-to-end și care permite screenshot (captură de ecran) în conversații.

Securitatea trebuie privita tot timpul in raport cu ceva. Suprafețele de atac sunt multe, iar threat model-urile și mai multe, după cum am menționat mai sus. De aceea, la alegerea telefoanelor, laptop-urilor și aplicațiilor utilizate, trebuie avut în vedere un threat model realist pentru persoana care le va folosi.


## Threat model - ce-i ăla și de ce ar trebui să ne gândim la el

Un threat model este practic un model de amenințare. "Ce tip de adversar am?", "Ce puncte slabe am?", "Unde există vulnerabilități?"
Problema la ora actuală e cam așa: date strâng toți, log-uri țin toți, iar din punct de vedere al "mă va da pe mâna poliției/partidului" toți o vor face cu un mandat în față.

"Aoleo! Hackeri!". Da, corect. Însă și aici intervin unele deosebiri. Să luăm câteva cazuri super simplificate:
- elevi pusi pe glume proaste / răzbunări legate de jocuri video: de obicei aptitudini de bază, uneori nu stiu să se ferească, în general pot fi prinși ușor și dacă sunt conștienți de asta nu vor face mari pagube. Ușor de fentat cu o parolă bună la WiFi și un nume de rețea (SSID) care să nu îi incite, firewall, antivirus și atenția de a nu face click pe toate link-urile dubioase trimise pe diverse aplicații de chat
- skids: denumirea vine de la "script kiddies". Persoane care folosesc programe/script-uri gata făcute de alții și nu își dezvoltă propriile unelte. Gradul de periculozitate depinde de mai mulți factori, însă pot fi fentați cu un minim de măsuri de securitate
- părinți elicopter: acel gen de părinți care exagerează cu supravegherea. Spyware, stalkerware, keyloggers, monitorizarea traficului de net. Li se mai reduce din avânt cu antivirus, monitorizarea traficului de net (dacă vezi că ai conexiuni dubioase e clar că ceva nu e în regulă.. detalii mai încolo), pseudoanonimitate (care oricum e bună pentru minori, că nu vrei să atragi toți dubioșii de pe net și nici să rămâi pentru totdeauna cu cine stie ce username tâmpițel ales la 10 ani)
- scammers: clasicul "Ați câștigat o mașină/bani/etc.! Vă rugăm dați-ne numărul cardului, numele posesorului, data de expirare și CVV-ul pentru a intra în posesia premiului". "Fiul dumneavoastră a accidentat grav un pieton". Și alte asemenea. Ușor de fentat prin a cunoaște pe ce lume trăiești și prin a nu le da nici un fel de date. Phishing tot aici intră
- dragoste și trădare! : aici e grav. În categoria asta intră foști, parteneri abuzivi, parteneri geloși, toata gama. Pot fi orice de la nivel de skid la nivel de APT, doar că au cea mai crâncenă motivație să ți-o coacă. Dacă persoana mai are și aptitudini avansate în domeniul calculatoarelor și al telecomunicațiilor, deja e chiar grav, practic ai un APT care are o problemă personală și intimă cu tine
- APT: Advanced Persistent Threat. Entitate cu capabilități avansate, care obține acces ilegal la un sistem și își stabilește o prezență pe termen lung în acesta. De obicei sunt grupuri cu finanțare puternică în spate, și/sau susținute politic (la nivel de stat). Foarte puțin probabil ca o persoană fizică să aibe de-a face cu așa ceva. De obicei iau în vizor companii, entități industriale, elemente de infrastructură critică, instituții de stat, cu scopuri diverse: colectare de date sensibile/secrete, sabotaj, furt de proprietate intelectuală (putin mai pe larg aici: [APT](https://www.imperva.com/learn/application-security/apt-advanced-persistent-threat/) )

Cu cât avem mai multe programe/aplicații instalate și mai multe conturi de utilizator pe diverse platforme, cu atât avem mai multe potențiale puncte slabe. Crește suprafața de atac. Dacă aplicațiile respective nu sunt cu update-urile la zi, se agravează situația. Patching-ul și actualizările sunt importante. 

Un smartphone care e out-of-support (nu mai primește update-uri de sistem de operare) reprezintă o vulnerabilitate. Nu doar că sistemul de operare al acestuia nu este la zi cu patch-urile de securitate, dar la un moment dat și aplicațiile instalate rămân în urmă. Cât timp acest software tot rămâne în urmă, se găsesc portițe pentru a exploata vulnerabilitățile lor (noi unelte de hacking etc.). Instalarea de aplicații inutile, de exemplu calculator sau lanternă - orice telefon mobil cat de cat recent are acestea implicit, duce la mărirea riscului. Unele din ele chiar sunt malware/spyware, chiar dacă sunt pe Play Store. 

Trebuie să ținem cont de toate device-urile conectate pe care le avem: telefoane mobile, laptop, PC, console de jocuri video, Smart TV, smart orice, orice chestie din gama IoT (aspirator, frigider, etc). Cu cât avem mai multe device-uri conectate la net, cu atât avem mai multe potențiale puncte slabe. Orice are cameră și se conectează la net trebuie tratat cu atenție. Și camerele de supraveghere trebuie puse în locuri unde nu pun viața privată în pericol și securizate cum trebuie, cu patch la zi, username și parolă greu de ghicit/aflat, etc., altfel uite așa ajungi vedetă porno pe [Shodan](https://www.shodan.io/) și după aia la secțiunea de amatori de pe toate site-urile "picante".

Legat de conturi pe diverse platforme: pe cele mari si bine puse la punct se pot face fără grijă conturi utilizând numărul de telefon și adresa de email "primară" (dacă nu se dorește anonimitate, evident). Pe tot felul de forumuri sau aplicații de hobby-uri (din gama celor găsite pe ceea ce se numește clear web, adică ce vedem în mod normal dintr-un browser obișnuit) se recomandă crearea unui cont cu nume de utilizator diferit de cel real, poză de profil diferită de cea reală (și preferabil să nu se repete între ele), dintr-o adresă de email secundară. Pentru forumurile din dark web (care pot fi accesate doar prin Tor) evident că recomandat e să ai anonimitate, folosind o adresă de email (pseudo)anonimă (care nu cere număr de telefon sau alte date reale la înscriere), nume de utilizator total irelevant și poză de profil lipsă sau irelevantă. 
Ca rezumat: cu cât e mai dubios forumul, cu atât ar trebui să fie mai clar că e cazul să fii anonim. Acum intrebarea ar fi ce să cauți pe așa ceva daca ești om cuminte? De exemplu, pentru a vedea dacă datele tale apar pe undeva, sau pentru a vedea dacă au fost postate poze cu tine (care evident nu le vrei publice). Dar despre astfel de verificări, mai încolo puțin.

Dacă un forum/site (non-guvernamental) îți cere confirmarea datelor cu o poză a unui act de identitate oficial (carte de identitate, pașaport, permis de conducere auto), e absolut clar că e dubioasă treaba. Mai ales dacă nu are de ce să respecte GDPR. Nici un forum/site care nu aparține unei entități a statului nu are de ce să ceară așa ceva, și te pui în pericol dacă le dai. La un moment dat vor fi ori sparți ori luați de autorități, iar datele tale personale vor fi peste tot, în funcție de pe cine au supărat (a se vedea cazul Parler). 

Deci: conturi multe, cu același nume de utilizator (real sau cu legătură cu cel real), legate toate de 1-3 adrese de email ce pot fi legate de o identitate reală, cu poze de profil identice = rău. Chiar dacă nu vrei musai să te ascunzi de cineva, bogăția asta de date înșirate peste tot conduce la extragerea ușoară a și mai multe date despre tine, care în final pot duce la compromiterea unor conturi sau device-uri (de exemplu cu parole puse pe baza datelor de naștere, numele animalelor de companie, hobby-uri). Toate conturile pe care le avem trebuie luate în calcul la threat model, pentru că fiecare din ele și modul în care a fost făcut poate reprezenta o vulnerabilitate.

Pentru accesarea conținutului unor site-uri care insistă să le dai o adresă de email sau pentru descărcarea unor documente care necesită email se poate folosi o adresă de email temporară sau burner (gen TempMail, mailpoof, emailondeck, guerilla mail). Acest lucru te scapă de o grămadă de spam și eventuale mail-uri de phishing.

Altă mare problemă o reprezintă aplicațiile de chat. Și aici, problemele sunt cam la fel: vrem sau nu anonimitate? De cine trebuie să ne ferim? La ce o folosim mai exact (ce tip de comunicare și cu cine)?

## Cum alegem o aplicație de chat
Agitația recentă cu noua politică Whatsapp a generat o grămadă de discuții și a readus aspectele de securitate/privacy în atenția publicului larg. În esență, au zis că platforma Facebook va avea acces și la (meta)datele din Whatsapp. Și că teoretic nu se aplică în UE. Mai multe despre asta se poate citi direct pe site-ul lor, la partea cu politici de securitate și privacy. Acest lucru are impact mai degrabă asupra algoritmilor publicitari, nu înseamnă că aplicația e musai mai puțin sigură în fața unor atacatori sau a unor interceptări legale. Apropos de interceptări legale, în cazul lor e vorba mai mult despre (pseudo)anonimat, că decriptoare au și autoritățile. Recomand citirea documentației tehnice generale și a politicilor de securitate și privacy pentru aplicațiile folosite/luate în calcul.

Câteva lucruri de luat în considerare la alegerea unei aplicații de chat:
- ce permisiuni necesită din partea sistemului de operare
- ce date necesită pentru utilizare și ce date leagă de tine
- cât și cum stochează aceste date, chiar și după ștergerea contului
- cripare: nu? da? end-to-end? ce algoritm?
- ce setări de privacy oferă
- ce alte vulnerabilități are (de exemplu, tastatura utilizată)

Un rezumat bun e aici: [Secure messaging apps comparison](https://www.securemessagingapps.com/)

### Permisiuni necesare aplicațiilor de chat

Cu cât o aplicație are nevoie de mai multe permisiuni, cu atât e mai rău, pentru foarte mult numărul de chestii care pot fi folosite în scop malițios.
În articolul de mai jos sunt detaliate destul de clar permisiunile necesare celor mai populare aplicații, cu excepția Facebook Messenger, ca nu mai era cazul sa o discute si pe aceea, fiind una din cele care necesită cele mai multe permisiuni.

[Android trackers and permissions: Did I say you could do that?](https://getsession.org/android-trackers-and-permissions/)
![Android trackers and permissions table](https://getsession.org/wp-content/uploads/2020/06/small_clean_permissions_test_2-e1599620821852.png)
sursă foto: Session App

### Date necesare și (pseudo)anonimitate

Câte/ce date sunt necesare pentru a utiliza o aplicație? 
Cele mai multe necesită cel puțin număr de telefon. Multe cer și număr de telefon, și adresă de email, cu limitări la provider-ul de email.

Ca idee, nu puteti adera la Facebook folosind chiar orice adresă de email, iar crearea unui cont de Gmail sau Yahoo necesita număr de telefon. Bineînțeles că în România înca se mai pot cumpăra SIM-uri prepay fără act de identitate folosind cash, dar în multe țări acest lucru e imposibil.

De exemplu, [Session](https://getsession.org/) nu necesită în nici un fel număr de telefon sau adresă de email. Altele necesită, dar nu insistă sa fie de la un provider "clasic" (mainstream), deci se pot utiliza servicii de mail "puțin mai anonime", de tip Protonmail sau Tutanota. 

Pentru a folosi Protonmail este necesar un număr de telefon, dar acesta poate fi unul temporar obținut prin aplicații de tip CoverMe, sau un burner (cartelă SIM prepay, cumpărată preferabil cu bani cash, utilizată cu un singur scop într-un telefon care nu are teoretic nici o legătură cu persoana respectivă). 

[Tutanota](https://tutanota.com/) nu cere nici număr de telefon, nici altă adresă de email.

[Status](https://status.im/account-creation/) nu necesită nici număr de telefon, nici adresă de email.

Telegram necesită număr de telefon, dar acesta poate fi complet ascuns față de ceilalți participanți la conversație. Nu cere adresă de email și nici setarea unui username, iar numele poate fi schimbat inclusiv într-un emoji.

Signal necesită număr de telefon, nu oferă posibilitatea de a-l ascunde de alții și, mai rău, te anunță când cineva din lista de contacte a aderat. Ce e rău în asta? De exemplu, următoarea situație: persoană cu partener abuziv aderă la Signal pentru a comunica cu familia si avocatul în vederea ieșirii din relație. Partenerul vede notificarea, se enervează (că percepe Signal ca fiind o aplicație folosită de cei care vor să se ascundă pentru a face rele), poate acționa violent față de celălalt și/sau îi poate confisca telefonul, tăind-ui astfel contactul cu cercul de susținere.

Numărul de telefon, adresa de email, precum si o gamă largă de alte date sunt legate de utilizator. Un update recent la Apple App Store a introdus posibilitatea de a vedea ce date sunt legate de tine, per aplicație, și ce date sunt colecționate.

![Date legate de tine, per app](https://i1.wp.com/9to5mac.com/wp-content/uploads/sites/6/2021/01/App-privacy-labels-messaging-apps.png)
sursă foto: Forbes
