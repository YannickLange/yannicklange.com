<script>
    export let data;
</script>

<ul>
    {#each data.posts as post}
        <li>
            <h2>
                <a href={post.path}>
                    {post.meta.title}
                </a>
            </h2>
            published {post.meta.date}
        </li>
    {/each}
</ul>
