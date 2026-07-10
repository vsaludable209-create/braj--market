
<!DOCTYPE html>
<html lang="es">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Brajá Market</title>

<style>

*{
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
}

body{
margin:0;
background:#faf7ef;
color:#333;
}


/* ENCABEZADO */

header{

background:linear-gradient(135deg,#557a46,#8db255);
color:white;
padding:40px 20px;
text-align:center;

}

header h1{

font-size:45px;
margin:0;

}

header p{

font-size:20px;

}


/* MENU */

.menu{

display:flex;
justify-content:center;
gap:15px;
padding:20px;
flex-wrap:wrap;

}


.menu button{

border:none;
background:#e7c35a;
padding:12px 25px;
border-radius:30px;
cursor:pointer;
font-weight:bold;

}


/* BUSCADOR */

.buscar{

text-align:center;
padding:20px;

}


.buscar input{

width:80%;
max-width:500px;
padding:15px;
border-radius:30px;
border:1px solid #ccc;
font-size:16px;

}


/* BANNER */

.banner{

background:#fff3c4;
padding:30px;
text-align:center;
font-size:24px;

}



/* PRODUCTOS */

.contenedor{

display:grid;
grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
gap:25px;
padding:40px;

}


.producto{

background:white;
border-radius:20px;
overflow:hidden;
box-shadow:0 5px 15px rgba(0,0,0,.15);
transition:.3s;

}


.producto:hover{

transform:translateY(-8px);

}



.producto img{

width:100%;
height:220px;
object-fit:cover;

}


.info{

padding:20px;

}


.info h2{

color:#557a46;

}


.precio{

font-size:22px;
font-weight:bold;
color:#d39b00;

}


.btn{

display:block;
text-align:center;
background:#25D366;
color:white;
padding:12px;
border-radius:20px;
text-decoration:none;
margin-top:15px;

}



/* CANASTAS */

.canastas{

background:#557a46;
color:white;
padding:35px;
text-align:center;

}


.canastas h2{

font-size:30px;

}


/* FOOTER */

footer{

background:#333;
color:white;
padding:20px;
text-align:center;

}


</style>

</head>


<body>


<header>

<h1>🥬 Brajá Market</h1>

<p>Alimentos de calidad a tu hogar</p>

</header>



<div class="menu">

<button>🥕 Verduras</button>
<button>🍎 Frutas</button>
<button>🌱 Orgánicos</button>
<button>🛒 Canastas</button>

</div>



<div class="buscar">

<input 
type="text" 
placeholder="Buscar productos...">

</div>




<div class="banner">

🌱 Productos frescos seleccionados cada semana  
<br>
🚚 Entregamos directo a tu hogar

</div>




<section class="contenedor">



<div class="producto">

<img src="https://images.unsplash.com/photo-1542838132-92c53300491e">

<div class="info">

<h2>Canasta Fresca</h2>

<p>Verduras variadas para toda la familia.</p>

<p class="precio">$15</p>

<a class="btn" href="#">
Pedir ahora
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1598030343246-eec71cb442a0">

<div class="info">

<h2>Lechuga Fresca</h2>

<p>Cosecha fresca para ensaladas.</p>

<p class="precio">$1</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1592924357228-91a4daadcfea">

<div class="info">

<h2>Tomates Premium</h2>

<p>Seleccionados y llenos de sabor.</p>

<p class="precio">$2.50</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1518977676601-b53f82aba655">

<div class="info">

<h2>Papas Naturales</h2>

<p>Producto directo del campo.</p>

<p class="precio">$2</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1582515073490-39981397c445">

<div class="info">

<h2>Zanahorias</h2>

<p>Frescas y saludables.</p>

<p class="precio">$1.50</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1589927986089-35812388d1f4">

<div class="info">

<h2>Pimientos</h2>

<p>Colores y sabores naturales.</p>

<p class="precio">$2</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1566385101042-1a0aa0c1268c">

<div class="info">

<h2>Brócoli</h2>

<p>Ideal para comidas saludables.</p>

<p class="precio">$1.75</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>




<div class="producto">

<img src="https://images.unsplash.com/photo-1619566636858-adf3ef46400b">

<div class="info">

<h2>Frutas de Temporada</h2>

<p>Selección natural y fresca.</p>

<p class="precio">$12</p>

<a class="btn" href="#">
Comprar
</a>

</div>

</div>



</section>





<section class="canastas">

<h2>🌿 Canastas Semanales</h2>

<p>
Elige tu canasta y recibe productos frescos directamente en tu hogar.
</p>

</section>




<footer>

© 2026 Brajá Market  
<br>
De la tierra a tu hogar 🌱

</footer>



</body>
</html>
