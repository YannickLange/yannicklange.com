<script>
    import { onMount } from 'svelte';
    import { writable } from 'svelte/store';
    import mermaid from 'mermaid';

    let container;
    let rendered = writable(false);

    onMount(async () => {
        mermaid.initialize({ theme: 'neutral', startOnLoad: false });
        rendered.set(true); 
        setTimeout(async () => {
            await mermaid.run()
        }, 0)
    });
</script>

<div>
    {#if $rendered}
    <div class="mermaid">
        <slot/>
    </div>
    {:else}
    <div>
        <p></p>
    </div>
    {/if}
</div>

<style>

</style>
