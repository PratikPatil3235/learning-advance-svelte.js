<script>
  const names = [
    {
      firstName: "Bruce",
      lastName: "Wane",
    },
    {
      firstName: "Clark",
      lastName: "kent",
    },
    {
      firstName: "Berry",
      lastName: "Allen",
    },
  ];
</script>

<main>
    {#each names as name (name) }
        <h3><slot name="hero" firstName={name.firstName} lastName={name.lastName}/></h3>
    {/each}
</main>