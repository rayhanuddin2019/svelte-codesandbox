<script>
	let count = 0;
	let count2 = 0;
	function handleClick() {
	  count += 1;
	}
	function handleClick2() {
	  count2 += 2;
	}
</script>

<style>
	button {
	  background: red;
	  color: white;
	  border: none;
	  padding: 8px 12px;
	  border-radius: 2px;
	}
</style>

<button on:click={handleClick}>
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<hr/>
<button on:click={handleClick2}>
   Clicked {count2} {count2 === 1 ? 'time' : 'times'}
</button>