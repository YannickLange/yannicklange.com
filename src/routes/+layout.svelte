<script>
    import '$lib/styles/style.css';
    import Header from '$lib/components/Header.svelte';
</script>

<style>
  .container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    height: 100vh;
  }

  .content {
    flex-grow: 1;
    max-width: 800px; /* Adjust the maximum width of the content area */
    padding: 20px;
    box-sizing: border-box;
  }
</style>

<main>
    <div class="container">
        <Header/>
        <div class="content">
            <slot/>
        </div>
    </div>
</main>

