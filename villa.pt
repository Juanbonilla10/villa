var villa=document.getElementById("villa_platzi");
var papel=villa.getContext("2d");
document.addEventListener("keydown",der);
var xi=10;
var yi=10;
var x=aleatorio(0,480);
var y=aleatorio(0,480);
var movimiento=10;
var teclas=
{
  UP:38,
  DOWN:40,
  LEFT:37,
  RIGHT:39
}

var fondo=
{
  url:"imagenes/tile.png",
  cargaOK:false
}
var vaca=
{
  url:"imagenes/vaca.png",
  cargaOK:false
}
var cerdo=
{
  url:"imagenes/cerdo.png",
  cargaOK:false
}

fondo.imagen=new Image();
fondo.imagen.src=fondo.url;
fondo.imagen.addEventListener("load", cargarfondo);

vaca.imagen=new Image();
vaca.imagen.src=vaca.url;
vaca.imagen.addEventListener("load",cargarvaca);

cerdo.imagen=new Image();
cerdo.imagen.src=cerdo.url;
cerdo.imagen.addEventListener("load",cargarcerdo);


function cargarfondo()
{
  fondo.cargaOK=true;
  dibujar();
}
function cargarvaca()
{
  vaca.cargaOK=true;
  dibujar();
}
function cargarcerdo()
{
  cerdo.cargaOK=true;
  dibujar();
}
function dibujar()
{

  if (fondo.cargaOK)
  {
    papel.drawImage(fondo.imagen,0,0);
  }
  if (vaca.cargaOK)
  {
    for(l=0; l<2; l++)
    {
    x= aleatorio(0,420);
    y= aleatorio(0,420);
    papel.drawImage(vaca.imagen,x,y);
    }

    /*function aleatorio(max,min)
    {
      var resultado;
      resultado =Math.floor(Math.random()*(max-min+1))+min
      return resultado;
    }*/
    if (cerdo.cargaOK)
    {
      papel.drawImage(cerdo.imagen,xi,yi);
    }
  }
}
function aleatorio(max,min)
{
  var resultado;
  resultado =Math.floor(Math.random()*(max-min+1))+min
  return resultado;
}
function der(evento)
{
  switch (evento.keyCode)
  {
    case teclas.RIGHT:
      dibujar();
      xi=xi+movimiento;
    break;
    case teclas.DOWN:
      dibujar();
      yi=yi+movimiento;
    break;
    case teclas.LEFT:
      dibujar();
      xi=xi-movimiento;
    break;
    case teclas.UP:
      dibujar();
      yi=yi-movimiento;
    break;
    default:
    break;
  }
}
function mantenerposicion()
{
  if (vaca.cargaOK)
  {
    for(l=0; l<2; l++)
    {
      var man=x;
      var pos=y;

    }
  }
}
