<script>
	export let title;

  import GoCommerce from "gocommerce-js";
  // This Causes a reference error, but without it you
  //   can make an instance of GoCommerce in web browser on index page
  // const commerce = new GoCommerce({
  //   APIUrl: "http://localhost:9111"
  // });
</script>

<h1>{title}</h1>

<style>
	h1 {
		font-family: Helvetica, sans-serif;
	}
</style>