<script lang="ts">
	export let count: number = 2;
	let times = 2;
	$: result = count * times;
</script>

<div>{count} x {times} = {result}</div>
<button
	on:click={() => {
		times += 1;
	}}>+1</button
>
