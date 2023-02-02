<script>    
    const blogs = [
        ["Let's write a blog in Rust - Part 2", "2023-02-02", 2],
        ["Let's write a blog in Rust - Part 1", "2023-01-27", 1],
    ]
</script>

<h1 class=title>Blogs</h1>
<ul>
    {#each blogs as blog}
        <li><a href={`/blog/${blog[2]}`}>{blog[0]}  -  {blog[1]}</a></li>
    {/each}
</ul>