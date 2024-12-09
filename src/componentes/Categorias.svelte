<script>
    export let categorias = [
        { name: "Jordan", image: "./imagenes/jordan9.png" },
        { name: "Yeezy", image: "./imagenes/yeezy.png" },
        { name: "Nike", image: "./imagenes/nike.png" },
        { name: "Adidas", image: "./imagenes/adidas.png" },
        { name: "Gucci", image: "./imagenes/gucci.png" },
        { name: "Louis vuitton", image: "./imagenes/louisvuitton.png" },
        { name: "Balenciaga", image: "./imagenes/balenciaga.png" },
        { name: "New Balance", image: "./imagenes/newbalance.png" },
    ];
</script>

<style>
    .categorias {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        gap: 200px;
        margin: 50px;
    }
    .categoria {
        text-align: center;
        max-width: 150px;
    }
    .categoria img {
        width: 100%;
        height: auto;
        border-radius: 10px;
    }
</style>

<section class="categorias">
    {#each categorias as categoria}
        <div class="categoria">
            <img src={categoria.image} alt={categoria.name}>
            <p>{categoria.name}</p>
        </div>
    {/each}
</section>
