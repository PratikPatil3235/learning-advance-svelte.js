<script>
    import {createEventDispatcher} from 'svelte'

    const dispatch=createEventDispatcher();
    function greet(event){
        dispatch('greet', 'Hello')
    }
</script>

<button on:click={greet}>Greet</button>