# Bug Race (tillägg)

Om du redan har skapat spelet Bug Race - Intro så har du ett spel där du styr en skalbagge som springer runt en bana. Målet med spelet är att undvika att hamna utanför banan, då blir det Game Over. Men hur vinner du i spelet? Och hur kan man lägga till fler spelare och ändra banor? Dax att utveckla spelet vidare. Här finns förslag på hur du bygger olika tillägg. Välj en eller flera - eller hitta på egna! 

![Bug race med två spelare](image_2.png)

> **HUR KODAR JAG?** 
</br>
Följ denna instruktion steg för steg och koda ditt projekt i verktyget Scratch. <a href="https://scratch.mit.edu" target="_blank"> Klicka här för att öppna Scratch i en ny flik.</a> Se till öppna ditt projekt Bug Race - Intro och koda vidare på det. Du kan behöva titta tillbaka i instruktionen för [Bug Race (intro)](bug-race-intro) om du har glömt hur du kodade vissa skript.
</br>

  Då börjar vi utveckla spelet!

## 1: Mållinje för att vinna spelet

För att kunna vinna spelet behöver du en mållinje för banan och ett skript som säger att du vinner spelet när skalbaggen rör vid mållinjen. Det liknar det skript du redan skapat i ditt Bug Race-spel, som styr hur spelet blir Game Over när skalbaggen rör vid det gröna gräset. Gör såhär för att koda mållinjen:

1.  Börja med att rita en mållinje där du vill ha den, förslagsvis strax bakom skalbaggens startposition.

  ![Bild på Bug race](image_0.jpg)

2. Skapa nu ett VILLKOR för skalbaggen som säger: **om** skalbaggen rör vid färgen gul (eller din mållinjes färg), **då** vinner man spelet. (Tips: Om du inte kommer på hur du ska koda detta, kan du kika på skript du har kodat som styr Game Over.)

3. Vad ska hända **om** skalbaggen rör vid mållinjen? Den kan till exempel säga "Mål!" eller "Grattis!"
Lägg till **"stoppa detta skript"** för att avsluta spelet.

4. Lägg det nya i din **för alltid**-loop. Så här kan det se ut:

  ![För alltid loop](image_1.png)
  
Nu har du skapat skriptet för mållinjen.
På nästa sida kan du lägga till fler spelare.


## 2: Flera spelare

Nu har du ett spel för en spelare. Men det kan vara roligt att spela flera – eller spela med två händer! Om banan är tillräckligt bred kan du lägga till en skalbagge eller något annat djur och låta dem tävla mot varandra om vem som kommer först i mål.

![Bug race med två spelare](image_2.png)

1.  Börja med att lägga till en ny sprajt. Välj fritt i biblioteket eller KOPIERA skalbaggens sprajt om du vill att två skalbaggar tävlar mot varandra. Ändra storlek så att båda får plats på banan.

2. Om du har en ny sprajt som inte är kopia på den första, kan du kopiera koden för skalbaggen. På så sätt behöver du inte skapa samma skript en gång till. Du kopierar genom dra hela skriptet till den nya sprajten.  Nu gör båda sprajtar samma sak!

3. Du behöver ändra skripten för att styra sprajten så att inte båda ska styras med vänster- och högerpil. Välj i rullistan för **"när _ trycks ned"**, till exempel tangenterna A och D.

4. Du kanske märker att din nya sprajt startar på samma ställe som skalbaggen? Du behöver ändra startposition. Flytta sprajten dit du vill att den ska stå. Du hittar sprajtens koordinater i sprajtens informationsruta, markera sprajten och tryck på "i". Ändra värden för **"gå till x: y:"**.

  ![Sprajtar](image_4.png)

> Testa spelet! Nu kan du styra båda sprajtar. Men vad händer när en av dem hamnar utanför banan?

5. Om du vill kunna tävla om vem som kommer först i mål, kan det inte bli Game Over när en spelare hamnar utanför banan. Istället kan du t ex välja att sprajtarna säger "Aj!" och hamnar tillbaka på sin startposition. Så här kan det se ut då:

  ![Skript för att starta om](image_5.png)

> Testa spelet! Om det buggar och någon sprajt säger "Mål!" för tidigt kan det bero på att färgen gult finns i den nya sprajten. Testa att ändra färg då.

nu har du kodat in fler spelare.
På nästa sida kan du ändra banan till en labyrint.

## 3: Ändra banan till en labyrint

Eftersom skriptet för sprajtarna bara känner av om de rör sig på grön färg, och inte hur själva banan ser ut, är det enkelt att byta ut banan. Du kan till exempel göra en labyrint som bakgrund istället.

![Bugrace som en labyrint](image_6.png)

1. Tryck på din SCEN och gå till fliken för BAKGRUNDER. Välj **Rita ny bakgrund**.

2. Fyll först med samma gröna färg som i din första bakgrund. Du kan välja färg med färgväljaren som finns till höger om färgrutorna, tryck på den och sedan på den gröna färgen i din första bakgrund.

  ![Färgväljaren](image_7.png)

3. Gör en labyrint genom att dra upp flera vita rektanglar på den gröna bakgrunden, eller rita själv med penseln. Tänk på att banan behöver vara tillräckligt bred för att kunna spela!

4. Rita en gul mållinje i slutet av labyrinten. Tänk på att använda samma gula färg som till mållinjen du ritade i Tillägg 1. Om du inte vill ha en mållinje kan du istället rita gula bananer eller något annat som spelaren ska nå fram till.

> Tips: Gör flera olika bakgrunder och se vilka som är roliga att spela med!

Nu har du skapat ny bana.
På nästa sida kan du skapa mjukare styrning när sprajtarna svänger.

## 4: Mjukare styrning

Du har kanske märkt att det kan vara svårt att styra sprajten när du spelar. Varje tryckning vrider den ett visst antal grader,
men om du håller inne händer ingenting - förrän efter en liten stund. Då börjar den snurra jättefort!

Den här "ketchupeffekten" kan man se när man skriver text också. Testa i en ruta där du kan skriva text, som till
exempel längst upp i internet-browsern där Scratch är öppet. Om du trycker ner "a" på tangentbordet kommer först ett a,
sedan ingenting - och sedan en hel rad, jättesnabbt.

För varje "bokstav" som datorn får inskickad, kommer Händelsen "När [a] trycks in" att skickas, och det lilla skriptet
som vrider sprajten blir utfört. Det är därifrån "ketchupeffekten" kommer.

![Hur sprajten styrts hittills](old_turning.png)

Men det finns andra sätt för Scratch att läsa av tangentbordet. Under "Känna av" finns ett villkor som heter
"tangent [mellanslag] nedtryckt?".

![Ett villkor som läser av tangentbordet](keypress.png)

Det kan man använda i ett "Om"-block (som man kan hämta från fliken "Kontroll")
för att få sprajten att vrida sig lite grann när en viss knapp är nedtryckt (man kan ändra [Mellanslag] till vilken
tangent som helst).

![Ett "om"-block med tangentbordsvillkor i](if_turning.png)

Var ska man placera "Om"-blocket, då? Tja, om man lägger det på samma ställe som flyttar sprajten framåt hela tiden,
så kommer den vrida sig lite grann för varje steg framåt, om knappen man valt är nedtryckt. Då får man en mjuk sväng.

Prova olika värden för hur många grader den ska vrida sig! Och glöm inte att ta bort de de andra skripten som vrider
på sprajten!

## Färdig!
Grattis, nu har du gjort klart uppgiften.

**Glöm inte att spara ditt projekt!** Döp det gärna till uppgiftens namn så att du enkelt kan hitta den igen.

> **Testa ditt projekt**  
Visa gärna någon det som du har gjort och låt dem testa. Tryck på **dela** för att andra ska kunna hitta spelet på Scratch. Gå ut till projektsidan och låt någon annan testa spelet!

## Utmaning
Har du tid över? Här kommer en utmaning för dig som vill fortsätta:

### Flera banor
Kan du skapa skript som **byter scenens bakgrund** när en spelare kommer i mål – så att spelet består av flera banor?

## Frågeställningar

* Hur kan du kopiera kod i Scratch?

* Vad kan du behöva tänka på när du kopierar kod mellan olika sprajter?
