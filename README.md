# Blog

dit is mijn blog blablabla introtekst later meer toevoegen

## Gastspreker 1 Killian Valkhof - 7-2-2024

“Choose the least powerful language suitable for a given purpose”

Probeer componenten in html en css te maken zodat de browser al het werk voor je doet. Hierdoor runt je website veel sneller en werkt hij ook als de JavaScript het niet meer doet.

**Custom checkbox**

Focus-visible kan je gebruiken voor focus interacties zonder de muis. Focus is alleen met muis

Niet outline: none; gebruiken. Hiermee haal je de outline weg. In plaats daarvan gebruik je outline-color: transparent;. Hierdoor is de outline er nog, maar je ziet hem niet. Als je dit doet kunnen gebruikers die hoog contrast modus gebruiken nog wel de outline zien als ze dat willen.

**Colorpicker in de browser**

Je kan een color picker maken in html met <input type=”color”>.

Met color-scheme kan je wisselen naar dark- of lightmode. Het kan ook op basis van welke modus de gebruiker heeft in de browser.

**In-page transitions**

Vroeger moest je jQuery gebruiken om een smooth scroll te maken. Dit vergde veel JavaScript code. Tegenwoordig kan je in css scroll-behavior: smooth; gebruiken om dit in één regel te doen. Hiermee doe je het via de browser. Het is beter, sneller en je kan easing curves gebruiken.

Als het gaat om toegankelijkheid wil je deze smooth scroll wel uitzetten voor mensen met motion sickness. Zorg ervoor dat je standaard de smooth scroll uitzet en als je gebruiker een optie heeft om ‘reduce motion’ aan of uit te zetten. Daarna kan je hem aan of uit zetten op basis van of die optie is gecheckt of niet.

Met position: sticky; kan je heel bewust elementen vast laten zetten op een bepaald gedeelte in het scherm terwijl je blijft scrollen.

**Carousels**

scroll-snap-\*. Hiermee kan je elementen laten snappen (in het engels). Dus als je een lijst van afbeeldingen naast elkaar hebt, kan je 1 afbeelding perfect laten snappen in het midden.

[youtu.be/34zxWFLCDlc](http://youtu.be/34zxWFLCDlc) of [youtu.be/34zxWFLCDIc](http://youtu.be/34zxWFLCDIc) volgens mij is de link kapot 🤢

**Details en summary**

Hiermee kan je elementen open en dicht laten klappen. Met de marker pseudo class kan je het default driehoekje veranderen. Je kan de marker ook veranderen als hij open is. Met een hover erbij kan je duidelijk maken dat het een interactief element is.

**Dialog**

Nieuw element in html om gebruikers keuzes te laten geven. Je kan dit vervangen door een alert, want een alert zorgt ervoor dat al je JavaScript wordt uitgeschakeld. Als je een dialog activeert, komt het tevoorschijn op de toplayer. Dit is voor ALLES. De toplayer is een laag boven de pagina.

Een <dialog> moet je wel alles zelf maken. Een sluitknop staat er bijvoorbeeld niet standaard op. Die moet je allemaal zelf erin zetten. Hetzelfde geld voor positionering en andere styling. Je kan de achtergrond ook stylen met backdrop-filter. Hiermee kan je de achtergrond blurren, donkerder maken etc.

**Container queries**

Container queriues zijn net als mediaqueries, maar ze kijken naar de breedte van de container waar het element in zit inplaats van de hele pagina.

**:has() selector**

Je kan hiermee checken of iets is aangevinkt bijvoorbeeld. Als het is aangevinkt doet het iets. Het is een soort van if else statement van JS in CSS. Meer hier te lezen: https://polypane.app/where-is-has/

**Stop using JS in the future…**

Dit zijn een aantal features die nog niet helemaal klaar zijn, maar in de toekomst hopelijk overal supported is.

-   Met field-sizing kan je een input of textarea breder/groter maken op basis van de hoeveelheid tekst.
-   Met grid-template-rows: masonry; kan je een grid maken kan je een grid maken en elementen automatisch laten vullen. Je kan zien hoe het wordt gebruikt op de Pinterest website.
-   Met <selectlist> kan je alles aanpassen aan een dropdown menu. Je kan bij wijze van zelf een grid maken als het de selectlist open klapt.
-   Scroll driven animations. Hiermee kan je zonder JavaScript dingen laten doen op basis van de scroll positie. Je kan dus rechtsboven scrollen, en linksonder iets laten animeren.

Korte reflectie:

Het eerste wat ik dacht na deze lezing was: “holy shit!”. Ik hoorde hiervoor al dat developers heel graag naar een conferentie willen gaan waar Killian spreekt, en ik begrijp dat nu volledig. Ik vond de informatie die hij met ons deelde extreem waardevol en ook een hele goede boodschap.

Het idee van de lezing was om technieken te laten zien die heel veel mensen in JavaScript doen, maar dat je die heel goed ook in HTML en CSS kan doen. De reden waarom je niet zo snel JS in wil springen is omdat je site meer moet laden als je JS gebruikt. Met een paar functies zal dat niet een groot probleem zijn, maar hoe groter je project wordt en hoe meer JS je toevoegd, kan het zeker oplopen tot een tragere website. Daarom is het een goede standaard om alles wat je kan doen in CSS ook echt daadwerkelijk in CSS te doen. De ironie van deze lezing is natuurlijk dat ik nog veel wil leren in JS, dus op een bepaalde manier is het niet handig voor mij om nòg minder JS te gebruiken ;). Maar zonder grapjes, dit was een extreem waardevolle lezing en je merkt gelijk dat Killian weet waar hij het over heeft en enorm veel passie heeft voor web development.

De twee technieken die mij het meest opvielen waren de dialogs en :has() selectors. De dialog sprak me aan want ik had geen idee dat dit mogelijk was zonder JS. Ik wist wel van een alert af, maar ik had geen idee dat je dus in principe je eigen alert kan maken en die stylen op de manier hoe jij wil. De :has() selector was ook verbazend voor mij. Hoe ik het begreep kan je dus checken of een element iets heeft en op basis daarvan iets laten gebeuren. Dat klinkt verdacht veel als een if else statement… Ik moet zelf nog meer researchen voor deze selector, maar dit lijkt me echt een enorm handige feature om te gebruiken.

Dus in conclusie, een enorm waardevolle lezing waar ik zeker wat aan heb gehad. Ondanks dat het wat uitliep en mijn concentratie aan het eind een beetje verloor, was het zeker een lezing die ik niet snel zal vergeten!

## Gastspreker 2 Fenna de Wilde - 14-2-2024

Creative frontend designer

**Toegankelijkheid**

Niemand in bedrijven geeft om toegankelijkheid, ookal is het heel belangrijk.

Dingen om altijd toe te passen:

-   focus state
-   aria attr
-   toegankelijke carrousel
-   focus guards

**Focus state**

Met een focusstate kan je je website laten gebruiken door mensen die geen muis gebruiken. Met focus-visible registreerd alleen als je met tab iets selecteert.

Je kan een globale focus styling geven aan de hele site, en dan bij specifieke elementen een meer custom styling toe te voegen waar nodig.

**Aria attributes**

Met een aria-label kan je een soort alt tekst toevoegen aan elementen die dat niet kunnen hebben. Bijvoorbeeld een button met alleen een icoon. Met een aria-label kunnen screenreaders de button voorlezen.

Aria-controls

Aria-expanded geeft aan of iets open of dicht is geklapt. Denk aan bijvoorbeeld een dropdown of een hamburger menu. Het schakelt tussen twee states “true” en “false”.

Met aria-live kan je dynamische elementen laten lezen door screenreaders.

**Carrousels**

Als je de carrousel een role=”region” of het element <section> gebruikt en een ariaroledescription=”carousel” geeft dan kan je screenreader uitlezen dat je in een carrousel bent.

Als een slide niet zichtbaar is op het scherm, moet deze verborgen wordenv oor alle gebruikers door aria-hidden=”true” aan de wrapper van de slide toe te voegen en tabindex=”1” aan alle children die focusable zijn.

Vermijdt het gebruik van li elements voor slides. De leest de screenreader eerst alle list items voor. Als je dan een paar niet zichtbaar maakt worden die niet opgelezen terwijl je dat wel wil. Gebruik iets anders (section, divs) zodat alles wel netjes wordt opgelezen.

De carousel controls moeten ook aria-labels krijgen zodat screenreaders die ook kunnen oplezen.

**Focus guards**

Zorg ervoor dat als je een dialog met een close button hebt, dat je focus niet naar de close button gaat als de dialog niet open is. Maar wanneer je via een button de dialog opent wil je dat je focus direct verandert naar de close button. Hiermee zorg je ervoor dat de gebruiker niet gedisorienteerd raakt.

**Kleurcontrast**

Zorg ervoor dat er voldoende kleurcontrast in je website zit zodat mensen met zichtproblemen je website goed kunnen gebruiken. Er zijn tools en richtlijnen om te controleren of je kleurcontrasten goed genoeg zijn. Met chrome devtools krijg je bijvoorbeeld een vinkje op een element als het voldoende kleurcontrast heeft.

**Lettergroottes**

Het is ook belangrijk de juiste lettergrootte te gebruiken om vermoeiende ogen te voorkomen. De standaardregel is om minstens 16 pixels lettergrootte te gebruiken.

**Lijnlengtes**

Voor optimale leesbaarheid is een regellengte van 50 tot 75 tekens, inclusief spaties, ideaal. Zorg ervoor dat je een maximale regellengte hebt zodat het niet stretched op een heel breed scherm.

**Alt-text**

Zorg dat je altijd een goede alt-text toevoegd aan een afbeelding.

**Semantische code**

Schrijf semantisch correcte HTML code!

**Andere dingen die je kan doen…**

-   Skip to content button
-   Prefers-reduced-motion
-   Alle autoplay videos moeten gepauzeerd kunnen worden
-   Zelf een screenreader gebruiken

Korte reflectie:

Fenna’s lezing ging volledig over toegankelijkheid en hoe je dat toepast op je websites. Ze heeft veel technieken laten zien hoe je met HTML en CSS je website een stuk toegankelijker kan maken. Op school leren we een beetje hoe je websites toegankelijk maakt, maar deze lezing ging een stuk meer in detail.

Wat ik vooral merkte was dat er veel hidden features zijn die je gewoon even moet weten om je site iets toegankelijker te maken. Bijvoorbeeld als het gaat om een focus state. Normaal gesproken gebruik je de :focus selector om je focus state te stylen. Dit is alleen niet helemaal wat je wil, omdat hij ook de focus state activeert wanneer je op je muis ergens hebt geklikt wat focusable is. Wat je eigenlijk wil is focus-visible gebruiken. Hiermee focus je alleen op dingen als je het met tab hebt geselecteerd.

Voor mij waren de aria attributes en carrousel wel het lastigst te begrijpen. Ik snap het idee van een aria attribute wel. Met een aria-label kan je bijvoorbeeld een soort alt-text toevoegen aan elk element wat je wil. Dit is een must voor buttons zonder tekst bijvoorbeeld. Maar dan heb je ook nog aria-controls, expanded en live waarvan ik niet helemaal begeep wat ze deden. Bij carrousels ging ze ook erg in detail over roles en roledescriptions, maar ik kon het na een tijdje niet echt meer volgen helaas. Als het gaat om aria-attributes moet ik zelf nog even verder gaan researchen dus.

De algemene boodschap van de lezing vond ik ook erg goed. Ze werkt in een omgeving waar toegankelijkheid een bijzaak is. Het is voor de meeste developers helaas niet heel belangrijk en bij sommige opdrachtgevers ook niet. Fenna is heeft heel veel passie voor het maken van websites waar IEDEREEN van kan genieten. Ik vind dat heel nobel en ik ben blij dat ze in deze lezing hierover kon spreken.

## Gastspreker 3 Jeffrey Arts - 28-2-2024

Ontwerper / Kunstenaar / Front-end developer

**Deployment**

Lokale omgevingen en server

Jeffrey heeft een script gemaakt waarmee hij snel een project kan deployen.

**Toolbox workflow**

Met de toolbox die Jeffrey heeft ontwikkelt kan hij complexe 3D vormen en andere effecten maken zonder dat hij zorgen hoeft te maken over andere dingen zoals routing. Deze effecten kan hij dan heel makkelijk integreren in zijn eigen projecten

**CSS glitch**

Als je in CSS een div in de Z as roteert door een afbeelding, krijg je in elke browser een ander effect. Het ziet er in elke browser heel vreemd uit op een andere manier. Dit laat zien dat niet elke browser hetzelfde werkt.

**Andere toolbox dingen**

Jeffrey kan met isometrische 3D objecten in zijn toolbox leuke dingen doen. Door het perspectief te veranderen op hetzelfde object kan hij verschillende interessante vormen mee maken. Hiermee heeft hij bijvoorbeeld de covidster gemaakt. Hiervan heeft hij er ook 700+ geschilderd.

Hij heeft ook een website waarmee je sculpturen kan maken die hij dan kan realiseren in beton.

Try → fail → new truth → succeed

of

Try → reflect → new truth

Jeffrey’s webdevelopment ecosystem:

-   From [localhost](http://localhost) to the web in under 5 minutes
-   Stick to core technologies as much as possible
-   Create tools that support personal workflow

Het advies is dus, creeër je eigen ecosysteem. Kies bewust je framework en voor een reden. Zorg ervoor dat je een robuuste manier hebt om je projecten te bouwen zodat je op de beste manier projecten kan realiseren.

**Korte reflectie**

Over het algemeen vond ik het een interessant verhaal, maar niet een heel ‘nuttig’ verhaal. Het ging vooral over wat hij heeft gemaakt en dat liet hij zien. Maar het was dus niet iets waar ik veel van kon opsteken en zelf wat van kon toepassen in mijn eigen projecten. Ik kan niet na deze lezing ineens een eigen 3D tool ontwikkelen. Er was ook een beetje een mis-match van tools die wij gebruiken en die Jeffrey gebruikt. Jeffrey gebruikt namelijk enorm veel libraries en frameworks voor al zijn werk, terwijl wij juist leren om te werken zonder. Daarom vond ik het toch lastig om iets waardevols uit deze lezing te krijgen.

Uiteraard vind ik _wat_ hij heeft gemaakt enorm cool. Het lijkt meer dat hij echt een kunstenaar first is en gebruikt hij programmeren als een tool. Hij heeft bijvoorbeeld een toolboxje waarmee hij 3D vormen kan maken. Die 3D objecten worden orthografisch weergegeven. Dit betekent dat ze geen verdwijnpunt hebben, dus geen perspectief en dus eigenlijk altijd als een 2D object worden gezien. Hij heeft dus een één of andere complexe kubusvorm gemaakt die je op oneindig veel perspectieven kan bekijken waardoor je telkens een andere 2D vorm maakt. Hier heeft hij dus 700+ schilderijtjes van gemaakt.

Het belangrijkste wat ik hieruit heb opgestoken is dat je gewoon dingen moet maken omdat je het leuk vind. Jeffrey heeft allerlei projecten gemaakt die veel tijd kosten en misschien compleet nutteloos zijn voor de meeste mensen, maar hij doet het omdat hij er voldoening uit krijgt. En daar sta ik compleet achter. Tegenwoordig moet _alles_ een reden hebben. Waarom deze button? Waarom dit logo op deze manier? Waarom deze kleur? WAAROM NIET???? Waarom mogen we niet iets maken omdat we dat gewoon leuk vinden? Natuurlijk niet altijd, maar af en toe een beetje eigen saus creeëren geeft gewoon een meer persoonlijke touch.

## Gastspreker 4 Nils Binder - 6-3-2024

Van 9elements

**3 units bij 9elements**

-   Communication design (corporate identity - print etc. Non coding designers)
-   Product development (big projects - data vis, banking clients etc)
-   Web development (frontend, small to medium sized websites)

Deze drie units werken samen om mooie projecten te realiseren.

**Wrapper element (aka container)**

A wrapper sets a:

-   max width for the content
-   padding for the content
-   centers content

Originele manier om een wrapper te stylen:

.wrapper {

max-width: 75rem;

margin: 0 auto;

max-width: 0 1.5rem;

}

Korter:

.wrapper {

width: min(100% - 3rem, 75rem)

margin-inline: auto;

}

Korter maar minder leesbaar:

.wrapper {

margin-inline: max(1.5rem, ((100% - 75rem) / 2));

}

Vroeger maakte we website layouts in photoshop. Tegenwoordig kan je dit veel beter in een software als Figma doen. Dit is omdat Figma speciaal gemaakt is voor webdesign. Dingen als layouts en shadows lijken heel erg op de manier hoe CSS het ook doet.

In Figma maken we vaste designs. Hierdoor kan je perongeluk automatisch ook statische websites maken terwijl je JUIST veel meer flexibelere websites kan maken.

In CSS you have ALOT of viewport units which you can use. In Figma theres no way to use any of these. In figma you only have pixels, % and rem.

**Optional column technique**

Je kan veel creatievere en interessante grids maken die niet altijd exact hetzelfde eruit zien op elke grootte. Met optional grids kan je extra grid cellen toevoegen die niet altijd gebruikt worden (witruimte), maar wel gebruiken KUNNEN worden. Bijvoorbeeld wanneer je de pagina groter of kleiner maakt.

Op deze website zie je een goed voorbeeld hiervan: [dasruhrgebiet.de](http://dasruhrgebiet.de)

Als je een website maakt, maak gebruik van de ruimte die je hebt! Als je een groot scherm hebt wil je gebruik maken van de extra ruimte die je hebt. Je kan bijvoorbeeld de navigation verplaatsen naar links of de headlines uitvergroten.

[bryck.com](http://bryck.com)

**Korte reflectie+**

## Gastspreker 5 Jeremy Keith - 14-3-2024

Declarative Design

**Music**

Two different approaches:

-   **Classical:** A classical musician makes music using notes. It’s very deliberate and specific
-   **Jazz:** Much more improvised

**Programming**

Two different approaches:

-   Imperative programming: Give the computer instructions which it will then execute in order.
-   Declarative programming: You only declare the output and the computer will figure out how to get there. SQL is an example of this type of programming.

HTML is declarative. This is because it is domain specific.

CSS is declarative. This is because every line you write in CSS is a suggestion.

Javascript is imperative. You are not bound to a specific vocabulary.

In declarative programming, if you make a mistake, the browser will ignore the mistake and continue with the rest of the code. In imperative programming if you make a single mistake, it will stop and give you an error.

Declarative languages can only be used in specific places and you have a lot more leeway if you make mistakes.

Imperative languages are able to be used in many places.

**Example of an imperative mindset:**

You could make an entirely functional button in JS, but you wouldn’t do it because HTML gives it to you for free. So listen to this quote:

> Javascript should only do what only javascript can do

Declarative programming could feel like giving up control beause you would give agency to the browser instead of yourself. Imperative programming is definitely more of the developer being in control.

**Declarative in CSS**

If using pixels instead of rems and padding-left instead of padding-inline-start, you would program a lot more imperative. You are then dictating what shows up on screen for the end user. If the user is using a language which reads from right to left or has a different standard font size the website would not show up correctly for the user.

[utopia.fyi](http://utopia.fyi)

These days in CSS you have a lot of functions like calc(), clamp, min and max etc. which you could use to create great responsive designs. You shouldn’t want to have complete control all the time, let the computer do the calculations. You should set the guard rails yourself and then let the browser do the rest of the work filling in the gaps.

> Be the browser’s mentor, not its micromanage

[buildexcellentwebsit.es](http://buildexcellentwebsit.es)

Is declarative better than imperative? It depends…

-   Culture: depending on the workspace culture, you could have a imperative culture (be here on time, perfect schedules) or more declarative (I don’t care how you do it, but have this task done at the end of the week)
-   Thinking:
    -   Analytical thinking. Understand the whole by analysing the individual bits.
    -   Systems thinking. Thinking more broadly and looking at the whole.
-   Design systems: most design systems are more akin to analytical thinking.

An imperative designer would style 3 buttons of the same family by declaring each color and style individually.

A declarative designer would say: the border should be 20% lighter than the background colour

It also depends on the medium. Things like print, native app and os-specific things you might want to use an imperative approach.

But on the world wide web, it is probably a safe bet that you should be thinking more declaratively.

Responsive design is more of a conversation with the user instead of dictating the user.

## Gastspreker(s) 6 Marieke en Pim - 3-4-2024

Van Digitaal toegankelijk.

**Situationele beperkingen**

-   Je kijkt een filmpje in de trein zonder geluid
-   Je kan je scherm niet zien omdat de zon erop schijnt

**Tijdelijke beperkingen**

-   Je breekt je arm en nu kan je niet meer je muis gebruiken voor een paar maanden

**Permanente beperkingen**

-   ADHD
-   Blind
-   Doof
-   Etc...

Stel jezelf de vraag: 'wie sluit je uit' als je aan een project werkt. Je kan best een flitsende website maken, maar iemand met epilepsie wil daar niet op komen natuurlijk.

**Wat is digitale toegankelijkheid**

WCAG is Web Content Accessibility Guidelines. Die geven aan wat je moet doen om een website toegankelijk te maken.

4 hoofdonderwerpen

P.O.U.R.:
-   perceivable
-   operable
-   understandable
-   robust

4 hele belangrijke

-   audio control
    -   audio van langer dan 3 seconden moet je kunnen pauzeren of stoppen
-   no keyboard trap
    -   Wanneer je met het toetsenbord navigeert mag je niet vast komen te zitten
-   pause stop hide
    -   alle bewegende, knipperende, scrollende elementen die: automatisch starten, langer dan 5s duren en parallel aan andere content getooond; wordt moet gepauzeerd of gestopt kunnen worden
-   three flashes or below threshold
    -   Er mag geen enkel element 3 keer of meer binnen een seconde flitsen

**Wat kan je hieraan doen?**

- P.O.U.R.
- Stel deze vragen:
    - Kan deze content door iedereen worden waargenomen? (percievable)
    - Kan de content door iedereen bereikt en gebruikt worden? (operable)
    - Kan deze content door iedereen begrepen worden? (understandable)
    - Is de techniek achter mijn digitale product semantisch correct opgebouwd? (robust)
- Beluister jouw digitale product eens met een schermlezer!
- Ga door je website heen zonder muis
- Test met je doelgroep

## Gastspreker Rosa Schuurmans - 10-4-2024

**Circuit bending**

De creatieve manipulatie van ciruits in elektronische apparaten om nieuwe muziek- of visuele instrumenten te creëren.

In principe maak je van bestaande (elektronische) spullen iets anders.

Circuit bending is het begin van de elektronische kunst / unstable media.

Circuit bending is te vergelijken met inspect element. Eigenlijk kijk je naar iets wat bestaat (website) en kijk je hoe het werkt en je kan vanalles aanpassen wat erin zit.

> De status-quo niet per definitie accepteren
