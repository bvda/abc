# Alternativ løsningsmetode til sidste lag</h1>
Følg den ovenstående guide til der forefindes et kryds på U-laget på terningen. Her efter vil en af følgende mønstre være i U-laget:
		
<table class="cube_table">
	<th colspan="4">OLL cases</th>
	<tr>
		<td class="cube_table_cube_td">
			<img src="../images/beginner/oll-case04.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 1: Forlygter
		</td>
		<td class="cube_table_cube_td">
			<img src="../images/beginner/oll-case05.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 2: Fluesmækker
		</td>
	</tr>
	<tr>
		<td class="cube_table_cube_td">
			<img src="../images/beginner/oll-case06.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 3: Butterfly
		</td>
		<td class="cube_table_cube_td">
			<img src="../../images/beginner/oll-case07.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 4: Sune
		</td>
	</tr>
	<tr>
		<td class="cube_table_cube_td">
			<img src="../../images/beginner/oll-case08.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 5: Anti-sune
		</td>
		<td class="cube_table_cube_td">
			<img src="../../images/beginner/oll-case09.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 6: Motorcykel
		</td>
	</tr>
	<tr>
		<td class="cube_table_cube_td">
			<img src="../../images/beginner/oll-case10.png">
		</td>
		<td class="cube_table_algorithm_td">
			Case 7: Bil
		</td>
	</tr>
</table>
		
		<p>Orientér U-laget således at et af den ovenstående mønstre vender som på illustrationen (Det nederste lag er altid F-laget på terningen). Herefter benyttes følgende algoritme til at orienterer hjørnerne:</p>
		
		<p class="cube_algorithm_p">R U R' U R U2 R'</p>

		<p>Det er vigtigt at nævne, at det ofte er nødvendigt at udføre oevnstående algoritmer flere gange, da den cycler igennem de forskellige mønstre.</p> 
		
		<p>Vær opmærksom på at orientere det nye mønster, så det vender rigtig jævnfør illustrationerne i den ovenstående tabel.</p>
		
		<h2>Corner permutation</h2>
		
		<p>Efter orientering af U-laget skal hjørnerne sættes på plads. Dette gøres ved at benytte nedenstående algoritme:</p>
		
		<p class="cube_algorithm_p">R' F R' B2 R F' R' B2 R2</p>
		
		<p>Det er vigtigt, at hvis der er "forlygter" på terningen, det vil sige at to hjørner vender således at to hjørner har samme farve i U-laget, skal være på B-siden af terningen. Hvis det ikke er tilfældet, kan ovenstående algoritme udføres en gang hvorpå der vil komme mønstret vil opstå i U-laget.</p>
		
		<table class="cube_table_content">		
			<tr>
				<td class="cube_table_content_td">		
					<img src="../../images/beginner/rubiks_cube_oll_headlights.png" />		
				</td>			
			<tr>		
				<td class="cube_table_content_td" colspan="2">Orientér terningen så de to hjørnestykker med samme farve er på B-siden.</td>		
			</tr>		
		</table>
		
		<h2>Edge permutation</h2>
		
		<p>Når hjørnestykkerne er løst skal kantstykkerne til sidst på plads, dette gøres med nedenstående algortime:</p>
		
		<p class="cube_algorithm_p">R U' R U R U R U' R' U' R2</p>
		
		<p>Hvis der ikke er et løst kantstykke, udføres algoritmen en gang for at få det. Algoritmen cykler tre kanter mod uret, derfor kan det nødvendigt at udføre den to gange for at løse terningen.</p>
		
		<table class="cube_table_content">		
			<tr>
				<td class="cube_table_content_td">		
					<img src="../../images/beginner/pll-case06.png" />		
				</td>
			</tr>
			<tr>		
			<td class="cube_table_content_td" colspan="2">Orientér terningen så det kantstykke er på B-siden.</td>		
			</tr>		
		</table>
		
		</div>
		<div id="footer">	
		<?php include("../../includes/footer.php"); ?>
		</div>
		</div>