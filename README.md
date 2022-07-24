# AI in de Klas - Objectclassificatie v2 met YOLOv6
## Introductie

<img src="resultaten/Resultaat_Kajak.png" width="800">

Tijdens eerdere projecten maakten leerlingen en cursisten kennis met supervised learning (Machine Learning) en hoe je het kan toepassen om aan objectclassificatie te doen. 
We maakten met bovenstaande aanpak reeds een [Slimme Vuilnisbak](https://www.robbewulgaert.be/onderwijs/bouw-een-slimme-vuilnisbak) en [eigen projecten](https://www.robbewulgaert.be/onderwijs/1-jaar-ai-in-de-klas). 

Bovenstaande aanpak is uitstekend voor een inleiding in objectclassificatie door te werken met bv. een Teachable Machine. Deze aanpak kent echter ook beperkingen, omdat het slechts één klasse per keer detecteert / aantoont. 
Die aanpak kan dus moeilijkn overweg met meer gecompliceerde scenes zoals een drukke straat, een koelkast met meerdere items ... Door gebruik te maken van een YOLO-framewerk kunnen we deze beperking oplossen. 
YOLOv6 is een éénfasig framework voor objectdetectie, speciaal voor industriële toepassingen, met een hardware-vriendelijk efficiënt ontwerp en hoge prestaties.

<img src="resultaten/Resultaat_Barry.png" width="800">

Deze aanpak is gebaseerd op aangepaste code van [Meituan YOLOv6](https://github.com/meituan/YOLOv6). Ook de COCO-dataset werd aangepast voor gebruik in het Nederlandstalig onderwijs. 



## Waar wordt nog aan gewerkt?

- [ ] Lesmateriaal zoals boekjes, slides ... 
- [ ] Materiaal ontwerpen om eigen datasets te trainen en toe te voegen aan de Notebook ... 
- [ ] Eindresultaten uit de klaspraktijk ... 
- [ ] Beter gestructureerde Colab Notebook. 

<img src="resultaten/output.gif" width="800">

## Hoe gebruiken? 

Dit materiaal behoort tot de lessenreeks 'Objectclassificatie v2 met YOLOv6' op het Sint-Lievenscollege Gent. 
Met dit lesmateriaal is het mogelijk aan objectdetectie te doen met de standaard COCO-dataset, of met een zelfgemaakte dataset. 
Objectdetectie is mogelijk op drie bronnen, namelijk: 

- [ ] een afbeelding
- [ ] een video
- [ ] de webcam-feed

Afbeeldingen en video's kunnen ingeladen worden via de GitHub of vanaf de computer van de leerling. Hierbij kan ook geteld worden hoeveel objecten uit elke klasse uit de dataset er werd gedetecteerd. 
Bij de webcam kan live objectdetectie worden toegepast, zonder teller-functie. 

<img src="resultaten/resultaat_schaap.png" width="800">

## Modellen en dectectiemogelijkheden 

Standaard maakt de Notebook gebruik van YOLOv6 met de Nano en Small modellen. Deze maken gebruik van de COCO-dataset. Deze werd getraind op circa 120.000 afbeeldingen kan een flink aantal items detecteren; namelijk: 
<table>
    <thead>
        COCO Dataset
    </thead>
<tr>
</tr>
<tr>
<td>
persoon
</td>
<td>
fiets
</td>
<td>
auto
</td>
<td>
motor
</td>
<td>
vliegtuig
</td>
</tr>
<tr>
<td>
bus
</td>
<td>
trein
</td>
<td>
vrachtwagen
</td>
<td>
boot
</td>
<td>
verkeerslicht
</td>
</tr>
<tr>
<td>
brandkraan
</td>
<td>
stopbord
</td>
<td>
parkeermeter
</td>
<td>
bank
</td>
<td>
vogel
</td>
</tr>
<tr>
<td>
kat
</td>
<td>
hond
</td>
<td>
paard
</td>
<td>
schaap
</td>
<td>
koe
</td>
</tr>
<tr>
<td>
olifant
</td>
<td>
beer
</td>
<td>
zebra
</td>
<td>
giraf
</td>
<td>
rugzak
</td>
</tr>
<tr>
<td>
paraplu
</td>
<td>
handtas
</td>
<td>
das
</td>
<td>
koffer
</td>
<td>
frisbee
</td>
</tr>
<tr>
<td>
ski
</td>
<td>
snowboard
</td>
<td>
sportbal
</td>
<td>
vlieger
</td>
<td>
basebalknupel
</td>
</tr>
<tr>
<td>
basebalhandschoen
</td>
<td>
skateboard
</td>
<td>
surfbord
</td>
<td>
tennisracket
</td>
<td>
fles
</td>
</tr>
<tr>
<td>
wijnglas
</td>
<td>
tas
</td>
<td>
vork
</td>
<td>
mes
</td>
<td>
lepel
</td>
</tr>
<tr>
<td>
kom
</td>
<td>
banana
</td>
<td>
appel
</td>
<td>
sandwich
</td>
<td>
sinaasappel
</td>
</tr>
<tr>
<td>
broccoli
</td>
<td>
wortel
</td>
<td>
hot dog
</td>
<td>
pizza
</td>
<td>
donut
</td>
</tr>
<tr>
<td>
cake
</td>
<td>
stoel
</td>
<td>
zetel
</td>
<td>
plant in een pot
</td>
<td>
bed
</td>
</tr>
<tr>
<td>
eettafel
</td>
<td>
toilet
</td>
<td>
tv
</td>
<td>
laptop
</td>
<td>
muis
</td>
</tr>
<tr>
<td>
afstandsbediening
</td>
<td>
toetsenbord
</td>
<td>
GSM/Smartphone
</td>
<td>
microgolfoven
</td>
<td>
oven
</td>
</tr>
<tr>
<td>
broodrooster
</td>
<td>
lavabo
</td>
<td>
koelkast
</td>
<td>
boek
</td>
<td>
klok
</td>
</tr>
<tr>
<td>
vaas
</td>
<td>
schaar
</td>
<td>
teddybeer
</td>
<td>
haardroger
</td>
<td>
tandenborstel
</td>
</tr>
</table>


## Credits

Voor vragen over deze lessenreeks kan je terecht bij jouw leerkracht over mailen naar: robbe.wulgaert@sintlievenscollege.be 

Bedacht en uitgewerkt met educatief doeleinde door Robbe Wulgaert, [Sint-Lievenscollege Gent](https://www.sintlievenscollege.be). 

[robbewulgaert.be ](https://www.robbewulgaert.be)

[AI in de Klas ](https://www.aiindeklas.be)
