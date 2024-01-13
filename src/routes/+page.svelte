<script>
    import '$lib/styles/style.css';
    import Portrait from '$lib/components/Portrait.svelte';
    import Diagram from '$lib/components/Diagram.svelte';
</script>

<Portrait/>
<h2>Yannick Lange</h2>
<p>hello</p>
<Diagram>
    flowchart TB 
        A & B --> C & D
</Diagram>

