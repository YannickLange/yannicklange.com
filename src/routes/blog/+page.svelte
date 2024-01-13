<style>
    ul {
        margin: 0px;
    }

    li {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 10px; /* Adjust spacing between list items */
    }
</style>
<script>
    export let data;
</script>

<ul>
    {#each data.posts as post}
        <li>
            <a href={post.path}>
                {post.meta.title}
            </a>
            <span>
                {post.meta.date}
            </span>
        </li>
    {/each}
</ul>
