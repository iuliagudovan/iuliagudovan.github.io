Această pagină are ca scop aducerea în atenția publicului larg a unor noțiuni de securitate și privacy în mediul virtual.
Nu o sa folosesc "intimitate" sau "confidențialitate" în loc de "privacy" pentru ca lumea o sa se gandeasca la alte chestii si nu e tot timpul cazul.
Pagina asta e destinată publicului larg, nu experților din zona IT/security, așa că nu aruncați cu ouă și roșii stricate pentru că unele lucruri sunt simplificate. 
Spre final e putin mai tehnic :)

## Cuprins
1. [Securitate si privacy - de ce ar trebui sa te intereseze ambele](https://github.com/iuliagudovan/iuliagudovan.github.io/blob/gh-pages/index.md#securitate-si-privacy---de-ce-ar-trebui-sa-te-intereseze-ambele)
2. [Threat model - ce-i ăla și de ce ar trebui să ne gândim la el](https://github.com/iuliagudovan/iuliagudovan.github.io/blob/gh-pages/index.md#threat-model---ce-i-%C4%83la-%C8%99i-de-ce-ar-trebui-s%C4%83-ne-g%C3%A2ndim-la-el)
3. [Cum alegem o aplicație de chat](https://github.com/iuliagudovan/iuliagudovan.github.io/blob/gh-pages/index.md#cum-alegem-o-aplica%C8%9Bie-de-chat)
4. [Cum îmi dau seama dacă parola/datele mele circulă libere pe net?](https://github.com/iuliagudovan/iuliagudovan.github.io/blob/gh-pages/index.md#cum-%C3%AEmi-dau-seama-dac%C4%83-paroladatele-mele-circul%C4%83-libere-pe-net)
5. ["You don't know the power of The Dark Side!": Darknet, deep web - cum se intră, cum te protejezi, ce găsim acolo?](https://github.com/iuliagudovan/iuliagudovan.github.io/blob/gh-pages/index.md#you-dont-know-the-power-of-the-dark-side-darknet-deep-web---cum-se-intr%C4%83-cum-te-protejezi-ce-g%C4%83sim-acolo)

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
6. Accesul fizic la device-uri și raza vizuală

Securitatea trebuie privita tot timpul in raport cu ceva. Suprafețele de atac sunt multe, iar threat model-urile și mai multe, după cum am menționat mai sus. De aceea, la alegerea telefoanelor, laptop-urilor și aplicațiilor utilizate, trebuie avut în vedere un threat model realist pentru persoana care le va folosi.


## Threat model - ce-i ăla și de ce ar trebui să ne gândim la el

Un threat model este practic un model de amenințare. "Ce tip de adversar am?", "Ce puncte slabe am?", "Unde există vulnerabilități?"
Problema la ora actuală e cam așa: date strâng toți, log-uri țin toți, iar din punct de vedere al "mă va da pe mâna poliției/partidului" toți o vor face cu un mandat în față.

"Aoleo! Hackeri!". Da, corect. Însă și aici intervin unele deosebiri. Să luăm câteva cazuri super simplificate:
- elevi pusi pe glume proaste / răzbunări legate de jocuri video: de obicei aptitudini de bază, uneori nu stiu să se ferească, în general pot fi prinși ușor și dacă sunt conștienți de asta nu vor face mari pagube. Ușor de fentat cu o parolă bună la WiFi și un nume de rețea (SSID) care să nu îi incite, firewall, antivirus și atenția de a nu face click pe toate link-urile dubioase trimise pe diverse aplicații de chat; știu că sunt și elevi foarte talentați în domeniu, dar vorbesc de cazul general, elevul tipic din România, nu de elite
- skids: denumirea vine de la "script kiddies". Persoane care folosesc programe/script-uri gata făcute de alții și nu își dezvoltă propriile unelte. Gradul de periculozitate depinde de mai mulți factori, însă pot fi fentați cu un minim de măsuri de securitate
- părinți elicopter: acel gen de părinți care exagerează cu supravegherea. Spyware, stalkerware, keyloggers, monitorizarea traficului de net. Li se mai reduce din avânt cu antivirus, monitorizarea traficului de net (dacă vezi că ai conexiuni dubioase e clar că ceva nu e în regulă.. detalii mai încolo), pseudoanonimitate (care oricum e bună pentru minori, că nu vrei să atragi toți dubioșii de pe net și nici să rămâi pentru totdeauna cu cine stie ce username tâmpițel ales la 10 ani)
- scammers/țepari: clasicul "Ați câștigat o mașină/bani/etc.! Vă rugăm dați-ne numărul cardului, numele posesorului, data de expirare și CVV-ul pentru a intra în posesia premiului". "Fiul dumneavoastră a accidentat grav un pieton". Și alte asemenea. Ușor de fentat prin a cunoaște pe ce lume trăiești și prin a nu le da nici un fel de date. Phishing tot aici intră
- dragoste și trădare! : aici e grav. În categoria asta intră foști, parteneri abuzivi, parteneri geloși, toata gama. Pot fi orice de la nivel de skid la nivel de APT, doar că au cea mai crâncenă motivație să ți-o coacă. Dacă persoana mai are și aptitudini avansate în domeniul calculatoarelor și al telecomunicațiilor, deja e chiar grav, practic ai un APT care are o problemă personală și intimă cu tine
- APT: Advanced Persistent Threat. Entitate cu capabilități avansate, care obține acces ilegal la un sistem și își stabilește o prezență pe termen lung în acesta. De obicei sunt grupuri cu finanțare puternică în spate, și/sau susținute politic (la nivel de stat). Foarte puțin probabil ca o persoană fizică să aibe de-a face cu așa ceva. De obicei iau în vizor companii, entități industriale, elemente de infrastructură critică, instituții de stat, cu scopuri diverse: colectare de date sensibile/secrete, sabotaj, furt de proprietate intelectuală (putin mai pe larg aici: [APT](https://www.imperva.com/learn/application-security/apt-advanced-persistent-threat/) )

Cu cât avem mai multe programe/aplicații instalate și mai multe conturi de utilizator pe diverse platforme, cu atât avem mai multe potențiale puncte slabe. Crește suprafața de atac. Dacă aplicațiile respective nu sunt cu update-urile la zi, se agravează situația. Patching-ul și actualizările sunt importante. 

Un smartphone care e out-of-support (nu mai primește update-uri de sistem de operare) reprezintă o vulnerabilitate. Nu doar că sistemul de operare al acestuia nu este la zi cu patch-urile de securitate, dar la un moment dat și aplicațiile instalate rămân în urmă. Cât timp acest software tot rămâne în urmă, se găsesc portițe pentru a exploata vulnerabilitățile lor (noi unelte de hacking etc.). Instalarea de aplicații inutile, de exemplu calculator sau lanternă - orice telefon mobil cat de cat recent are acestea implicit, duce la mărirea riscului. Unele din ele chiar sunt malware/spyware, chiar dacă sunt pe Play Store. 

Trebuie să ținem cont de toate device-urile conectate pe care le avem: telefoane mobile, laptop, PC, console de jocuri video, Smart TV, smart orice, orice chestie din gama IoT (aspirator, frigider, etc). Cu cât avem mai multe device-uri conectate la net, cu atât avem mai multe potențiale puncte slabe. Orice are cameră și se conectează la net trebuie tratat cu atenție. Rețeaua ar trebui segmentată. Camerele de supraveghere trebuie puse în locuri unde nu pun viața privată în pericol și securizate cum trebuie, cu patch la zi, username și parolă greu de ghicit/aflat, etc., altfel uite așa ajungi vedetă porno pe [Shodan](https://www.shodan.io/) și după aia la secțiunea de amatori de pe toate site-urile "picante".

Legat de conturi pe diverse platforme: pe cele mari si bine puse la punct se pot face fără grijă conturi utilizând numărul de telefon și adresa de email "primară" (dacă nu se dorește anonimitate, evident). Pe tot felul de forumuri sau aplicații de hobby-uri (din gama celor găsite pe ceea ce se numește clear web, adică ce vedem în mod normal dintr-un browser obișnuit) se recomandă crearea unui cont cu nume de utilizator diferit de cel real, poză de profil diferită de cea reală (și preferabil să nu se repete între ele), dintr-o adresă de email secundară. Pentru forumurile din dark web (care pot fi accesate doar prin Tor) evident că recomandat e să ai anonimitate, folosind o adresă de email (pseudo)anonimă (care nu cere număr de telefon sau alte date reale la înscriere), nume de utilizator total irelevant și poză de profil lipsă sau irelevantă. 
Ca rezumat: cu cât e mai dubios forumul, cu atât ar trebui să fie mai clar că e cazul să fii anonim. Acum intrebarea ar fi ce să cauți pe așa ceva daca ești om cuminte? De exemplu, pentru a vedea dacă datele tale apar pe undeva, sau pentru a vedea dacă au fost postate poze cu tine (care evident nu le vrei publice). Dar despre astfel de verificări, mai încolo puțin.

Dacă un forum/site (non-guvernamental) îți cere confirmarea datelor cu o poză a unui act de identitate oficial (carte de identitate, pașaport, permis de conducere auto), e absolut clar că e dubioasă treaba. Mai ales dacă nu are de ce să respecte GDPR. Nici un forum/site care nu aparține unei entități a statului nu are de ce să ceară așa ceva, și te pui în pericol dacă le dai. La un moment dat vor fi ori sparți ori luați de autorități, iar datele tale personale vor fi peste tot, în funcție de pe cine au supărat (a se vedea cazul Parler). 

Deci: conturi multe, cu același nume de utilizator (real sau cu legătură cu cel real), legate toate de 1-3 adrese de email ce pot fi legate de o identitate reală, cu poze de profil identice = rău. Chiar dacă nu vrei musai să te ascunzi de cineva, bogăția asta de date înșirate peste tot conduce la extragerea ușoară a și mai multe date despre tine, care în final pot duce la compromiterea unor conturi sau device-uri (de exemplu cu parole puse pe baza datelor de naștere, numele animalelor de companie, hobby-uri). Toate conturile pe care le avem trebuie luate în calcul la threat model, pentru că fiecare din ele și modul în care a fost făcut poate reprezenta o vulnerabilitate.

Pentru accesarea conținutului unor site-uri care insistă să le dai o adresă de email sau pentru descărcarea unor documente care necesită email se poate folosi o adresă de email temporară sau burner (gen TempMail, mailpoof, emailondeck, guerilla mail). Acest lucru te scapă de o grămadă de spam și eventuale mail-uri de phishing. 

Altă mare problemă o reprezintă aplicațiile de chat. Și aici, problemele sunt cam la fel: vrem sau nu anonimitate? De cine trebuie să ne ferim? La ce o folosim mai exact (ce tip de comunicare și cu cine)?

## Cum alegem o aplicație de chat
Agitația recentă cu noua politică Whatsapp a generat o grămadă de discuții și a readus aspectele de securitate/privacy în atenția publicului larg. În esență, au zis că platforma Facebook va avea acces și la (meta)datele din Whatsapp. Și că teoretic nu se aplică în UE. Mai multe despre asta se poate citi direct pe site-ul lor, la partea cu politici de securitate și privacy. Acest lucru are impact mai degrabă asupra algoritmilor publicitari, nu înseamnă că aplicația e musai mai puțin sigură în fața unor atacatori sau a unor interceptări legale. Apropos de interceptări legale, în cazul lor e vorba mai mult despre (pseudo)anonimat, că decriptoare au și autoritățile. Recomand citirea documentației tehnice generale și a politicilor de securitate și privacy pentru aplicațiile folosite/luate în calcul.

Câteva lucruri de luat în considerare la alegerea unei aplicații de chat:
- cu cine dorim să comunicăm, ce fel de date/informații vrem să transmitem
- ce permisiuni necesită din partea sistemului de operare
- ce date necesită pentru utilizare și ce date leagă de tine
- cât și cum stochează aceste date, chiar și după ștergerea contului
- cripare: nu? da? end-to-end? ce algoritm?
- ce setări de privacy oferă
- ce alte vulnerabilități are (de exemplu, tastatura utilizată)

Un rezumat bun e aici: [Secure messaging apps comparison](https://www.securemessagingapps.com/)

"Dar dacă aplicația X e folosită de hackeri/teroristi/etc.?" - Cât timp nu ai treabă cu respectivii, nu ai de ce să-ți faci griji. Cel mult arată că e mai sigură/privată decât altele. Cât timp tu nu ești implicat în activități ilegale, nu te afectează cu nimic dacă un necunoscut care folosește aceeași aplicație comite diverse fapte. Exemplu concret: Facebook cu grupurile de escrocherii/îndoctrinare pentru extremiști diverși, Whatsapp cu grupurile de porno non-consensual sau chiar cu minori, olx cu obiecte furate. 

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

Pentru a folosi [Protonmail](https://protonmail.com/) este necesar un număr de telefon, dar acesta poate fi unul temporar obținut prin aplicații de tip [CoverMe](http://www.coverme.ws/en/index.html), sau un burner (cartelă SIM prepay, cumpărată preferabil cu bani cash, utilizată cu un singur scop într-un telefon care nu are teoretic nici o legătură cu persoana respectivă). [Tutanota](https://tutanota.com/) nu cere nici număr de telefon, nici altă adresă de email. Ambele sunt criptate.

[Status](https://status.im/account-creation/) nu necesită nici număr de telefon, nici adresă de email.

[Telegram](https://telegram.org/) necesită număr de telefon, dar acesta poate fi complet ascuns față de ceilalți participanți la conversație. Nu cere adresă de email și nici setarea unui username, iar numele poate fi schimbat inclusiv într-un emoji.

[Signal](https://signal.org/en/) necesită număr de telefon, nu oferă posibilitatea de a-l ascunde de alții și, mai rău, te anunță când cineva din lista de contacte a aderat. Ce e rău în asta? De exemplu, următoarea situație: persoană cu partener abuziv aderă la Signal pentru a comunica cu familia si avocatul în vederea ieșirii din relație. Partenerul vede notificarea, se enervează (că percepe Signal ca fiind o aplicație folosită de cei care vor să se ascundă cu rea intenție), poate acționa violent față de celălalt și/sau îi poate confisca telefonul, tăind-ui astfel contactul cu cercul de susținere. Alt punct slab al Signal este faptul că pentru tastaturile (virtuale, e vorba de smartphones) folosite pentru caractere non-europene (și aici discuția a fost cu accentul pe chineză și hindi) se poate ignora marcajul de incognito și se pot astfel înregistra mesajele (practic, nu ține cont de "disable personalized learning" și deci stochează cuvintele/frazele folosite des). Este posibil să se întâmple și cu alte tastaturi. Practic, o parte din securitatea acestei aplicații depinde de securitatea tastaturii folosite. 

Alte variante de aplicații de chat sunt [Threema](https://threema.ch/en), [Keybase](https://keybase.io/), [Wire](https://wire.com/en/), [Element](https://element.io/).

Numărul de telefon, adresa de email, precum si o gamă largă de alte date sunt legate de utilizator. Un update recent la Apple App Store a introdus posibilitatea de a vedea ce date sunt legate de tine, per aplicație, și ce date sunt colecționate.

![Date legate de tine, per app](https://i1.wp.com/9to5mac.com/wp-content/uploads/sites/6/2021/01/App-privacy-labels-messaging-apps.png)
sursă foto: Forbes

### Setări de securitate și privacy

Cele mai importante setări sunt:
- autentificarea multi-factor (da, chiar si prin SMS, ca tot e mai bine decât o simplă parolă)
- opțiunea de a dezactiva învățarea personalizată pentru tastatură
- blocarea funcției de screenshot (captură de ecran)
- ascunderea anumitor date față de persoane care nu sunt contacte 

Autentificarea multi-factor (2FA) este utilă oricui. Uneori încetinește treburile (în funcție și de alte setări - la fiecare intrare în cont dintr-un browser nou, se cere al 2-lea factor de autentificare; browser nou se consideră și unul care e setat să nu țină minte nimic, chiar dacă e vorba de același calculator și aceeași rețea), dar poate salva situația dacă parola e compromisă. 
2FA poate fi făcută în mai multe feluri:
- SMS
- PIN 
- smartphone (dacă adversarul are acces fizic la el se complică situația și trebuie crescută securitatea smartphone-ului prin deblocare cu amprentă și/sau model de deblocare complex, sau, mai simplu, folosit altă metodă de 2FA)
- cheie USB securizată, gen [YubiKey](https://www.yubico.com/)

Este recomandat ca 2FA să fie activată peste tot pe unde e posibil. Cea mai ușoară variantă de a face asta este prin SMS, dar nu e cea mai sigură. A doua cea mai ușoară ar fi utilizarea smartphone-ului, fie printr-o aplicație de tip Google Authenticator (sau Blizzard Authenticator pentru jocurile Blizzard) sau confirmare în aplicația corespunzătoare de pe telefon.

Opțiunea de dezactivare/blocare a învățării personalizate pentru tastatură (Incognito keyboard) duce la faptul că tastatura nu mai memorează cuvinte/fraze des folosite. Tastatura le învață pentru a oferi predicții în scopul de a scrie mai repede. Teoretic, și tastatura în sine poate fi trecută în modul incognito, iar datele pot fi șterse, însă acest lucru este destul de dificil și niciodată 100% eficient. De ce contează? Degeaba este aplicația de chat în sine sigură, dacă tastatura reprezintă o vulnerabilitate. Datele colectate de către tastatură pot fi recuperate mai ușor decât conversațiile. Chiar dacă nu reprezintă un set complet de date față de conversațiile în sine, tot se pot extrage o grămadă de informații utile.

Blocarea funcției de screenshot împiedică participanții la conversație să memoreze conversația prin screenshot. Evident că cineva poate poza/filma ecranul cu un alt smartphone sau camera foto, dar e ceva recomandat mai ales în cazul discuțiilor mai sensibile cu persoane care nu sunt musai de încredere și care pot folosi acea conversație împotriva ta. Unele aplicații oferă măcar o avertizare dacă cineva face screenshot. La momentul scrierii acestei pagini nici Facebook Messenger, nici Whatsapp nu oferă posibilitatea de a bloca screenshot-urile sau posibilitatea de a primi o avertizare dacă se face screenshot.

Whatsapp:

Whatsapp nu oferă anonimitate. Este nevoie de un număr de telefon pentru utilizare și nu acceptă numere din aplicații de tip CoverMe. Se poate obține oarecum pseudoanonimitate folosind un SIM burner, nume irelevant și poză de profil lipsă, dar alfarea IP-ului și în final a identității utilizatorului nu este o problemă. Oferă criptare, dar colecționează foarte multe date despre utilizator (pe care le trimite la compania mamă precum și la terți) și nu oferă nici un fel de opțiuni de privacy reale/utile. Nu oferă blocarea screenshot-urilor, nici dezactivarea învățării automate pentru tastatură. Setările de privacy sunt foarte de suprafață și utile doar pentru a te feri de utilizatorul tipic. Nu consider că este recomandat pentru transmiterea de date medicale, contracte, acte sau orice alt fel de date sensibile.

![Whatsapp privacy settings](/images/whatsappprivacy.jpg)

Signal:

Nu oferă anonimitate. Este nevoie de număr de telefon pentru utilizare. Totuși, nu cere nici adresă de email, nici nume "real", numele setat putând fi chiar și un emoji. Se poate obține oarecum pseudoanonimitate folosind un SIM burner, nume irelevant și poză de profil lipsă. O problemă actuală a Signal constă în faptul că acesta te notifică când cineva din lista ta de contacte aderă, acest lucru putând fi chiar periculos în anumite situații. Problema poate fi evitată folosind pentru Signal un număr de telefon necunoscut persoanei de care te ferești, iar cum multe telefoane sunt dual-SIM, acest lucru nu ar trebui să fie prea complicat.

![Signal join notification](/images/signaljoin.jpg)

Session:

Session oferă anonimitate, privacy și criptare. Anonimitatea e oferită prin faptul că nu se cere nici număr de telefon, nici adresă de email pentru a-l folosi. Datorită modelului său descentralizat, este foarte dificil să se facă o legătură între un ID de Session și o adresă IP, care să ducă la un device specific și la identitatea utilizatorului. Se poate alfa din Google Play Store sau Apple App Store cine a descărcat aplicația, dar ID-ul în sine se poate schimba după fiecare conversație.

Această aplicație nu permite screenshot în nici un fel, nici în conversații, nici în meniul principal sau în setări. Oferă incognito keyboard (blocarea învățării personalizate pentru tastatură) și blocarea accesului la aplicație cu modelul de deblocare sau amprenta folosit/ă de Android)

![Session app](/images/sessionapp_privacy_anon.png)

### “Do. Or do not. There is no try.” 

[PinePhone](https://www.pine64.org/pinephone/)/[Bunnie Precursor](https://www.bunniestudios.com/blog/?p=5921) + burner SIM + Tor (sau Brave/DuckDuckGo) + Protonmail/Tutanota (și email temporar în anumite situații) + Telegram/Session/Element + poză de profil lipsă sau irelevantă + nume de utilizator irelevant și care să nu fie repetat pe mai multe conturi + 2FA peste tot + FDE (full disk encryption)

## Cum îmi dau seama dacă parola/datele mele circulă libere pe net?

[Have I been pwned](https://haveibeenpwned.com/)

[Intelligence X](https://intelx.io/)

## "You don't know the power of The Dark Side!": Darknet, deep web - cum se intră, cum te protejezi, ce găsim acolo?

Darknet e acea parte a internetului unde se găsesc tot felul de chestii... mai puțin legale. A accesa și citi nu e propriu-zis ilegal (cu câteva excepții), dar a lua parte activ la anumite comunități și a cumpăra e altceva. Faptul că știi ceva nu înseamnă musai că și practici/folosești :)

2 puncte de plecare în explorarea darknet sunt:

[The Hidden Wiki](https://thehiddenwiki.org/)

[dark.fail](https://dark.fail/)

Darknet-ul propriu-zis e format din site-uri .onion

Adresele cu .onion sunt "hidden services" și e nevoie de [Tor](https://www.torproject.org/) pentru a le accesa. Alte site-uri dubioase fac parte din deepweb și nu sunt indexate de motoarele de căutare. Mai există și unele care sunt indexate, dar tot din categoria asta: paste sites, unele forumuri/pagini de data leaks. O parte din ele sunt indexate și de Google/Bing/Yandex, altele pot fi găsite cu motoare de căutare pentru deep/darknet.

Ca sfaturi de navigare:
- chiar și site-urile non-.onion vor fi accesate numai din Tor
- hotspot din date mobile de pe un SIM burner ar fi ideal
- evită crearea de conturi dacă nu sunt absolut musai necesare pentru a ajunge la informația dorită
- mare atenție cu acumularea de punctaj/currency pe diverse forumuri pentru a obține acces la informații; de obicei acest punctaj poate fi obținut și prin metode pașnice, dar e mai lent
- în cazul creării unui cont, se va folosi o adresă de email temporară sau oferită de un provider ce oferă (pseudo)anonimitate
- nu se va folosi numele real sau porecle/alias-uri cunoscute
- nu se vor folosi poze de profil cunoscute (care sunt folosite și pe alte conturi)
- nu se vor reutiliza parole
- în cazul interacțiunii ulterioare cu persoane întâlnite acolo, se vor folosi conturi (pseudo)anonime și aplicații de chat cât mai sigure
- nu se va descărca (și rula/dezarhiva ulterior) nimic fără a folosi un mediu bine izolat (sandbox sau mașină virtuală - virtual machine, VM)
- dacă sună prea bine pentru a fi adevărat, sigur e țeapă sau honeypot. multe lucruri pot fi honeypot aici, deci atenție

Un site util celor interesați de malware (pentru reverse engineering sau alte studii) e [vx-underground](https://vx-underground.org/)

Două forumuri posibil utile ar fi leakzone.net (data leaks & resources) și raidforums.com (database sharing and marketplace forum). Aici sunt lăsate intenționat fără link, pentru a nu face click pe ele din greșeală :)

Tot data leaks:

https:// ddosecrets. com/wiki/Distributed_Denial_of_Secrets (fără spații)
