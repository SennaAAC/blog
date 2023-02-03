<script>    

    import ArticleCard from "$lib/ArticleCard.svelte";
    const blogs = [
        ["Let's write a blog in Rust - Part 2", "2023-02-02", 2],
        ["Let's write a blog in Rust - Part 1", "2023-01-27", 1],
    ]
</script>

<h1 class=title>Blogs</h1>
<div class=article-grid> 
    {#each blogs as blog}
         <ArticleCard name={blog[0]} date={blog[1]} link={`/blog/${blog[2]}`}></ArticleCard>
    {/each}
</div>

<style>

    .title {
        text-align: center;
    }
    .article-grid {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 10px;
    }
</style>