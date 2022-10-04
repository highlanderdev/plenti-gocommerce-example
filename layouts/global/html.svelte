<script>
  import Head from './head.svelte';

  export let content, layout, allContent, user, adminMenu;
</script>

<html lang="en">
<Head title={content.filename} />
<body>
  {#if user && $user.isAuthenticated}
    <svelte:component this={adminMenu} {user} bind:content/>
  {/if}
  <main>
    <svelte:component this={layout} {...content.fields} {allContent} />
  </main>
</body>
</html>
