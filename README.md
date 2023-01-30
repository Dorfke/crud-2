# crud-2
TypeScript - CRUD užduotis 1
Užduoties tikslas
Atvaizduoti duomenis HTML lentele, pagal esybių schemą.

Failų struktūra
components/ - aplankas skirtas komponentams - klasėms, kurios naudojamos atvaizduoti elementams DOM'e

data/ - duomenų failai

helpers/ - Pagalibinės funkcijos ir klasės, skirtos kodo švarinimui ir perpanaudojimui

types/ - bendrai naudojami tipai

Esybių ryšių diagrama (entity relation diagram).


Darbo atlikimo eiga
Aplanke ./types duoti tipų 'griaučiai'. Implementuokite tipus pagal schemą. car-joined.ts tipas turi turėti tokias savybes:

id: string
price: number
year: number
brand: string
model: string
./helpers/cars-collection.ts

Sukurkite konstruktorių, kuris priimtų markes, mašinas ir modelius. Gautus duomenis išsaugokite objekte
Sukurkite privatų metodą joinCar kuris apjungtų vieną mašiną
Sukurkite metodą, kurį iškvietus gautumėte visas apjungtas mašinas.
./components/app.ts

Sukurkite savybes:
private htmlElement: HTMLElement;
private carsCollection: CarsCollection;
Sukurkite konstruktorių, kuris
priimtų selektorių ir pagal jį rastą elementą priskirtų į htmlElement savybę.
sukurtų pradinį carsCollection objektą
Sukurkite metodą initialize, kuriame būtų atliekami komponento atvaizdavimo veiksmai
./components/table.ts

Sukurkite tipą TableProps:
title: string
columns: Type
rowsData: Type[]
Sukurkite savybes:
public htmlElement: HTMLTableElement;
private props: TableProps;
private tbody: HTMLTableSectionElement;
private thead: HTMLTableSectionElement;
Sukurkite konstruktorių, kuris:
sukurtų pradinius htmlElement, thead ir tbody elementus
iškviestų metodą initialize
Sukurtite metodą initialize, kuriame:
atliktumete lentelės antraštės atvaizdavimą
atliktumetė lentelės duomenų eilučių atvaizdavimą
apjungtumėte elementus
./components/app.ts

papildykite initialize metodą, jog būtų įterpiama lentelė
Rezultato pavyzdys


Papildomai
Sukurkite lentelės duomenų patikrinimo funkciją, kuri tikrintų duomenų sutapimą su antraštės stulpeliais
Kodo dalis, kurios gali būti perpanaudotos iškelkite į atskiras funkcijas aplanke helpers
Atsakymai
GaliTE peržiūrėti sprendimą aplanke ./atsakymas