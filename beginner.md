# Begynder
Denne løsningsmetode er opdelt i otte forskellige trin. Disse trin kan beskrives som:

1. Cross
2. First Layer Corners
3. Second Layer Edges	
4. Cross on U-face	
5. Orient Edges in U-Layer
6. Permute Edges in U-Layer
7. Permute corners in U-Layer
8. Orient corners in U-Layer		

Der findes en alternativ måde til løsning af det sidste lag, det kræver man to algoritmer mere. Læs mere om 4 Look Last Layer (4LLL) [her](awesome/4lll.md).

## Cross
I første del af løsningen skal der dannes et kryds på terningen. Det er ligemeget hvilket farve krydset er, dog er det vigtigt kanterne placeres så de stemmer med centrene på de andre sider.
	
Der findes ingen algoritmer til at lave krydset med, det skal ske intuitivt. Netop derfor har de fleste speedcubere en favorit farve hvis kryds de laver hver gang. Det gør det nemmere at genkende hjørner og kanter når de første to lag løses med avancerede metoder.

Det er derfor en god idé at finde en krydsfarve man kan lide, og holde sig til den.

<table class="cube_table_content">	
	<tr>	
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_cross_up.png" />	
		</td>
	</tr>	
	<tr>		
		<td class="cube_table_content_td">Terningen skal se sådan ud, når du er færdig med dette trin.</td>		
	</tr>		
</table>		
		
## First Layer Corners
I næste trin i løsningen skal hjørnerne placeres på deres respektive pladser. Det er vigtigt at forstå at hjørner, ligesom kanter, har en unik placering på terningen. Det er derfor vigtigt at sørge for at ikke blot krydsfarven, men også lagfarverne passer, når hjørnerne placeres.

Når et hjørne er identificeret, drejes det hen på den position, der er lige under den rigtig placering for hjørnet, hvorefter følgende algoritme udføres:

> R' D' R D

Den ovenstående algoritme udføres indtil hjørnet er på plads. Når alle hjørner er placeret fortsættes der på nøste trin.
		
<table class="cube_table_content">		
	<tr>
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_first_layer_up.png" />		
		</td>
	<tr>
		<td class="cube_table_content_td">Nu er hele første lag på terningen løst</td>		
	</tr>		
</tr>		
</table>		
		
## Second Layer Edges
På dette trin skal de to første lag færdiggøres, der findes to cases der læses på næsten samme måde, faktisk er algoritmen bare spejlvendt. Fælles for begge cases er at kanten, som skal placeres drejes hen, så den passer med centerfarven der skal være F-siden. Herefter benyttes en af to algoritmer, alt efter og kanten skal til.	

Hvis kanten skal til venstre udføres algoritmen:
> U' L' U L U F U' F'
	
Hvis kanten derimod skal til højre udføres følgende algoritme:
> U R U' R' U' F' U F
		
Fortsæt med at benytte de to algoritmer, til at alle kanterne i den det anden lag er på plads. Det kan ske, at en af kanterne er placeret på sin rigtige plads, men vendt forkert. Hvis dette er tilfældet byttes kanten bare ud med en tilfældig kant fra top-laget.

<table class="cube_table_content">		
	<tr>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_second_layer_edge_left.png" />		
		</td>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_second_layer_edge_right.png" />		
		</td>		
	</tr>		
	<tr>		
		<td class="cube_table_content_td" colspan="2">Her ses de to cases, der findes i dette trin.<br />Første case: kant til venstre, anden case: kant til højre</td>		
	</tr>		
</table>

<table class="cube_table_content">		
	<tr>
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_second_layer_complete.png" />		
		</td>		
	</tr>		
	<tr>		
		<td class="cube_table_content_td" colspan="2">Nu er de to første lag på terningen løst.</td>		
	</tr>		
</table>	

<h2>Orient Edges in U-Layer</h2>		
<p>Dette trin er starten på at fuldende det sidste lag. Faktisk er det ret nemt, da der kun er en algoritme at lære:</p>		
<p class="cube_algorithm_p">F R U R' U' F'</p>		
<p>Der er dog noget, der skal holdes styr på, fire mønstre som de fire kanter i top-laget danner. Det er vigtigt at algoritmen bliver udført mens det pågældende mønster er placeret som de tre nedenstående illustrationer:</p>		

<table class="cube_table_content">		
	<tr>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_top_layer_case_1.png" />		
		</td>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_top_layer_case_2.png" />		
		</td>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_top_layer_case_3.png" />		
		</td>		
	</tr>		
	<tr>		
		<td class="cube_table_content_td" colspan="3">Her ses de tre cases, der findes i dette trin. Første case: ingen kanter orienteret korrekt, anden case: to kanter korrekt orienteret diagonalt, tredje case: to kanter korrekt orienteret parallelt</td>		
	</tr>		
</table>

Hvis den første case optræder, udfør da algoritmen en gang for at få den anden case, udfør algoritmen en gang mere og top-krydset vil være løst. Hvis tilfældet er den anden case, kommer den tredje case og derefter top krydset.

<table class="cube_table_content">		
	<tr>
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_top_cross_complete.png" />	
		</td>		
	</tr>		
	<tr>		
		<td class="cube_table_content_td">Krydset på toppen af terningen er nu løst.</td>		
	</tr>		
</table>		
		
## Permute Edges in U-Layer
På dette trin skal kanterne placers på deres rigtige pladser, her der er der igen kun en algoritme at lære:

> R U R' U R U2 R'

Algoritmen bytter to kanter diagonalt og vender tre hjørner. Hjørnerne betyder intet i denne sammenhæng da vi kun koncentrere os om kanterne for kompleksitetens skyld. Hjørnerne kan være placeret på tre forskellige måder: Parallelt, diagonalt eller løst.

Det er vigtigt, at algoritmen bliver udført mens det pågældende mønster er placeret som de tre nedenstående illustrationer:	
		
<table class="cube_table_content">		
	<tr>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_permute_top_layer_cross_case_1.png" />		
		</td>		
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_permute_top_layer_cross_case_2.png" />		
		</td>
	</tr>		
	<tr>		
		<td class="cube_table_content_td" colspan="2">Her ses de to cases der findes på dette trin.<br /> Grøn indikerer, at kanten er korrekt placeret. Rød indikerer, at kanten ikke er korrekt placeret.</td>	
	</tr>
</table>				
		
## Permute corners in U-Layer
Når alle kanterne på terningen er sat på plads mangles der nu kun de fire sidste hjørner i top-laget. Her er det vigtigt at forstå forskellen på placering og orientering, det vi er ude efter er at få hjørnerne på deres respektive pladser.	

Dette opnåes med følgende algoritme:
> U R U' L' U R' U' L

Hvis et af hjørnerne er placeret rigtigt, skal dette være placeret på URF.
<table class="cube_table_content">		
	<tr>
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_urf_correct_oriented.png" />		
		</td>	
		<td class="cube_table_content_td">		
			<img src="../images/beginner/rubiks_cube_urf_incorrect_oriented.png" />		
		</td>		
	<tr>		
		<td class="cube_table_content_td" colspan="2">Her ses to forskellige cases, begge hjørner er placeret korrekt, og er derfor korrekt placeret på URF placeringen.</td>		
	</tr>		
</table>		
		
## Orient corners in U-Layer
Til sidst skal de resterende hjørner roteres så top-laget bliver løst. Der er ikke nogle nye algoritmer at lære her, da vi benytter den sammen algoritme som i første trin, der roterer et hjørne:
> R' D' R D
		
Når hjørnet er læst, drejes U-laget til der atter er et uløst hjørne, hvorefter ovenstående algoritme udføres til alle hjørner vender korrekt.

Hvis et af hjørnerne er placeret rigtigt, skal dette være placeret på URF.
		
## Cheat sheet
<a href="cheat-sheet-beginner.pdf">Download</a> et cheat sheet med alle algoritmerne til denne løsning, lige til at printe ud og stikke i lommen.