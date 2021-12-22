<script>
    let players = [
        {
            "firstname": "Alexander",
            "lastname": "Dahlquist",
            "points": 12
        },
        {
            "firstname": "Johan",
            "lastname": "Andersson",
            "points": 10
        },
        {
            "firstname": "Kalle",
            "lastname": "Paulsson",
            "points": 8
        }
    ];
</script>

<table class="table">
	<thead>
		<tr>
			<th scope="col">#</th>
			<th scope="col">Name</th>
			<th scope="col">Last</th>
			<th scope="col">Points</th>
		</tr>
	</thead>
	<tbody>
        {#each players as player, index}
            <tr>
                <th scope="row">{index + 1}</th>
                <td>{player.firstname}</td>
                <td>{player.lastname}</td>
                <td>{player.points}</td>
            </tr>
        {/each}
	</tbody>
</table>
