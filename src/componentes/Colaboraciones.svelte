<script>
    export let colaboraciones = [
        { name: "Nike x Off-White", image: "./imagenes/nike_offwhite.png" },
        { name: "Adidas Campus Bad Bunny", image: "./imagenes/adidas_badbunny.png" },
        { name: "Nike x Travis Scott", image: "./imagenes/nike_travisscott.png" },
    ];
</script>

<style>
    .colaboraciones {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        gap: 1rem;
        margin: 2rem 0;
        text-align: center;
        align-items: center;
        color: #AD8A1F;
        font-weight: bold;
    }
    .colaboracion {
        text-align: center;
        max-width: 300px;
    }
    .colaboracion img {
        width: 100%;
        height: auto;
        border-radius: 10px;
        text-align: center;
    }
    .colaboracion p {
        width: 100%;
        height: auto;
        text-align: center;
        color: #AD8A1F;
        font-weight: bold;
    }

    h2{
        text-align: center;
        font-size: bold;
        font-size: 50px;
        color: #AD8A1F;
    }
</style>

<h2>Colaboraciones</h2>
<section class="colaboraciones">
    {#each colaboraciones as colaboracion}
        <div class="colaboracion">
            <img src={colaboracion.image} alt={colaboracion.name}>
            <p>{colaboracion.name}</p>
        </div>
    {/each}
</section>
