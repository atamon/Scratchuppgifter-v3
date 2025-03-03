# Romba

Visst är det tråkigt att damsuga så varför inte försöka koda en egen liten robotdamsugare som kan hjälpa till hemma? 
Det är lättare än vad du tror! 

Börja med att ta bort katt sprajten och klicka sedan på skapa ny sprajt och börja rita din alldeles egen robotdamsugare. Den kan se ut precis så som du vill att den ska se ut! Kanske såhär:
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/dammsugare.png)


Roboten kommer också behöva en yta att damsuga, så klicka därefter på bakgrunder och använd fantasin för att rita upp antingen ditt rum eller kanske din drömlägeneht sedd ifrån ovan.
Viktigt här är att alla väggar är samma färg och att inget annat är målat i samma färg!

Här är ett enkelt exempel på hur det kan se ut: 
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rum.png)


En damsugare är ju inte så användbar om det inte finns smuts så nu måste vi också välja en ny färg som ska vara smuts. Rita ut lite smuts eller damm lite här och var, tänk att det inte har städats på riktigt länge !
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rummedSmuts.png)


Sådär! Nu har vi en riktigt smutsig lägenhet och en robot som vi kan programera att städa upp efter oss! 

## Få roboten att röra på sig!

Det första som vi vill göra är att få roboten att röra sig, börja med att lägga till ett rör dig frammåt block och sätt det till 5 steg. Vi vill också att roboten aldrig ska sluta göra detta så vi lägger också detta blocket i ett för alltid block. 
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörSigFram.png)

Nu rör sig roboten på sig, men den kommer också röra sig genom väggar och inte städa bort någon smuts. Vi behöver koda lite mer. 

Börja med att ta ett kontrollblock, om ... då, och dra ut detta . Klicka därefter på känna av blocken och välj blocket "rör vid färgen", dra in detta i "om" blocket som du tidigare drog ut.

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörVidFärg.png)


Klicka på den färg som finns i känn av färg blocket och använd pippettverktyget för att välja exakt samma färg som väggarna genom att klicka på en av väggarna.

Nu känner roboten av om den åker in i en vägg, men den vet inte vad den ska göra om det här händer! Vi måste skriva lite kod till. Gå till rörelseblocken och välj sväng vänster. Skriv in 36 grader här.

Sådär, lägg in rör dig frammåt blocket i annars biten av om blocket så att det ser ut något såhär: 
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörelseKlar.png)


Om allt har gått bra har vi nu en robot som rör sig runt i rummet vi ritade i början, men ingenting damsugs! Vi behöver koda lite till.

## Damsugare

För den här biten kommer vi behöva lägga till en grupp specialblock. Nere i vänstra hörnet hittar vi en knapp som ser ut såhär 

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/laggtillBlock.png)

Klickar vi på den kommer vi till en sida där vi kan lägga till massor med olika tillägg, men just den här gången vill vi lägga till Pennan så vi klickar på den ruta som ser ut såhär 

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/pennaBlock.png)

Sådär! Nu kan vi hitta våra pen-block längst ner under våra vanliga block. 

Det första vi måste göra är att sätta pennan till den storlek som vi vill ha. Detta gör vi innan vårt för alltid block. Beroende på hur stor eller liten din robot är så kommer du kanske behöva skriva in en annan siffra här men i mitt fall passar 30 väldigt bra. Det viktigaste är att pennan är mindre än vad din robotdamsugare är!

Vi sätter också pennan till samma färg som golvet genom att dra ut ett "sätt färg till" block. Välj golvfärgen på samma sätt som vi valde färgen för väggen!

Eftersom vi inte heller vill dammsuga innan vi är ovanför smuts så sätter vi också ut blocket "Penna upp" i vårt "om då" block precis innan "rör dig frammåt" blocket.

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/damsugarConfig.PNG)



Sådär! Nu är vi redo att koda själva städandet!

Inne i vår för alltid loop lägger vi nu till ytterligare ett om block precis under vårt penna upp block. Vi anväder samma känn av färg block som vi använde för att känna av väggarna, men istället för färgen på väggarna väljer vi nu färgen vi valde på smutsen!

Inne i det här blocket lägger vi in ett penna ner block och med det är vi klara! Scriptet borde nu se ut någo sådanthär:

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/damsugOmFärg.PNG)

Sätt ihop den här biten kod med resten för att få en bit kod som ser ut såhär:


![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/slutresultat.PNG)

Vi kan nu köra det och se hur roboten damsuger upp smutsen vi ritade ut! 


## Fortsättning (Fler alternativ i framtiden)
Kanske finns det något i hemmet som roboten behöver undvika? Kanske finns det något husdjur eller liknande som roboten måste kunna undvika. 

### Koda ett litet husdjur 
Börja med att rita ett husdjur eller välj en sprajt som du tycker skulle vara rolig att ha som ett husdjur!

Vi kodar husdjuret på samma sätt som vi kodade damsugaren börja med att lägga till ett rör dig frammåt block och sätta det till 5 steg. Vi vill också att roboten ska sluta göra detta så vi lägger också detta blocket i ett för alltid block. 
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörSigFram.png)


Ta också ett kontrollblock, om ... då, och dra ut detta . Klicka därefter på känna av blocken och välj blocket "rör vid färgen", dra in detta i "om" blocket som du tidigare drog ut.

![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörVidFärg.png)


Klicka på den färg som finns i känn av färg blocket och använd pippettverktyget för att välja exakt samma färg som väggarna genom att klicka på en av väggarna.

Nu känner husdjuret av om den åker in i en vägg! Nu vehöver vi bara ett till rörelseblock, välj sväng vänster och skriv in 36 grader här.

Sådär, lägg in rör dig frammåt blocket i annars biten av om blocket så att det ser ut något såhär: 
![alt text](https://github.com/Kodcentrum/Scratchuppgifter-v3/blob/master/Robot_ai_block/rörelseKlar.png)


Nu har vi ett hudjur som rör sig runt i rummet!

## Få damsugaren att undvika husdjuret
Beroende på om du har ritat en egen sprajt eller tagit en som redan är färdig så kanske din damsugare redan kommer akta sig för ditt husdjur. Om det till exempel har samma färg som dina väggare eller en kontur med samma färg så kommer din robotdamsugare akta sig när den kommer nära!

Men om det inte är så kan vi programmera lite till för att få damsugaren att akta sig för husdjuret. 

Vi tar ett till om block och placerar det innan om blocket som kollar efter väggarna. I detta blocket sätter vi precis som med väggarna ett sväng vänster/höger block med 36 grader. 

För att få damsugaren att vända även när den stöter på sprajten tar vi ett rör vid block och väljer vår nya sprajt i listan. Detta blocket placerar vi sen i om-blocket. Sådär! Damsugaren undviker nu också katten som springer runt i lägenheten!

### Saker att arbeta vidare på
Kan du göra så att roboten skiljer på fler saker? Kanske finns det en viss smuts som den inte ska damsuga upp utan istället hälla vatten på? 

Går det att få roboten att röra sig på annat sätt?


