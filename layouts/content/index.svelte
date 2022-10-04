<script>
	export let title;
  import { onMount } from "svelte";
  import GoCommerce from "gocommerce-js";

  // This needs to happen clientside only.
  // onMount prevents SSR from trying to evaluate this
  onMount(async () => {
    const commerce = new GoCommerce({
      APIUrl: "http://localhost:9111"
    });
  });
</script>

<h1>{title}</h1>

<style>
	h1 {
		font-family: Helvetica, sans-serif;
	}
</style>
