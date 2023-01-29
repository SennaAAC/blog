<script>
    let theme = "🌅"

    const change_theme = () => {
        let root = document.documentElement;
        if (root.getAttribute("data-theme") === "dark") {
            root.setAttribute("data-theme", "light");
            theme = "🌇";
        } else {
            root.setAttribute("data-theme", "dark");
            theme = "🌅";
        }

    }
</script>

<nav>
    <ul>
        <li>
            <a href="/">Home</a>
        </li>
        <li>
            <a href="/blog">Blogs</a>
        </li>
    </ul>
    <ul>
        <li><button on:click={change_theme}>{theme}</button> </li>
    </ul>
</nav>

<style>
    nav {
        background-color: rgba(0, 0, 0, 1.0);
        padding-left: 20px;
        position: fixed;
        top:0;
        width: 100%;
        overflow:hidden;
    }

    li {
        padding:7px
    }

    button {
        background-color: inherit;
        border:none;
        padding-right: 30px;
        box-shadow: none;
    }

</style>