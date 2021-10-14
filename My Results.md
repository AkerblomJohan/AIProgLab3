# Här är mina resultat hittils:

I den här filen ska ni beskriva:
- Era experiment
- Era slutsatser

## Glöm inte!

Glöm inte att ha med figurer:

![TensorBoard download](fig/TensorBoardDownload.png "Glöm inte att kryssa i 'Show data download links' så att ni kan ladda ner era filer.")


7
a) 

Det finns ingen större tidsskillnad på LR. Ju större LR det är desto snabbare tränas modellen.
Medan ett för stort värde kan leda till att man lär sig en suboptimal för snabbt eller att det blir en instabil träningsprocess.
Första bilden är för Conventional med LR = 0.01, 0.3, 0.6 samt 0.9  


//Bild, får ej in atm

Andra bilden är Non-Conventional med LR = 0.01, 0.3, 0.6 samt 0.9 

//Bild, får ej in atm


b) 

Där är en stor skillnad om man kollar till Accuracy av testerna och "Batch-Size". Ju större size desto mer uppdateringar blir det och på så sätt mer "accurate" men det kan också leda till dålig generalisering. 
Om man istället har mindre batch-size blir det mindre uppdateringar och det kan leda till att modellen inte går samman. 

c) 

Non-Conv är väldigt snabb jämfört med Conv modellen. Men samtidigt så har Conv modellen lite högre accuracy än vad Non-Conv har. 

Conv modellen bevarar förhållandet mellan pixlar genom att lära sig bildfunktioner med små kvadrater av inmatade data samtidigt som de använder flera lager på bilder och använder filtrering för att analysera bildinmatningar.  

Non-Conv är rader med datapunkter som genom neuroner använder samma nätverk. De använder också vikter för att lära sig och vikterna ändras efter varje iteration. 

d) 

Både non-conv och conv ger dåliga resultat på "Moved Data" testseten. conv ger ett resultat på snitt 18, non conv ligger nere på 12. På de roterade testsetten ger conv en accuracy på 86, vilket är 10 under de vanliga. non-conv hamnar på 75, vilket är ungefär 14 under de vanliga. 
Det är samma skillnad mellan de olika testseten för båda nätverken. 