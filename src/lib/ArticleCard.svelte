<script>
    export let name;
    export let link;
    export let date;
</script>

<a href={link}>
    <article class=card>
        <h3>{name}</h3>
        <h3>{date}</h3>
    </article>
</a>

<style>
    .card {
        text-align: center;
        box-shadow: rgba(0, 0, 0, 0.06) 0px 2px 4px, rgba(0, 0, 0, 0.05) 0px 0.5px 1px;
        transition: all .2s ease-in-out;
        margin-top: 5px;
        margin-bottom: 5px;
    }

    h3 {
        font-size: 20px;
    }

    .card:hover {
        box-shadow: rgba(0, 0, 0, 0.22) 0px 19px 43px, rgba(0, 0, 0, 0.18) 0px 4px 11px;
        cursor: pointer;
        transform: translate3d(0px, -2px, 0px);
    }

    a:hover {
        text-decoration: none;
    }
</style>