---
Title: Laddningsanalys
Template: analysis
---
Laddningsanalys
===
I denna rapport skall tre webbplatser analyseras om deras laddningshastighet och storlek

Urval
---
De sidor som kommer att analyseras är följande <a href="https://www.youtube.com">youtube.com</a>, <a href="https://www.netonnet.se">netonnet.se</a> och <a href="https://www.github.com">github.com</a>
Detta då olika sidor med olika ändamål är intressant att analysera.

Metod
---
För varje sida börjades det med att först ta en skärmbild. Efter det kördes varje sida genom PageSpeed Insights. Från verktyget
PageSpeed Insights noterades varje sidas poäng, FCP (First Contentful Paint), LCP (Largest Contentful Paint) och Speed Index. Detta gjordes båda för desktop/dator och mobil för sidorna. Sen genom devtools i webläsarens noterades också, utöver PageSpeed Insights värderna, laddningstid, resursstorlek, och överförd resursstorlek. Detta gjordes med cache disbled i devtools.

Resultat
---
Här kommer resultat om de olika webbplatserna.
<div class="embed-container">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRnbEmDcuU3AfCsqWoQW4f6z3ZLaz7YV9ScALTk9CZ6QTUk047WJRrujcnTEC9FSoIrI9xwdVanLJFc/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</div>

### youtube.com

<img src="%base_url%/image/youtube.png" class="analysis-image">

Betyg: 38 (dator), 46 (mobil).
FCP: 1s (dator), 5.9s (mobil).
LCP: 4.3s (dator), 8s (mobil).
Speed Index: 5.2s (dator), 5.9s (Mobil).
Laddningstid: 2.45s.
Storlek: 21.8 MB.
Överförda Resurser: 6.8 MB.

### netonnet.se

<img src="%base_url%/assets/img/netonnet.png" class="analysis-image">

Betyg: 72 (dator), 57 (mobil).
FCP: 0.8s (dator), 4.2s (mobil).
LCP: 0.9s (dator), 10.2s (mobil).
Speed Index: 2.5s (dator), 6.7s (Mobil).
Laddningstid: 1.08s.
Storlek: 6 MB.
Överförda Resurser: 3.3 MB.
### github.com

<img src="%base_url%/assets/img/github.png" class="analysis-image">

Betyg: 62 (dator), 56 (mobil).
FCP: 0.9s (dator), 3.1s (mobil).
LCP: 1s (dator), 3.5s (mobil).
Speed Index: 2.5s (dator), 7.4s (Mobil).
Laddningstid: 1.29s.
Storlek: 6.7 MB.
Överförda Resurser: 1.7 MB.

Analys och Diskussion
---

Youtube hade det sämsta resultatet av alla webbsidor, men detta är ändå förstålligt då den har alltid nytt innehåll att visa upp
och den ska ladda in mycket media (bilder) och allt ska hämtas och skrivas ut istället för andra webbsidor som kan ha mer i html från start. Youtube gör ändå att bra jobb med att endast ha 21.8 MB för alla bilder då vissa webbsidorn kan ha en bild som är lika stor som hela youtube startsida. Det som skulle kunna göra sidan snabbare är såklart mindre upplösta bilder och mindre videos som visas samtidigt. Sen i PageSpeed Ingsights visas att det finns en render blocking resource som skulle kunnan ändras för att rendera snabbare.

Netonnet hade det bästa resultatet som jag trodde skulle vara i mitten då den också laddar in massa bilder och information som inte kan skrivas direkt in i html filen. Fungerar lite samma som Youtube med massa objekt med en titel och en bild som laddas in
Det är samma som i youtube att minska bilders upplösning och kvalité för bilder. 

Github som jag trodde skulle vara den snabbaste då det är mindre bilder och annan data som ska hämtas och visas. Men den tog längre tid och hade större storlek på sidan. I Github var det väldigt många scripts som laddades in. Varje script tog 25ms så det blir många millesekunder när 20+ scritps ska laddas in. Kollar man på namn på filer verkar de använda React så det är mycket som ska laddas in.

Det vanligaste sättet är att optimera bilder mer och se till att rendering inte blockeras av scripts.

Rankning:
<ol>
    <li>Netonnet</li>
    <li>Github</li>
    <li>Youtube</li>
</ol>

Jag skulle säga att den absoluta laddningstod som jag sätter som gräns för att vara en snabb inladdning är 2s. Långsam efter 4s.
Alla sidor förutom Youtube laddade in på under 2s. Även om Youtube inte laddade in på under 2s var det under 3s och upplevdes då inte som långsam. Så generellt tyckte jag att de laddade in snabbt.

Övrigt
---
Casper Berneklint