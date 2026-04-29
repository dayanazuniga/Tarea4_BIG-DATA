# Tarea4_BIG-DATA
Codigo mongo db

use amazonVentas
switched to db amazonVentas
db.clientes.find()
{
  _id: ObjectId('69f14ec26c814027b0eac856'),
  nombre: 'Carlos Perez',
  correo: 'carlos@gmail.com',
  ciudad: 'Bogotá'
}
{
  _id: ObjectId('69f14ec26c814027b0eac857'),
  nombre: 'Ana Torres',
  correo: 'ana@gmail.com',
  ciudad: 'Medellín'
}
for(i=1;i<=100;i++){
db.productos.insertOne({
producto:"Producto "+i,
categoria:"Electrónica",
precio:Math.floor(Math.random()*500000)+50000,
stock:Math.floor(Math.random()*100)
})
}
{
  acknowledged: true,
  insertedId: ObjectId('69f151ce9a2cac3dc4a984ff')
}
db.productos.countDocuments()
102
db.productos.find().limit(5)
{
  _id: ObjectId('69f150eaf0c3a705b09fe56b'),
  nombre: 'Laptop Lenovo',
  categoria: 'Tecnología',
  precio: 2800000,
  stock: 50
}
{
  _id: ObjectId('69f150eaf0c3a705b09fe56c'),
  nombre: 'Mouse Gamer',
  categoria: 'Accesorios',
  precio: 90000,
  stock: 70
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849c'),
  producto: 'Producto 1',
  categoria: 'Electrónica',
  precio: 402796,
  stock: 23
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849d'),
  producto: 'Producto 2',
  categoria: 'Electrónica',
  precio: 508515,
  stock: 24
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849e'),
  producto: 'Producto 3',
  categoria: 'Electrónica',
  precio: 270512,
  stock: 9
}
db.productos.insertOne({
nombre:"Teclado",
precio:120000,
stock:30
})
{
  acknowledged: true,
  insertedId: ObjectId('69f1539c9a2cac3dc4a98500')
}
db.productos.find()
{
  _id: ObjectId('69f150eaf0c3a705b09fe56b'),
  nombre: 'Laptop Lenovo',
  categoria: 'Tecnología',
  precio: 2800000,
  stock: 50
}
{
  _id: ObjectId('69f150eaf0c3a705b09fe56c'),
  nombre: 'Mouse Gamer',
  categoria: 'Accesorios',
  precio: 90000,
  stock: 70
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849c'),
  producto: 'Producto 1',
  categoria: 'Electrónica',
  precio: 402796,
  stock: 23
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849d'),
  producto: 'Producto 2',
  categoria: 'Electrónica',
  precio: 508515,
  stock: 24
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849e'),
  producto: 'Producto 3',
  categoria: 'Electrónica',
  precio: 270512,
  stock: 9
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849f'),
  producto: 'Producto 4',
  categoria: 'Electrónica',
  precio: 80090,
  stock: 11
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a0'),
  producto: 'Producto 5',
  categoria: 'Electrónica',
  precio: 301870,
  stock: 90
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a1'),
  producto: 'Producto 6',
  categoria: 'Electrónica',
  precio: 92567,
  stock: 51
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a2'),
  producto: 'Producto 7',
  categoria: 'Electrónica',
  precio: 105832,
  stock: 2
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a3'),
  producto: 'Producto 8',
  categoria: 'Electrónica',
  precio: 477289,
  stock: 43
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a4'),
  producto: 'Producto 9',
  categoria: 'Electrónica',
  precio: 348823,
  stock: 14
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a5'),
  producto: 'Producto 10',
  categoria: 'Electrónica',
  precio: 273259,
  stock: 17
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a6'),
  producto: 'Producto 11',
  categoria: 'Electrónica',
  precio: 65333,
  stock: 26
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a7'),
  producto: 'Producto 12',
  categoria: 'Electrónica',
  precio: 128175,
  stock: 45
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a8'),
  producto: 'Producto 13',
  categoria: 'Electrónica',
  precio: 315737,
  stock: 19
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a9'),
  producto: 'Producto 14',
  categoria: 'Electrónica',
  precio: 549537,
  stock: 3
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984aa'),
  producto: 'Producto 15',
  categoria: 'Electrónica',
  precio: 449090,
  stock: 40
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984ab'),
  producto: 'Producto 16',
  categoria: 'Electrónica',
  precio: 470432,
  stock: 5
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984ac'),
  producto: 'Producto 17',
  categoria: 'Electrónica',
  precio: 176260,
  stock: 77
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984ad'),
  producto: 'Producto 18',
  categoria: 'Electrónica',
  precio: 278206,
  stock: 30
}
Type "it" for more
updateOne(...)
SyntaxError: Unexpected token (1:13)

> 1 | updateOne(...)
    |              ^
db.productos.find(
{precio:{$gt:300000}}
)
{
  _id: ObjectId('69f150eaf0c3a705b09fe56b'),
  nombre: 'Laptop Lenovo',
  categoria: 'Tecnología',
  precio: 2800000,
  stock: 50
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849c'),
  producto: 'Producto 1',
  categoria: 'Electrónica',
  precio: 402796,
  stock: 23
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a9849d'),
  producto: 'Producto 2',
  categoria: 'Electrónica',
  precio: 508515,
  stock: 24
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a0'),
  producto: 'Producto 5',
  categoria: 'Electrónica',
  precio: 301870,
  stock: 90
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a3'),
  producto: 'Producto 8',
  categoria: 'Electrónica',
  precio: 477289,
  stock: 43
}
{
  _id: ObjectId('69f151cd9a2cac3dc4a984a4'),
  producto: 'Producto 9',
  categoria: 'Electrónica',
  precio: 348823,
  stock: 14
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a8'),
  producto: 'Producto 13',
  categoria: 'Electrónica',
  precio: 315737,
  stock: 19
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984a9'),
  producto: 'Producto 14',
  categoria: 'Electrónica',
  precio: 549537,
  stock: 3
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984aa'),
  producto: 'Producto 15',
  categoria: 'Electrónica',
  precio: 449090,
  stock: 40
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984ab'),
  producto: 'Producto 16',
  categoria: 'Electrónica',
  precio: 470432,
  stock: 5
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b0'),
  producto: 'Producto 21',
  categoria: 'Electrónica',
  precio: 402682,
  stock: 38
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b1'),
  producto: 'Producto 22',
  categoria: 'Electrónica',
  precio: 366112,
  stock: 14
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b3'),
  producto: 'Producto 24',
  categoria: 'Electrónica',
  precio: 345850,
  stock: 47
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b4'),
  producto: 'Producto 25',
  categoria: 'Electrónica',
  precio: 394912,
  stock: 4
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b5'),
  producto: 'Producto 26',
  categoria: 'Electrónica',
  precio: 521016,
  stock: 20
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b6'),
  producto: 'Producto 27',
  categoria: 'Electrónica',
  precio: 393450,
  stock: 38
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b7'),
  producto: 'Producto 28',
  categoria: 'Electrónica',
  precio: 514248,
  stock: 80
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984b9'),
  producto: 'Producto 30',
  categoria: 'Electrónica',
  precio: 415275,
  stock: 86
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984ba'),
  producto: 'Producto 31',
  categoria: 'Electrónica',
  precio: 342332,
  stock: 63
}
{
  _id: ObjectId('69f151ce9a2cac3dc4a984bb'),
  producto: 'Producto 32',
  categoria: 'Electrónica',
  precio: 303658,
  stock: 41
}
Type "it" for more
db.productos.updateOne(
{nombre:"Teclado"},
{$set:{precio:100000}}
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
db.productos.find(
{nombre:"Teclado"}
)
{
  _id: ObjectId('69f1539c9a2cac3dc4a98500'),
  nombre: 'Teclado',
  precio: 100000,
  stock: 30
}
db.productos.deleteOne(
{nombre:"Teclado"}
)
{
  acknowledged: true,
  deletedCount: 1
}
db.pedidos.insertOne({
cliente:"Carlos Perez",
productos:[
{
nombre:"Laptop Lenovo",
cantidad:2,
precio:2800000
}
],
total:5600000
})
{
  acknowledged: true,
  insertedId: ObjectId('69f157229a2cac3dc4a98501')
}
db.productos.countDocuments()
102
db.pedidos.aggregate([
{
$group:{
_id:null,
totalVentas:{$sum:"$total"}
}
}
])
{
  _id: null,
  totalVentas: 5600000
}
db.productos.aggregate([
{
$group:{
_id:null,
promedio:{$avg:"$precio"}
}
}
])
{
  _id: null,
  promedio: 343124.85294117645
}
db.pedidos.aggregate([
{
$lookup:{
from:"clientes",
localField:"cliente",
foreignField:"nombre",
as:"datosCliente"
}
}
])
{
  _id: ObjectId('69f157229a2cac3dc4a98501'),
  cliente: 'Carlos Perez',
  productos: [
    {
      nombre: 'Laptop Lenovo',
      cantidad: 2,
      precio: 2800000
    }
  ],
  total: 5600000,
  datosCliente: [
    {
      _id: ObjectId('69f14ec26c814027b0eac856'),
      nombre: 'Carlos Perez',
      correo: 'carlos@gmail.com',
      ciudad: 'Bogotá'
    }
  ]
}
countDocuments()
ReferenceError: countDocuments is not defined
db.pedidos.aggregate([
{
$lookup:{
from:"clientes",
localField:"cliente_id",
foreignField:"_id",
as:"cliente"
}
}
])
{
  _id: ObjectId('69f157229a2cac3dc4a98501'),
  cliente: [],
  productos: [
    {
      nombre: 'Laptop Lenovo',
      cantidad: 2,
      precio: 2800000
    }
  ],
  total: 5600000
}
db.pedidos.aggregate([
{
$lookup:{
from:"clientes",
localField:"cliente",
foreignField:"nombre",
as:"datosCliente"
}
}
])
{
  _id: ObjectId('69f157229a2cac3dc4a98501'),
  cliente: 'Carlos Perez',
  productos: [
    {
      nombre: 'Laptop Lenovo',
      cantidad: 2,
      precio: 2800000
    }
  ],
  total: 5600000,
  datosCliente: [
    {
      _id: ObjectId('69f14ec26c814027b0eac856'),
      nombre: 'Carlos Perez',
      correo: 'carlos@gmail.com',
      ciudad: 'Bogotá'
    }
  ]
}
amazonVentas


