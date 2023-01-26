<script>
  
  export let data

  // console.log(data);

  const {flowers} = data
  console.log(flowers);
</script>

<div class="container">
  {#each flowers as item}
    <p>{item.species}</p>
  {/each}
</div>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		gap: 2em;
		padding: 2em;
	}
	img {
		height: 300px;
		width: 100%;
		object-fit: cover;
		object-position: center;
	}
</style>