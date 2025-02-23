<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menú Interactivo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f8f8;
        }
        .menu {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 50px;
        }
        .menu button {
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            background-color: #ff9800;
            color: white;
            transition: 0.3s;
        }
        .menu button:hover {
            background-color: #e68900;
        }
        .contenido {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            width: 80%;
            margin-left: auto;
            margin-right: auto;
        }
        .productos {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin-top: 10px;
        }
        .producto {
            background: #fff3e0;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.1);
            width: 200px;
            text-align: center;
        }
        .producto img {
            width: 100px;
            height: auto;
            margin-top: 5px;
        }
    </style>
</head>
<body>
    <h1>Menú Interactivo</h1>
    <div class="menu">
        <button onclick="mostrarSeccion('helado')">Helado</button>
        <button onclick="mostrarSeccion('paletas')">Paletas de Hielo</button>
        <button onclick="mostrarSeccion('nieves')">Nieves</button>
        <button onclick="mostrarSeccion('papas')">Papas</button>
        <button onclick="mostrarSeccion('botanas')">Botanas</button>
    </div>
    
    <div id="contenido" class="contenido">
        <h2 id="titulo"></h2>
        <p id="descripcion"></p>
        <div id="productos" class="productos"></div>
    </div>
    
    <script>
        function mostrarSeccion(seccion) {
            const contenido = document.getElementById('contenido');
            const titulo = document.getElementById('titulo');
            const descripcion = document.getElementById('descripcion');
            const productosDiv = document.getElementById('productos');
            
            const data = {
                helado: { descripcion: "Deliciosos helados de diferentes sabores y presentaciones.", productos: [] },
                paletas: { descripcion: "Refrescantes paletas de hielo en una gran variedad de sabores.", productos: [] },
                nieves: { 
                    descripcion: "Tradicionales nieves con ingredientes naturales.", productos: [
                         { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                         { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                         { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                         { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                    ] },
                papas: { 
                    descripcion: "Crujientes papas fritas con diferentes salsas y condimentos.", 
                    productos: [
                        { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                        { nombre: "Ruffles Queso", imagen: "https://cdn.shopify.com/s/files/1/0566/4391/1854/files/7501011167674_270923_48adaeea-cb0c-46ca-8496-92f9bd0e8289.webp?v=1696001745" },
                        { nombre: "Doritos Nacho", imagen: "https://m.media-amazon.com/images/I/71HnPB90QjL.jpg" },
                        { nombre: "Rancheritos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101116775L1.jpg" },
                        { nombre: "Fritos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101113112L.jpg?odnHeight=612&odnWidth=612&odnBg=FFFFFF" },
                        { nombre: " Cheetos flamin hot", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101113093L.jpg" },
                        { nombre: "Chetos", imagen: "https://http2.mlstatic.com/D_NQ_NP_988195-MLU77022706039_062024-O.webp"},
                        { nombre: "Churrumais", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750047800255L.jpg" },
                        { nombre: "Chips", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750301854470L1.jpg?odnHeight=612&odnWidth=612&odnBg=FFFFFF" },
                        { nombre: "Tostitos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750047803740L.jpg" },
                    ]
                },
                botanas: { 
                    descripcion: "Variedad de botanas para disfrutar en cualquier ocasión.", 
                    productos: [
                    { nombre: "Sabritas Clásicas", imagen: "https://lagranbodega.vteximg.com.br/arquivos/ids/297205-1000-1000/7501011167438.jpg?v=638418217795430000" },
                        { nombre: "Ruffles Queso", imagen: "https://cdn.shopify.com/s/files/1/0566/4391/1854/files/7501011167674_270923_48adaeea-cb0c-46ca-8496-92f9bd0e8289.webp?v=1696001745" },
                        { nombre: "Doritos Nacho", imagen: "https://m.media-amazon.com/images/I/71HnPB90QjL.jpg" },
                        { nombre: "Rancheritos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101116775L1.jpg" },
                        { nombre: "Fritos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101113112L.jpg?odnHeight=612&odnWidth=612&odnBg=FFFFFF" },
                        { nombre: " Cheetos flamin hot", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750101113093L.jpg" },
                        { nombre: "Chetos", imagen: "https://http2.mlstatic.com/D_NQ_NP_988195-MLU77022706039_062024-O.webp"},
                        { nombre: "Churrumais", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750047800255L.jpg" },
                        { nombre: "Chips", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750301854470L1.jpg?odnHeight=612&odnWidth=612&odnBg=FFFFFF" },
                        { nombre: "Tostitos", imagen: "https://i5.walmartimages.com.mx/gr/images/product-images/img_large/00750047803740L.jpg" },
                    ] }
            };
            
            titulo.innerText = seccion.charAt(0).toUpperCase() + seccion.slice(1);
            descripcion.innerText = data[seccion].descripcion;
            
            productosDiv.innerHTML = "";
            data[seccion].productos.forEach(producto => {
                const div = document.createElement('div');
                div.classList.add('producto');
                div.innerHTML = `<strong>${producto.nombre}</strong><br><img src="${producto.imagen}" alt="${producto.nombre}">`;
                productosDiv.appendChild(div);
            });
            
            contenido.style.display = 'block';
        }
    </script>
</body>
</html>
