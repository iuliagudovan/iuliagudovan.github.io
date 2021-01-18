### Salut!

Această pagină are ca scop aducerea în atenția publicului larg a unor noțiuni de securitate și privacy în mediul virtual.
Nu o sa folosesc "intimitate" în loc de "privacy" pentru ca lumea o sa se gandeasca la alte chestii si nu e tot timpul cazul ;)


## Securitate si privacy - de ce ar trebui sa te intereseze ambele

Faptul ca ceva e sigur nu inseamna musai si ca ofera privacy, iar faptul ca ceva ofera privacy nu inseamna ca e si sigur.
Noțiunea de privacy se poate referi la privacy versus marii colectori de date (Facebook, Google, Yandex, tot felul de scraper-e), versus autorități (cum se spune, "agențiile cu acronime din 3 litere") sau versus alte persoane fizice.
Una e să fentezi algoritmii publicitari ai Facebook, alta e să te ascunzi de un regim opresiv ca dizident/opoziție, și complet alta e să nu afle rudele că joci Dungeons & Dragons. Sau sa nu afle hoții că ai plecat în concediu și stai mult :) Alt caz demn de menționat ar fi victimele (de orice gen) violenței domestice. Persoanele cu parteneri abuzivi (zic la masculin ca sa fie mai general, nu e problema de gen aici) au nevoi mai complexe de privacy, mai ales daca au de gand sa iasa din relatie sau au fugit deja de acasa. E cam ca la protecția martorilor.

Când ne gândim la privacy, trebuie să avem în vedere următoarele:
1. Trackers:
- Google Firebase Analytics
- Microsoft Appcenter Crashes
- Countly
- Bugsnag
- Piwik
2. Metadate de toate felurile (istoric de navigare web, timp petrecut pe un site, reclame accesate, obiecte pe care a stat cu mouse-u etc., date EXIF în cazul imaginilor). Toate acestea pot da informații cu privire la interesele și preferințele utilizatorului fără a accesa efectiv date de identificare ale acestuia
3. Date de localizare (în toate formele)
4. Cookies
5. Postări pe social media sau alte tipuri de platforme: bineinteles, se pot posta diverse pe social media / net în general, la public, cu asumarea de către autor că, o dată ce a fost postat cu setarea "public", acel conținut poate fi accesat si salvat / arhivat de oricine. La fel și în cazul comunicării printr-o aplicație care nu oferă criptare end-to-end și care permite screenshot (captură de ecran) în conversații.

Securitatea trebuie privita tot timpul in raport cu ceva. Suprafețele de atac sunt multe, iar threat model-urile și mai multe, după cum am menționat mai sus. De aceea, la alegerea telefoanelor, laptop-urilor și aplicațiilor utilizate, trebuie avut în vedere un threat model realist pentru persoana care le va folosi.


## Threat model - ce-i ăla și de ce ar trebui să ne gândim la el

Un threat model este practic un model de amenințare. "Ce tip de adversar am?"
Problema la ora actuală e cam așa: date strâng toți, log-uri țin toți, iar din punct de vedere al "mă va da pe mâna poliției/partidului" toți o vor face cu un mandat în față.

"Aoleo! Hackeri!". Da, corect. Însă și aici intervin unele deosebiri. Să luăm câteva cazuri super simplificate:
- elevi pusi pe glume proaste / răzbunări legate de jocuri video: aptitudini de bază, uneori nu stiu să se ferească, în general pot fi prinși ușor și dacă sunt conștienți de asta nu vor face mari pagube. Ușor de fentat cu o parolă bună la WiFi și un nume de rețea (SSID) care să nu îi incite, firewall, antivirus și atenția de a nu face click pe toate link-urile dubioase trimise pe diverse aplicații de chat
- skids: denumirea vine de la "script kiddies". Persoane care folosesc programe/script-uri gata făcute de alții și nu își dezvoltă propriile unelte. Gradul de periculozitate depinde de mai mulți factori, însă pot fi fentați cu un minim de măsuri de securitate
- scammers: clasicul "Ați câștigat o mașină/bani/etc.! Vă rugăm dați-ne numărul cardului, numele posesorului, data de expirare și CVV-ul pentru a intra în posesia premiului". "Fiul dumneavoastră a accidentat grav un pieton". Și alte asemenea. Ușor de fentat prin a cunoaște pe ce lume trăiești și prin a nu le da nici un fel de date. Phishing tot aici intră
- dragoste și trădare! : aici e grav. În categoria asta intră foști, parteneri abuzivi, parteneri geloși, toata gama. Pot fi orice de la nivel de skid la nivel de APT, doar că au cea mai crâncenă motivație să ți-o coacă. Dacă persoana mai are și aptitudini avansate în domeniul calculatoarelor și al telecomunicațiilor, deja e chiar grav, practic ai un APT care are o problemă personală cu tine
- APT: Advanced Persistent Threat. Entitate cu capabilități avansate, care obține acces ilegal la un sistem și își stabilește o prezență pe termen lung în acesta. De obicei sunt grupuri cu finanțare puternică în spate, și/sau susținute politic (la nivel de stat). Foarte puțin probabil ca o persoană fizică să aibe de-a face cu așa ceva. De obicei iau în vizor companii, entități industriale, elemente de infrastructură critică, instituții de stat, cu scopuri diverse: colectare de date sensibile/secrete, sabotaj, furt de proprietate intelectuală (putin mai pe larg aici: https://www.imperva.com/learn/application-security/apt-advanced-persistent-threat/ )

### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/iuliagudovan/pisicainvizibila.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
