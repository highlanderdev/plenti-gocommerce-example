<script>
  export let product;
</script>


<svelte:head>
  {@html '<script class="gocommerce-product" type="application/json">' + JSON.stringify(product) + '</script>' }
</svelte:head>
