<script>
    import {createEventDispatcher} from 'svelte'
    const dispatch= createEventDispatcher()
</script>
<div>
    <h2>This is a popup</h2>
    <button on:click={()=>dispatch('close','Pratik')}>Close Popup</button>
</div>