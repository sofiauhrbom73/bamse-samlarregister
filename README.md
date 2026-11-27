# Bamse – mitt samlarregister

En enkel webbapp för en personlig samling av den svenska serietidningen Bamse.

## Funktioner
- Årgångsvy för 1973–2026.
- Markera enskilda nummer som ägda.
- Markera alla eller avmarkera alla i vald årgång.
- Tydliga statusfärger: grönt = äger, rött = saknar efter att numret bedömts, grått = ej bedömt.
- Separat lista över alla tidningar med filter för år och status.
- Skick, anteckningar, eget omslagsfoto och bildlänk per nummer.
- Statistik, utskrift samt export/import av JSON-säkerhetskopia.
- Samma lagringsnyckel som tidigare version: `bamse-samlarregister-v1`.

## Viktigt om årgångarna
Årtal och nummer 1973–1998 är markerade som kontrollerade enligt det underlag som använts i projektet. 1999–2026 är fortfarande preliminära och behöver kontrolleras mot katalogen innan de kan betraktas som kompletta. Appen visar därför detta i årgångsvyn. Antalet poster är en arbetslista, inte ett påstående om att varje nummer är slutligt verifierat.

## Omslagsbilder
Appen skapar inte och återanvänder inte påhittade Bamse-omslag. Ett omslag visas bara om användaren har lagt till en bild eller bildlänk. Använd endast originalomslag från källor där du har rätt att använda bilderna. Ett privat GitHub-repo gör inte automatiskt att en publicerad GitHub Pages-sida blir privat.

## Lagring och inloggning
Detta är en statisk testversion. Uppgifter sparas i `localStorage` i den aktuella webbläsaren. Det finns ännu ingen riktig serverbaserad inloggning eller gemensam databas. Lägg därför inte upp känsliga uppgifter och exportera säkerhetskopia regelbundet. En lösenordskontroll som enbart ligger i JavaScript skulle inte vara säker.

## Publicera med GitHub Pages
Ladda upp `index.html` och `README.md` till repots rot och aktivera GitHub Pages enligt repots inställningar.

## Säkerhetskopia
Välj **Exportera register** för att spara en JSON-fil. **Importera register** läser tillbaka en sådan fil. Ta en export innan du byter version eller webbläsare.
