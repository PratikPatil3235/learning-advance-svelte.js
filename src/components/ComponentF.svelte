<script>
  import { getContext } from "svelte";

  const username = getContext('username-context');
</script>

<h2>Child F Component</h2>
<h2>Child F UserName - {username}</h2>
