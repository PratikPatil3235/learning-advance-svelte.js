<!-- Posts.svelte -->
<script>
  import { onMount } from 'svelte';

  let posts = [];
  let loading = true;
  let error = null;

  onMount(async () => {
    try {
      const res = await fetch('https://jsonplaceholder.typicode.com/posts');
      if (!res.ok) throw new Error('Failed to fetch');
      posts = await res.json();
    } catch (err) {
      error = err.message;
    } finally {
      loading = false;
    }
  });
</script>

{#if loading}
  <p>Loading posts...</p>
{:else if error}
  <p style="color: red;">Error: {error}</p>
{:else}
  <ul>
    {#each posts as post}
      <li>
        <strong>{post.title}</strong>
        <p>{post.body}</p>
      </li>
    {/each}
  </ul>
{/if}
