# Procesverslag
**Auteur:** Sven Nijhuis

**De opdrachten:** [opdracht 1](https://svennijhuis.github.io/Animtion-Jordan-logo/) en [opdracht 2](opdracht2/index.html)

## Bronnenlijst
  1. School - leraar
  2. [W3schools](https://www.w3schools.com/)
  3. [Css-tricks](https://css-tricks.com/)



## Opdracht 1 plan

<details open>
  <summary>uitwerken na schetsen idee</summary>


  ### Je storyboard:

  ![](https://raw.githubusercontent.com/svennijhuis/Animtion-Jordan-logo/main/images/flow.png )

  Uiteindelijk heb ik niet helemaal mijn storyboard gevolgd, omdat ik het design niet mooi vond achteraf en ik kreeg andere ideeën.

  ### Je ambitie: 
  Aan deze technieken/punten wil ik werken:
  - Overgang
  - Draw line
 
</details>



## Opdracht 1 reflectie

<details open>
  <summary>uitwerken bij afronden opdracht</summary>

  ### Dit ging goed/Heb ik geleerd: 
  - Ik heb geleerd om meerdere animties in een te voegen.

          animation: top-to-bottom 3s forwards, 1s text-gradient-animation 4s forwards;
  - Om een line om een svg te vormen.

          @keyframes dash {
            to {
              stroke-dashoffset: 0;
            }
          }

          svg {
            height: 300px;
            width: auto;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation-name: svganimtion;
            animation-delay: 12s;
            animation-duration: 5s;
            animation-fill-mode: forwards;
            transition-timing-function: cubic-bezier(0.25, 0.1, 0.25, 1);
            fill: none;
          }

          @keyframes svganimtion {
            0% {
              fill: none;
            }
            100% {
              fill: var(--color-first);
            }
          }

          .cls-1{
            stroke:var(--color-first);
            stroke-miterlimit:10;
            stroke-width:3px;
            stroke-dasharray: 2000;
            stroke-dashoffset: 2000;
            animation: dash 5s linear forwards;
            animation-delay: 8.5s;
          }
  - Overgang met background letters

          @keyframes text-gradient-animation {
            0% {
              background-position: left bottom;
              color: transparent;
            }
            50% {
              background-position: left bottom;
            }
            75% {
              background-position: right top;
              background-image: linear-gradient(
                45deg,
                var(--color-second),
                var(--color-first)
              );
            }
            100% {
              background-position: right top;
              background-image: var(--color-first);
              color: var(--color-first);
            }
          }
  - line om html heen.
  
          -webkit-text-stroke: 1px var(--color-first);

  ### wat vond ik lastig: 
  - Ik heb geleerd om meerdere animties in een te voegen.
  - Om een line om een svg te vormen.
  - Overgang met background letters.
  - overline om html heen.
  - Twee animaties in een element
  - responsive maken, omdat ik niet mobile firt ben begonnen.
  - Css netjes houden.


  ### Je uitkomst:
  `light mode`
  ![](https://github.com/svennijhuis/Animtion-Jordan-logo/blob/main/images/einde-animatie.png)

  `Dark mode`
  ![](https://github.com/svennijhuis/Animtion-Jordan-logo/blob/main/images/dark-mode.png)

### Verbeteringen na feedback

#### Code ordenen 
          /*********************/
          /* CUSTOM PROPERTIES */
          /*********************/

#### Code korter schrijven
          span{
            animation-name: animtion-span;
            animation-duration: 0.5s;
            display: flex;
            align-items: center;
            animation-fill-mode: forwards;
          }

          span:nth-of-type(1) {
            animation-delay: 5s;
          }

          span:nth-of-type(2) {
            animation-delay: 5.5s;
          }

          span:nth-of-type(3) {
            animation-delay: 6s;
          }

          span:nth-of-type(4) {
            animation-delay: 6.5s;
          }

          span:nth-of-type(5) {
            animation-delay: 7s;
          }

          span:nth-of-type(6) {
            animation-delay: 7.5s;
          }
</details>



## Opdracht 2 plan

<details>
  <summary>Uitwerken na schetsen idee</summary>


  ### Je ontwerp:
  <img src="readme-images/dummy-plaatje.svg" width="375px" alt="ontwerp opdracht 2">


  ### Je ambitie: 
  Aan deze technieken/punten wil ik werken:
  - punt 1
  - punt 2
  - nog een punt
  - ...
</details>



## Opdracht 2 test

<details>
  <summary>Uitwerken na testen (week 6/7)</summary>

  Neem minimaal 5 bevindingen op:



  ### Bevinding 1:
  Omschrijving van wat er nog niet orde was (tekst en afbeeding(en)).

  #### oplossing:
  Beschrijving hoe je het hebt hebt opgelost of als het niet gelukt is hoe je het zou oplossen (tekst en afbeeding(en)).



  ### Bevinding 2:
  Omschrijving van wat er nog niet orde was (tekst en afbeeding(en)).

  #### oplossing:
  Beschrijving hoe je het hebt hebt opgelost of als het niet gelukt is hoe je het zou oplossen (tekst en afbeeding(en)).



  ### Bevinding 3:
  ...
</details>



## Opdracht 2 reflectie

<details>
  <summary>uitwerken bij afronden opdracht (voor week 8)</summary>

  ### Je uitkomst - karakteristiek screenshot(s):
  <img src="readme-images/dummy-plaatje.svg" width="375px" alt="uitkomst opdracht 2">


  ### Dit ging goed/Heb ik geleerd: 
  Korte omschrijving met plaatje(s)

  <img src="readme-images/dummy-plaatje.svg" width="375px" alt="top">


  ### Dit was lastig/Is niet gelukt:
  Korte omschrijving met plaatje(s)

  <img src="readme-images/dummy-plaatje.svg" width="375px" alt="bummer">
</details>