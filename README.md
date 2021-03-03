# CSS to the Rescue - Zen Garden
Live Demo:  https://ninapajonk.github.io/css-to-the-rescue-2021/

< foto eindresultaat>

# Week 1 - Je plan

Voor de eindopracht heb ik gekozen om aan de slag te gaan met "Zen-garden". Het lijkt mij een hele leuke uitdaging om de HTML van een menu kaart helemaal aan te pakken met puur CSS en deze keer Javascript links te laten liggen. 
Om te beginnen heb ik op Pinterest wat rond gekeken naar posters en bestaande menu kaarten. Al snel kwam ik een poster tegen met taarten. En door de inspirende lectures van Vasilis kreeg ik al snel ideeen  om dit stilstaand beeld om te toveren naar iets bewegends. 
## Inspiratie:

![Image of pinterest inpso](https://github.com/NinaPajonk/css-to-the-rescue-2021/blob/zen_garden/images/360%20Degrees%20Of%20Cake.jpg)

## Schetsen
Schets 1:

![Image of schets 1](/images/schets1.jpg)

De CSS- technieken waar ik mee aan de slag wil gaan:
- Prefer Color scheme (context)
- Print Style sheet (context) 
- SVG's toepassen met filters, animeren (Restrictie)
- Responsive maken zonder media queries, Clamps. (Restrictie)

Met alle 4 CSS- technieken nog niet eerder gewerkt voor deze minor. Prefer Color Scheme heb ik toegepast in de kennismakingsopdracht samen met Stan. Hiervoor hadden wij Baby Yoda gebruikt. In mijn concept wil ik deze verder uitbreiden gefocust op leesbaarheid door middel van contrast en mogelijke svg kleuren aanpassen. 
Voorbeeld kennismakingsopdracht:

```
/* ...................................add dark modus css.................................. */
@media screen and (prefers-color-scheme: dark) {
  body {
    background-color: black;
    color: navy;
  }
  section[name="lightsaber"]:after {
    display: block;
  }

  input[data="Orange"]:checked ~ label {
    --saberColor: rgb(252, 187, 67);
  }
  input[data="Yellow"]:checked ~ label {
    --saberColor: rgb(255, 255, 56);
  }
  input[data="Green"]:checked ~ label {
    --saberColor: rgb(5, 255, 5);
  }
  input[data="Red"]:checked ~ label {
    --saberColor: rgb(255, 0, 0);
  }
}

@media screen and (prefers-color-scheme: light) {
  body {
    background-color: #ddd;
    color: black;
  }
}
```
![Image of darkmodus baby yoda](/images/yoda_dark.jpg)
![Image of lightmodus baby yoda](images/yoda_light.jpg)



Waar liggen je (grootste) uitdagingen: Ik heb gemerkt dat ik CSS echt meer begin te waarderen. Voorheen gebruikte ik CSS puur alleen voor layout (grids etc.) en nu door onder andere de thema sessies is er een nieuwe wereld voor me open gegaan. De grootste uitdaging ligt het denk ik in de keuzesmaken. Wat ga ik wel toepassen in mijn ontwerp en wat niet... (Misschien in een volgend project de laserstralen toepassen?)


# Week 2  - Voortgang
De eerste stappen die ik heb gezet zijn het bekijken van de gegeven HTML. Wat zijn de categorieen, welke elementen zijn er gebruikt etc. Ik ben in CSS begonnen met het centreren en ruimte creeëren van de content. Veel zinnen begonnenn niet met hoofdletters dus hier heb ik first letter uppercase toegepast. En ik vond het qua hierarchie fijner lezen om de titels in capitals te weergeven. Daarnaast heb ik veel SVG's gevonden om net zoals de pinterest inspiratie deze onder elkaar te zetten en hopelijk te kunnen laten draaien. 
```
p:first-letter {text-transform:uppercase;}
h3:first-letter {text-transform:uppercase;} 
```
De uitdaging voor volgende week is om verder te gaan met de SVG's. Ik had eerst de svg's als een img ingeladen, maar na feedback van Vasilis tijdens de wrap up heb ik er voor gekozen om de gehele SVG in mijn HTML in te laden. Ik schrok eerst van de hoeveelheid code.. maar op deze manier kan je er wel veel meer mee. Ik heb ook nog ruzie met alle SVG's netjes onder elkaar te zetten maar hierga ik volgende week mee verder. 

# week 3 - voortgang
Mijn SVG's zijn inmiddels allemaal in zn geheel in de HTML gezet, en qua lay-out onder elkaar. Met de tekst ernaast van de Menu kaart vind ik het erg rommelig overkomen en niet fijn lezen. In de HTML zijn de prijzen van gerechten tussen de elementen div gezet. Ik heb hiervoor een span gemaakt, omdat ik dat gepaster vind bij de prijzen. En hierdoor makkelijker met een nieuwe div verder kon stylen dat wanneer je over de SVG's hovert de tekst te voor schijn komt. Dit heb ik gedaan met behulp van een youtube tutorial: https://www.youtube.com/watch?v=HHqBS7xFnPM. 
Om het qua huistijl meer bij mijn concept te laten passen heb ik in plaats van de rechte vormen die ze in de tutorial gebruiken voor ronde vormen zodat dit ook weer past bij de ronde SVG's. Zie video hieronder, het ging niet meteen de eerste keer soepeltjes: 

video


# Week 4 - Afronding

Na de laatste themasessie accessibility, de voorbeelden die we te zien kregen over grote/bekende bedrijven die op hun site de toegankelijkheid niet op orde hadden. En hoe moeilijk het dan voor gebruikers kan zijn om bijvoorbeeld simpel door een website te navigeren verbaasde mij enorm. Als ik meer tijd had gehad, had ik dat zeker nog willen toepassen in mijn eigen concept, die nu nog niet zo gebruiksvriendelijk is. 

In mijn concept heb ik er in de laatste week voor gekozen om toch een navigatie toe te voegen. Het plan in het begin was eigenlijk om alles in een window te proppen en dat de SVG's dus erg uitgezoomd waren. Pas wanneer je er over heen hoverde was het de bedoeling dat het door middel van scale vele malen groter zou worden. Dit is mij niet gelukt om voor elkaar te krijgen waardoor ik dus last minute voor een navigatie bar heb gekozen die op elk moment op de pagina zichtbaar is. Position: fixed;

Naast de context: Prefer color scheme, leek het mij ook leuk dat je handmatig op de site zelf door middel van de toggle de kleuren modus kon aanpassen. Zodat je niet hiervoor je systeem instelling hoefde aan te passen. Wanneer de toggle "switched" wordt de roze ronde knop bij dark modus iets donkerder. Ik heb gekozen voor een subtiele overgang van de toggle zelf omdat de achtergrond en de SVG's al mee veranderen. 

MOET NOG GEDAAN WORDEN:
Responsive zonder Media queries, hier voor heb ik wat onderzoek gedaan en kwam ik de techniek Clamp tegen. Ook dit heb ik nog niet eerder gebruikt. Source: https://www.youtube.com/watch?v=CICYdO0g8Ew

MOET NOG GEDAAN WORDEN:
SVG's animeren. 
source: https://www.youtube.com/watch?v=KLU4PUd7N14&t=933s

