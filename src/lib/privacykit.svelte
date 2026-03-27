<script>
    let props = $props();
    // svelte-ignore state_referenced_locally
        let policy = $state(props.policy);
    console.log(policy);
</script>
{#each policy as x}
<h2></h2>
{/each}