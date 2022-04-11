<svelte:head>
  <title>Content Manager</title>
</svelte:head>


<script>
  import { onMount } from 'svelte';
  onMount(async() => {
    const CMS = await import('netlify-cms-app/dist/netlify-cms-app')
    if(window){
      CMS.init()
    }
  })
</script>