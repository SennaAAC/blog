<script>
    import Blog from "./blog.md";
    let title = "Let's write a blog in Rust - Part 3"
    let date = "2023-02-01"
    let subtitle = "This is actually just a rewrite of the last post ... sorry."
    let topics = ["Rust", "Tauri", "Svelte", "Sveltekit"]
</script>

<p class="date">{date}</p>
<h1>{title}</h1>
<h2>{subtitle}</h2>
<h2>{topics.join(" • ")}</h2>
<hr>
<Blog></Blog>

<style>
    h1, h2 {
        margin-top: 0px;
        text-align: center;
        padding-bottom: 20px;
    }
    p {
        padding-top: 20px;
    }

    .date {
        color:grey;
    }

    hr {
        padding-bottom: 1px;
    }

</style>