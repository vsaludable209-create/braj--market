# brajá-market
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Brajá Market 🥬</title>

<style>
body{
font-family: Arial;
margin:0;
background:#f4f4f4;
}

header{
background:#2E7D32;
color:white;
text-align:center;
padding:20px;
}

.search{
text-align:center;
padding:10px;
}

input{
padding:10px;
width:80%;
max-width:400px;
border-radius:8px;
border:1px solid #ccc;
}

.container{
display:flex;
flex-wrap:wrap;
justify-content:center;
padding:10px;
}

.card{
background:white;
margin:10px;
width:200px;
padding:10px;
border-radius:10px;
box-shadow:0 2px 5px rgba(0,0,0,0.2);
}

.price{
color:#2E7D32;
font-weight:bold;
}

button{
background:#2E7D32;
color:white;
border:none;
padding:8px;
width:100%;
border-radius:5px;
margin-top:5px;
cursor:pointer;
}

.cart{
position:fixed;
bottom:10px;
right:10px;
background:#25D366;
color:white;
padding:15px;
border-radius:50px;
cursor:pointer;
font-weight:bold;
}

</style>
</head>

<body>

<header>
<h1>🥬 Brajá Market</h1>
<p>Catálogo online - Haz tu pedido fácil</p>
</header>

<div class="search">
<input type="text" id="buscar" onkeyup="filtrar()" placeholder="Buscar productos...">
</div>

<div class="container" id="productos">

</div>

<div class="cart" onclick="enviarWhatsApp()">
🛒 Ver pedido
</div>

<script>

const numeroWhatsApp = "593XXXXXXXXX"; // CAMBIA ESTO

let carrito = [];

const productos = [
{name:"Tomate", precio:1.20},
{name:"Lechuga", precio:0.80},
{name:"Banano", precio:1.00},
{name:"Manzana", precio:1.50},
{name:"Papa", precio:0.60},
{name:"Cebolla", precio:0.90}
];

function mostrar(){
let cont = document.getElementById("productos");
cont.innerHTML = "";

productos.forEach((p,i)=>{
cont.innerHTML += `
<div class="card">
<h3>${p.name}</h3>
<p class="price">$${p.precio.toFixed(2)}</p>
<button onclick="agregar(${i})">Agregar</button>
</div>
`;
});
}

function agregar(i){
carrito.push(productos[i]);
alert(productos[i].name + " agregado al pedido");
}

function enviarWhatsApp(){
if(carrito.length === 0){
alert("Tu carrito está vacío");
return;
}

let mensaje = "Hola, quiero hacer este pedido:%0A";

let total = 0;

carrito.forEach(p=>{
mensaje += "- " + p.name + " ($" + p.precio + ")%0A";
total += p.precio;
});

mensaje += "%0ATotal: $" + total.toFixed(2);

let url = "https://wa.me/" + numeroWhatsApp + "?text=" + mensaje;

window.open(url, "_blank");
}

function filtrar(){
let input = document.getElementById("buscar").value.toLowerCase();
let cards = document.getElementsByClassName("card");

for(let c of cards){
let text = c.innerText.toLowerCase();
c.style.display = text.includes(input) ? "block" : "none";
}
}

mostrar();

</script>

</body>
</html>
