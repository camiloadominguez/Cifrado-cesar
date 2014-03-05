Cifrado-cesar
=============
<<!doctype html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Cifrado cesar</title>
    <script type="text/javascript">
    function convert()
    {   
        var j;
        var n;
        var l;
        var r="";
        var a=document.getElementById('t1').value;
    //  alert(a);
        var b=a.length;
    //  alert(b);
        var c=a.charCodeAt(0);
    //  alert(c);
        var d=String.fromCharCode(c+10);
    //  alert(d);
        document.getElementById('t2').value=d;
        var z=document.getElementById('t2').value;
        b=z.length;
  //    alert(b);
        c=z.charCodeAt(0);

    //  alert(c);

    for(i=0;i<a.length;i++)
    { 
        
        
  //    alert("entro");

        j=a.charAt(i);
   //   alert(j);
        oument.getElementById('t2').value=j;
       
       l=a.charCodeAt(i);
 //    alert(l);
       n=String.fromCharCode(l+10);
    // alert("si"+n+"nada");
       if(a.charCodeAt(i)==32)
       {
        n=" ";
       r=r+n;
       }
       
       r=r+n;

      
      
      
     }
     document.getElementById('t2').value=r;

    }
    </script>
</head>
<body>
    <button onclick=convert()>Convertir</button>
    <br></br>

    <input type="text" id="t1"placeholder="ingrese nombre">
    <br></br>

    <input type="text" id="t2" placeholder="nombre convertido">

    <br></br>
    

</body>
</html>
