# Programmering
##  Lathund för JavaScript och grundläggande programmering
PS. I kodexemplerna nedan menas ``` >>``` att det efter dessa tecknerna är det som koden på raden ovan get som output

<table>
    <tr>
        <th><a href="#JS">JavaScript</a></th>
        <th><a href="#K">Komentarer</a></th>
        <th><a href="#SN">Sträng / Nummer </a></th>
        <th><a href="#V">Variabler</a></th>
        <th><a href="#L">Loggar</a></th>
        <th><a href="#F">Funktioner</a></th>
        <th><a href="#IE">If-else satser</a></th>
        <th><a href="#UPG">Uppgifter</a></th>
    </tr>
</table>

1. <span id="JS">__JavaScript__</span>
    * Programeringsspråk som är gjort för HTML och Webbläsaren
    * Lätt att lära sig - ett bra programmeringsspråk att börja med <br>
     __Regler__: 
     * Varje rad avslutats med ett ; för att visa programmet att det är en ny rad
     * Programmet ignorerar extra mellanslag / nyrad  (Fler än ett)

1. <span id="K">__Komentarer__ </span>
    * Komentarer är till för att du som programmerare ska kunna dokumentera din kod eller komma ihåg vad koden gör
    * Programmet kommer ignorera detta, så skriv på hur mycket du vill <br>
    __Regler__: 
     * För snyggt gränssnitt, använd /**/ metoden endast vid flera raders kommentarer & // endast vid enradskomentarer
    * Kod:
    ```javascript
    //Detta är en komentar
    
    /*
    Om du vill markera flera rader kan du även göra det. 
    Din kommentar slutar inte förens tecknet nedan:
     */
    ```
1. <span id="SN">__Sträng / Nummer__</span>
    * I JavaScript är det uppdelat i strängar och nummer 
    * En sträng  måste alltid vara inneslutet av '' och består oftast av en eller flera bokstäver
    * Ett nummer eller en uträkning kräver inga '' runt sig
    * En ekvation kan vara en sträng, men då räknar programmet ej ut ekvationen utan skriver ut den precis som det står <br>
    __Regler__: 
     * Både "" och '' räknas som kommentarsomslutare men håll dig till en av dem! (Rekomenderat '')
    * Kod:
    ```javascript
    'En sträng'
    //Sträng

    1
    //Nummer

    '1+3 nummer i sträng fungerar'
    //Sträng, fastän det är nummer i 

    1+3
    //Nummer

    '1+4'
    //Sträng fastän det inte finns några boksträver i den - '' gör det till en sträng
    ```

1. <span id="V">__Variabler__</span>
    * En variabel lagrar ett värde inom sig
    * Detta värde kan t.ex vara ett tal, en sträng eller en funktion
    * Värdet går att ändra under programmets olika delar / faser
    * Det finns olika typer av variabler, de vanligaste är:
        * Nummer
        * Text 
        * Lista
        * Objekt
    * Består av : namn på variabel och tilldelningsvärdet <br>
    __Regler__: 
     * Variabelnamn skrivs med liten bokstav i början, vid flera ord skrivs första bokstav i de andra orden som stor bokstav. (Ex. variabelnsNamn)
    * Kod:
    ```javascript
    var hansNamn = 'Samuel';
    //Tilldelar variabel kallad 'hansNamn' värdet 'Samuel'

    hansNamn = 'Johan';
    //Ändrar variabeln 'hansNamn's värde till 'Johan'

    var x = 0;
    //Sätter variabeln x till värdet 0

    var y = 2*x;
    //Sätter variabeln y till 2 gånger värdet på variabeln x (dvs. y = 2x0 = 0)
    ```

1. <span id="L">__Loggar__</span>
    * Loggar är till för att du ska kunna skriva ut saker till dig själv. 
    * Dessa kommer synas i 'console' som finns i CodePen
    * I loggen kan du skriva ut  : variabler, strängar, ekvationer, nummer mm. (Olika typer)
    * Det går att kombinera de olika typerna ovan genom att sätta + mellan dem <br>
    __Regler__: 
     * Används gränssnittet (mellanslag på de ställerna) som finns på sista loggen
    * Kod:
    ```javascript
    var x = 0;
    console.log(x);
        >>0

    console.log('Hey, what´s up');
        >>'Hey, what´s up'

    console.log(5)
        >>5

    console.log(4*2);
        >>8
    
    console.log(4+2 + 'Sträng' + x);
        >>'6Sträng0'

    ```

1. <span id="F">__Funktioner__</span>
    * En funktion är en "maskin" som tar in ett data och spottar ut en annan (Ex. f(x) = 2x+2)
    * Inom programmering används det mycket för att strukturera & slippa upprepa samma kod flera ggr.
    * Exempel : Lägger in heltalen X & Y och får ut det störta talet - det minsta
    * Består av : funktionsnamn, indata, beräkningar / flöde inuti funktionen, retunerar utdata värde (typ av slutsats) <br>
    __Regler__: 
     * Skriv funktionernas namn på samma sätt som variabel namn (se variabel avsnitt)
     * Använd samma upplägg (med mellanslag / nyrad) som funktionen "nameOnFunction" nedan - ökar läsligheten / ser proffsigt ut
    * Kod:
    ```javascript
    function nameOnFunction (input) {

    }
    //Skapar en funktion med namnet "nameOnFunction" och som skickar in varibeln "input"
    // Funktionens flöde (där uträknangar görs) är mellan {  flöde  }

    function nameOnFunction (input) {
        return input*2;
    }
    // Denna funktion kommer retunera / skicka ut värdet vi skickar in x2

    nameOnFunction(3);
    //Tillkallar funktionen "nameOfFunction" och skickar med 3 som indata.
        >>6

    x = nameOnFunction(3);
    //Sätter variabeln "x" till värdet som funktionen "nameOfFunction" retunerar vid indatat 3
        >>x = 6

    function multiply (number1, number2) { return number1*number2 }
    // Även detta är en funktion fast med två argument värden och inga nya rader - FULT SKRIVET, ANVÄND NYRAD

    ```

1. <span id="IE">__If-else satser__</span>
    * Används för att göra jämförelser mellan två värden
    * Jämförelserna retunerar alltid sant eller falskt
    * Teckan som används : ==, !=, <, > <br>
    __Regler__:
     * Skriv alltid mellanrum mellan tecknet och jämförelse (ex. 1 == 1)
    * Kod:
    ```javascript
    if(1 == 1) {
        console.log("stämmer")
    }
    >>"stämmer"
    // Kollar om 1 är samma sak som 1, vilket det är, så det mellan måsvingarna till if-satsen görs

    if(1 == 2) {
        console.log("sant")
    }else {
        console.log("falskt")
    }
    >>"falskt"
    // Kollar om 1 är samma sak som 2, vilket det inte är. Går därmed in i else-satsen (delen) och falskt skrivs ut

    var z = 1
    if(z == 1) {
        console.log("sant")
    }
    >>"sant"
    // Sätter variabeln z till 1 & kommar om z är lika med ett, vilket det är. Loggar därmed "sant"

    // Gämförelser
    if(1 > 0)
    // Kollar om 1 är större än 0
    if(1 < 0)
    // Kollar om 1 är mindre än 0
    if(1 != 0)
    // Kollar om 1 INTE är lika med 0

    ```



## UPPGIFTER 
1. <span id="UPG">__Cookie clicker__</span>

    * JavaScript kod:
    ```javascript
    var cookies = 0;
    var cookiesPerClick = 1;
    
    function collectCookie() {
        cookies = cookies + cookiesPerClick;
        document.getElementById("cookies").textContent = cookies+"st cookies";
    }

    function upgrade() {
        if(cookies >= (20 * cookiesPerClick)) {
            cookies = cookies - (20 * cookiesPerClick);
            cookiesPerClick = cookiesPerClick + 1;
            document.getElementById("cookies").textContent = cookies+"st cookies";
            document.getElementById("upgradeCost").textContent = "Uppgradering: "+ 20 * cookiesPerClick;
        }else {
          alert("Ej råd! du behöver: "+(20 * cookiesPerClick))
        }
    }
    ```
    
    ```html
    <button onclick="collectCookie()">Click me</button>
    <button onclick="upgrade()">Upgrade</button>
    <h2 id="upgradeCost">Uppgradering: 20</h2>
    <h1 id="cookies"></h1>
    ```
    <br>


__Saker att lägga till - Exempel__
* CSS
    ```css
    html {
        background: red; /* Ändra bakgrundens färg*/
        color: red; /* Ändra textens färg*/
    }
    /* Ps. går att byta ut "red" mot valfri färg */
    button {
        width: 100px; /* Gör knappen 100 pixlar bred, fler pixlar ger bredare knapp*/

        height: 100px; /* Gör knappen 100 pixlar hög, fler pixlar ger högre knapp*/

        border-radius: 50%; /* Gör knappen helt runt, mindre procent gör den mindre rund*/

        background: red; /* Ändra bakgrundens färg*/

        font-size: 10pt; /* Ändrar text-storlek, öka värdet för större text*/

        border: 2px solid blue; /* Skapar en 2 pixlars blå ram runt hela knappen, ändra gärna färg och antal pixlar*/
    }

    button:hover {
        tranform:rotate(180deg); /* Roterar knappen 180 grader när man har musen över den*/

        transform:scale(1.1); /* Gör knappen 10% större när man har musen över den*/
    }

    button:active {
        tranform:rotate(180deg); /* Roterar knappen 180 grader när man trycker på den*/

        transform:scale(1.1); /* Gör knappen 10% större när man trycker på den*/

        background: red; /* Gör knappens bakgrund röd när man trycker på den*/
    }
    ```
    Ps. Hitta fler roliga CSS tricks på länk nedan: <br>
    [CSS - W3 Schools](https://www.w3schools.com/css/)
    <br>
* HTML
    ```html
    <img onclick="collectCookie()" src="http://www.pngall.com/wp-content/uploads/2016/07/Cookie-Download-PNG.png%22%3E"> <!-- byt ut detta mot knappen för att få en bild på en kaka  -->

    <h1></h1> <!-- Lägg till titlar, finns h1 - h6 beroende på storlek -->
    <p></p> <!-- Lägg till brödtext, finns även <b></b> & <i></i> för fetstil respektive italic
    ```
    <br>
* JavaScript <br>
    * Autoclicker: 
    ```javascript
    var autoPerClick = 1; // Antal kakor per klick
    var autoTime = 1000; // Tiden mellan klicken i millisekunder. 1000 millisek = 1 sekund
    setInterval(function { cookies = cookies + autoPerClick }, autoTime) // Skapar ett interval som ökar "cookies" med autoPerClick varje sekund
    ```
    Utvecklar mer?
        + Lägg till så att man även kan uppgradera både antal kakor per klick & tiden mellan klicken  <br> <br>
    * Nivå: <br>
    Ändra om funktionen "collectCookie" till att kolla om nästa nivå är uppfylld
    ```javascript
    var level = 0;
    function collectCookie() {
        cookies = cookies + cookiesPerClick;
        document.getElementById("cookies").textContent = cookies+"st cookies";
        if(cookies > 100) { // Om du har över 100 kakor blir din nivå 1
            level = 1;
        }
        if(cookies > 1000) { // Om du har över 1 000 kakor blir din nivå 2
            level = 2;
        }
        if(cookies > 10000) { // Om du har över 10 000 kakor blir din nivå 3
            level = 3;
        }
    }
    ```
    Utvecklar mer?
        + Lägg gärna till fler nivåer
        + Ändra så att nivån beror på hur många kakor per klick du har
## Snötema
* https://matteraknaren.com/course/snow.scss
https://matteraknaren.com/course/snow.js
