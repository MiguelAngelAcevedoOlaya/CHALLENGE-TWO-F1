# Reto-2

## Relation Formula 1 - Fan

``` mermaid
classDiagram
    direction RL
    class Formula1{
        +Teams
        +Races
        +FIA
    }
    class Fan{
    }
    Fan"1" --> "1" Formula1 : See()

```

## Relation Formula 1 - Fan

``` mermaid
classDiagram
    class Fan{    
    }
    class Formula1{
        + Teams
        + Races
        + FIA
    }
    class Teams{
        + Team Principal
        + Pilots
        + Cars
        + Mechanics
        + Engineers
    }
    class FIA{
        + Categories
        + Rules
        + Comissioners
        + Security
    }
    class Races{
        + Countries
        + Circuits
        + Calendar
    }
    Fan --> Formula1 : See
    Teams --* Formula1
    FIA *--  Formula1
    Races --* Formula1
```

## Relation between Teams

``` mermaid
classDiagram
    Teams <|-- Ferrari
    Teams <|-- Mercedes
    Teams <|-- Mclaren
    Teams <|-- RedBull
    Teams <|-- AstonMartin
    Teams <|-- Alpine
    Teams <|-- RB
    Teams <|-- Kick
    Teams <|-- Haas
    Teams <|-- Williams
    class Teams{
        + Team Principal
        + Pilots
        + Cars
        + Mechanics
        + Engineers
    }
    class Ferrari{
      +Fred Vasseur
      +Charles leclerc 
      +Carlos Sainz
      +Ferrari SF24
      +Livery Red
      +Performance 8/10
    }
    class Mercedes{
      +Toto Wolf
      +Lewis Hamilton 
      +George Russel
      +Mercedes W15
      +Livery Silver and Black
      +Performance 8/10
    }
    class Mclaren{
      +Andrea Stella
      +Lando Norris 
      +Oscar Piastri
      +MCL38
      +Livery Orange and Black
      +Performance 8/10
    }
    class RedBull{
      +Cristian Horner
      +Max Verstappen
      +Checo Perez
      +RB20
      +Livery Blue, Red, Yellow and Black
      +Performance 10/10
    }
    class AstonMartin{
      +Mike Krack
      +Fernando Alonso
      +Lance Stroll
      +AMR24
      +Livery Green and Black
      +Performance 7.5/10
    }
    class Alpine{
      +Bruno Famin
      +Esteban Ocon
      +Pierre Gasly
      +A524
      +Livery Blue, pink and Black
      +Performance 6/10
    }
    class RB{
      +Laurent Mekies
      +Daniel Ricciardo
      +Yuki Tsunoda
      +VCARB01
      +Livery Blue, White, Red and Black
      +Performance 5/10
    }
    class Kick{
      +Alessandro Alunni Bravi
      +Valteri Bottas
      +Guanyou Zhou
      +C44
      +Livery Green and Black
      +Performance 5/10
    }
    class Haas{
      +Ayao Komatsu
      +Nico Hulkenberg
      +Kevin Magnussen
      +VF24
      +Livery Red, White and Black
      +Performance 4/10
    }
    class Williams{
      +James Vowles
      +Alexander Albon
      +Logan Sargeant
      +FW46
      +Livery Blue and Black
      +Performance 5/10
    }
```

## Relation Between Races

``` mermaid
classDiagram
    Races <|-- Bahrein
    Races <|-- SaudiArabia
    Races <|-- Australia
    Races <|-- Japan
    Races <|-- China
    Races <|-- Miami
    Races <|-- EmiliaRomagna
    Races <|-- Monaco
    Races <|-- Canada
    Races <|-- Spain
    Races <|-- Austria
    Races <|-- UnitedKingdom
    Races <|-- Hungary
    Races <|-- Belgium
    Races <|-- Netherlands
    Races <|-- Italy
    Races <|-- Azerbaiyan
    Races <|-- Singapour
    Races <|-- UnitedStates
    Races <|-- Mexico
    Races <|-- Brazil
    Races <|-- Vegas
    Races <|-- Qatar
    Races <|-- AbuDhabi
    class Races{
        + Countries
        + Circuits
        + Calendar
    }
    class Bahrein{
      +Sakhir
      +First Race
      +Febraury
      +Night
      +Circuit
    }
    class SaudiArabia{
      +Yeda
      +Second Race 
      +March
      +Night
      +Street
    }
    class Australia{
      +Melbourne
      +Tirht Race
      +March
      +Day
      +Circuit
    }
    class Japan{
      +Suzuka
      +Fourth Race
      +April
      +Day
      +Circuit
    }
    class China{
      +Shanghai
      +Fifth Race
      +April
      +Day
      +Circuit
    }
    class Miami{
      +Miami
      +Six Race
      +May
      +Day
      +Circuit
    }
    class EmiliaRomagna{
      +Imolia
      +Seven Race
      +May
      +Day
      +Circuit
    }
    class Monaco{
      +Monaco
      +Eight Race
      +May
      +Day
      +Street
    }
    class Canada{
      +Montreal
      +Ninth Race
      +June
      +Day
      +Circuit
    }
    class Spain{
      +Barcelona
      +Ten Race
      +June
      +Day
      +Circuit
    }
    class Austria{
      +Spielberg
      +Eleven Race
      +June
      +Day
      +Circuit
    }
    class UnitedKingdom{
      +Silverston 
      +Twelve Race
      +July
      +Day
      +Circuit
    }
    class Hungary{
      +Hungaroring
      +Tirthteen Race
      +July
      +Day
      +Circuit
    }
    class Belgium{
      +Spa
      +Fourthteen Race
      +July
      +Day
      +Circuit
    }
    class Netherlands{
      +Zandvoort
      +Fifhtteen race
      +August
      +Day
      +Circuit
    }
    class Italy{
      +Monza
      +Sixteen Race
      +September
      +Day
      +Circuit
    }
    class Azerbaiyan{
      +Baku
      +Seventeen Race
      +September
      +Day
      +Street
    }
    class Singapour{
      +Singapour
      +Eightteen Race
      +September
      +Night
      +Street
    }
    class UnitedStates{
      +Texas
      +Nineteen Race
      +October
      +Day
      +Circuit
    }
    class Mexico{
      +City of Mexico
      +Twenty Race
      +October
      +Day
      +Circuit
    }
    class Brazil{
      +Interlagos
      +Twenty One race
      +November
      +Day
      +Circuit
    }
    class Vegas{
      +Vegas
      +Twenty two race
      +November
      +Night
      +Street
    }
    class Qatar{
      +Lusail
      +Twenty three race
      +November
      +Night
      +Circuit
    }
    class AbuDhabi{
      +Yas Marina
      +Twenty four race
      +November
      +Day/Night
      +Circuit
    }


```
