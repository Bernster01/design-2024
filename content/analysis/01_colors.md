---
Title: Färganalys
Template: analysis
---
Färganalys
===
I denna rapport skall tre webbplatser analyseras om färgschema och font val

Urval
---
De sidor som kommer att analyseras är följande <a href="https://www.php.net">php.net</a>, <a href="https://developer.mozilla.org/en-US/">developer.mozilla.org</a> och <a href="https://www.python.org">python.org</a>
Detta genom att först välja något kopplat till kursen/kurspaketen. Så då blev det att kolla in webbplatser om de tekniker som används i kursen/kurspaketen.

Metod
---
För varje sida börjades det med att först ta en skärmbild. Efter det för att extrahera de olika färgerna användes WAVE plugin till chrome. Från detta plugin användes en color picker. Dessa färgkoder sparades ner. Efter det var det att ta fram fonter och då användes det inbyggda devtools med att inspektera de olika headings och brödtext för att se vilka fonter som används. Alla färger per sida samlades för att kunnna se vilket färgschema som använts.

Resultat
---
Här kommer resultat om de olika webbplatserna.

### PHP.net

<img src="%base_url%/assets/img/PHP.png" class="analysis-image">

<table class="analysis-table" style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #4F5B93">
<td style="height: 50px; width: 50px; background-color: #2B2B2B">
<td style="height: 50px; width: 50px; background-color: #F2F2F2">
</tr>
</table>
Oklart färgschema men möjligen ett monokromatiskt  tema eller ett akromatiskt tema med en extra färg
#### fonter

h1 - Fira Sans <br>
h2 - Fira Sans <br>
h3 - Fira Sans <br>
brödtext - Fira Sans <br>

Jag tror att de försöker se modern ut och lyckas med det genom sina val.
### developer.mozilla.org

<img src="%base_url%/assets/img/MDN.png" class="analysis-image">


<table class="analysis-table" style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #040404">
<td style="height: 50px; width: 50px; background-color: #1B1B1B">
<td style="height: 50px; width: 50px; background-color: #313131">
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
</tr>
</table>

Ett akromatiskt tema

#### fonter

h1 - Inter <br>
h2 - Inter <br>
h3 - Inter <br>
brödtext - Inter <br>
Jag tror att de lyckas med att försöka se åt som dokumentation genom större kontraster.
### python.org

<img src="%base_url%/assets/img/PYTHON.png" class="analysis-image">


<table class="analysis-table" style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #1E2933">
<td style="height: 50px; width: 50px; background-color: #204463">
<td style="height: 50px; width: 50px; background-color: #FFD343">
<td style="height: 50px; width: 50px; background-color: #E6E8EA">
<td style="height: 50px; width: 50px; background-color: #FAFAFA">
</tr>
</table>
Ett complementary färgschema
#### fonter

h1 - Oklart är en bild <br>
h2 - Flux Regular <br>
h3 - SourceSansProRegular <br>
brödtext - SourceSansProRegular <br>
Jag tror att de försöker se lite gammeldags ut och tycker de gör det genom färgval och border färger som ger en gammal windows känsla.

Analys och Diskussion
---
Det första jag la märke till var att 2 av 3 använda samma font för sina rubriker och brödtext vilket i tidigare kurser inte rekommmenderas. Utan det har rekomenderats att köra olika för att fåd et att vara bättre. Endast python.org hade olika, däremot hade de ingen h1 med text utan det var en bild i h1 taggen. Medans python.org och mdn hade tydliga teman hade jag svårare att säga vad PHP kör för tema, men jag gillar PHP mest utav de 3. Jag tycker PHP ger en modern känsla och ren känsla. Jag föredrar mer monokromatiskt teman, tycker att de är skönare att titta på. MDN tycker jag har för hög kontrast för min smak. Det känns lite vasst att titta på. Python tycker jag ser för omodern ut för min smak, även om jag tycker de uppfylelr profilen av programmvara. 
Jag tycker att MDN är den jobbigaste att titta på då den blir för vass i mina ögen sen är det Python då jag tycker att designen är något ful och PHP är det bästa av dess 3 i mina ögon.

Det jag tycker jag fått fram med denna lila studie är att färg gör stor skillnad i hur iallfall jag uppfattar sidan. Nu kan det självklart vara så att de försöker visa en annan profil än den jag tror. Det beror på vad de som designat tycker om de olika färgkombinationerna och vilken känsla de får utav det.

Övrigt
---
Casper Berneklint