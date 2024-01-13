<script>
    import '$lib/styles/style.css';
    import Portrait from '$lib/components/Portrait.svelte';
    import Code from '$lib/components/Code.svelte';
    let mermaidCode = 'flowchart TB; A & B --> C & D';
</script>

<Portrait/>
<h2>Yannick Lange</h2>
<p>hello</p>
<Code code={mermaidCode}/>


