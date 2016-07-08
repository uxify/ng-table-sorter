# ng-table-sorter
Angular directive to sort a table


Simple table sorter to sort the columns in a html table.
Pure javascript and angularJS code.
Click to sort function.


1)Add the directive 'ng-table-Mod' to the html element.
   <table ng-table-Mod="asc">

2)Enclose the head part of the table under <thead></thead>
	<thead>
		<tr>
			<th>Sl no.</th>
			<th>Item</th>
		</tr>
	</thead>

3) Enclose the body part of the table under <tbody></tbody>
   <tbody>
				<tr>
					<td>1</td>
					<td>Angular</td>
				</tr>
				<tr>
					<td>2</td>
					<td>React</td>
				</tr>
		</tbody>
