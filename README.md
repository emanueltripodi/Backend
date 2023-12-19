//intentar los desafios realizados por el profe en clase
let productos = [{
    nombre: "airforce",
    precio: 180000,
    stock: 23
},{
    nombre: "puma",
    precio: 40000,
    stock: 5
},{
    nombre: "jordan",
    precio: 300000,
    stock: 12
}]

let stockPositivo = [];

for (let producto of productos){
    if (producto.stock > 7){
        stockPositivo.push(producto);
    }
    
}
let funcionFilter = stockPositivo.filter((producto) => producto.stock > 7)
console.log(funcionFilter);

//console.log(stockPositivo);

let socios = [{
    club: "boca juniors",
    socios: 150000,
    capacidad: 60000
},{
    club: "river plate",
    socios: 120000,
    capacidad: 90000
},{
    club: "racing",
    socios: 30000,
    capacidad: 30000
}]

let clubsGrandes = [];
for (let socio of socios){
    if(socio.capacidad > 50000){
        clubsGrandes.push(socio)
    }
}
let filterSocios = socios.filter(socios => socio.capacidad > 50000)
console.log(filterSocios);
//console.log(clubsGrandes);

let antiguedad = [{
    empleado: "camilo",
    añosEmpresa: 3,
    sueldo: 60000
},{
    empleado: "sofia",
    añosEmpresa: 6,
    sueldo: 120000
},{
    empleado: "ema",
    añosEmpresa: 7,
    sueldo: 160000
}]

let masViejo = [];
for (let antiguo of antiguedad){
    if(antiguo.añosEmpresa > 5){
        masViejo.push(antiguo)
    }
}

let filterAntiguedad= antiguedad.filter(antiguedad => antiguo.añosEmpresa > 5)
console.log(filterAntiguedad);

//console.log(masViejo);


//desafio
id = 0
class ProductManager{
    #producto = [];

    getProductos(){
        return this.producto;
    }

    agregarProduct = (title, description, price, thumbnail, code, stock) =>{
    let produ = {
        title: title,
        description: description,
        price: price,
        thumbnail: thumbnail,
        code: Math.random(),
        stock: stock,
        id: this.id
    }
    this.id = this.id +1;
    this.#producto.push(produ);
    }}
    let getProductosbyId = producto.filter(produ => produ == this.id)
    if(getProductosbyId = null){
        console.log("Not found");} else{
            console.log(getProductosbyId);
        }
    
    
    /*products = [{
    title: "zapatilla",
    description: "borcego negro de cuero",
    price: 12000,
    thumbnail: "",
    code: 1,
    stock: 300},{
    title: "remera",
    description: "remera oversize negra",
    price: 6000,
    thumbnail: "https://d22fxaf9t8d39k.cloudfront.net/2bbdb1d316ff4cfcf81b54737d58eb85ef5f1c49d44ba7f4830578a61512a2d458726.jpg",
    code: 2,
    stock: 150},{
    title: "pantalon",
    description: "pantalon cargo verde",
    price: 17000,
    thumbnail: "",
    code: 3,
    stock: 100},{
    title: "camisa",
    description: "camisa lino blanca",
    price: 10000,
    thumbnail: "https://acdn.mitiendanube.com/stores/001/676/826/products/img-54561-f536e29b010a397fe416818493608584-1024-1024.jpg",
    code: 4,
    stock: 30

    }]*/
