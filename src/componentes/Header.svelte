<script>
  let firma = "./imagenes/firma.jpg";
  let logoCarrito = './imagenes/logo-carrito.png'
</script>

<div class="contenedor-header">
  <div class="Logo-marca">
    <img src={firma} alt="La firma de la página" />
    <h1>ZASHOP</h1>
  </div>
  <div class="header-nav">
    <a href="#">Ofertas</a>
    <a href="#">Tienda</a>
    <a href="#">Ayuda</a>
    <a href="#">Log-in</a>
    
  </div>
  <button class="boton-carrito"> <img src={logoCarrito} alt="la imagen del carrito">CARRITO</button>
</div>

<style>
  .contenedor-header {
    display: flex;
    flex-wrap: wrap;
    color: #AD8A1F;
    width: 100%;
  }
  
  .Logo-marca{
    display: flex;
    flex-wrap: wrap;
    color: #AD8A1F;
  }
  a{
    text-decoration: none; 
    color: #AD8A1F;
    margin: 10px;
  }
  .header-nav{
    margin-top: 35px;
    margin-left: 500px;
  }
  .boton-carrito{
    color: #AD8A1F;
    font-family: League Gothic;
    border-radius: 15px;
    height: 30px;
    border: 0.5px solid #AD8A1F ;
    margin-top: 25px;
    margin-left: 10px;
  }
  .boton-carrito img{
    height: 20px;
    margin-top: 5px;
  }

  
</style>
