<script>
    import { onMount } from 'svelte';
    import mermaid from 'mermaid';

    export let code = '';

    onMount(() => {
        mermaid.initialize({ startOnLoad: true });
        mermaid.contentLoaded();
    });
</script>

<div class="mermaid">
    {code}
</div>

<style>

</style>
