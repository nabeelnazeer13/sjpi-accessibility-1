# sjpi-accessibility-1


Den här webbplatsen hade flera problem, från dålig layout, distraherande element och riktigt svårnavigerade sektioner. HTML-koden är inte tillgänglighetsfokuserad och CSS-koden var avsiktligt förvirrande. Allt från teckensnittet till färgändringarna till JavaScript-tidsblockeringen gjorde att webbplatsen rankade riktigt lågt i Lighthouse.

Lighthouse report - 
Performance¨- 47
Accesbility - 81
Best practises -50
SEO - 82

Problem
Två <title>-taggar används.
Navigeringen är byggd med <span>-element istället för en lista.
En <button> innehåller ett <a>, vilket är ogiltig interaktiv kapsling.
Textinmatningen har ingen korrekt synlig <label>.
En klickbar <div> används istället för en riktig <button>.
Det finns en tom <h1>.
<marquee> är deprecated
Bilder presenteras som klickbart innehåll utan länkar eller knappar.
Cursor är inte pointer för klickbar element
Rörelse, blinkande, rotation, stort avstånd och tung textformatering minskar läsbarheten.
JavaScript blockerar huvudtråden, ändrar färger konstant, använder document.write() och stör webbläsarens normala beteende.

Vad jag gjorde
Använd semantiska landmärken: <header>, <nav>, <main>, <section>, <article>, <footer>.
Lägg till korrekta etiketter och tillgängliga namn i formulärkontroller.
Ersätt falska knappar och klickbara divs med riktiga knappar eller länkar.
Lägg till alt-text för informativa bilder och alt="" för dekorativa.
Ta bort blinkande, automatiskt flyttande, vilseledande annonsinnehåll och blockerande JavaScript.
Förbättra läsbarheten med lugnare färger, normalt avstånd, synliga fokusstilar och understrukna länkar.

Lighthouse report nu
Performance¨- 97
Accesbility - 100
Best practises -100
SEO - 100

Det svåraste med detta var CSS för mig. HTML-koden var lättare att läsa och se vad som var fel, men CSS-koden var så rörig och kaotisk att jag till slut bestämde mig för att göra om den från grunden.