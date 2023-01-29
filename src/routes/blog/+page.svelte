<script>    
    const blogs = [
        ["Let's write a blog in Rust - Part 1", "2023-01-27"]
    ]
</script>

<h1 class=title>Blogs</h1>
<ul>
    {#each blogs as blog, i}
        <li><a href={`/blog/${i+1}`}>{blog[0]}  -  {blog[1]}</a></li>
    {/each}
</ul>

<style>

    li {
        list-style-type: disc;
    }
</style>