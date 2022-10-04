<script>
  export let allContent;

  let products = allContent.filter(content => content.type === 'products');
</script>

{#each products as product}
  {JSON.stringify(product)}
  <br><br>
{/each}
