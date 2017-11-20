# dat_Abs_listM Tema 3 Programacion en entorno cliente  
## Datos Abstractos: Lista Con Metodos de Arrays  

### Version 1.0.0  
Renombrado de archivos:  
* t3_datAbs_list.html -> t3dat_Abs_listM.html  
* t3_datAbs_list.js -> t3dat_Abs_listM.js  
* t3_html_controls.js -> sin cambios  
* jscss.css -> sin cambios  
Detalles de la version 1.0.0:  
Ruta del script enlazado al html cambiado  
Modificacion de algunas de las funciones en *t3dat_Abs_listM.js*
1. Funciones añadir elementos  
2. Funciones Remover elementos  
3. Funciones de Añadir elementos en una posicion  
4. Funciones de remover elemento en una posicion  
Nueva Funcion place(list):  
Esta funcion reposiciona todos los elementos para evitar poner un NaN en mitad de la lista  
```[javascript]  
function place(array)  
/*Funcion que situa todos los elementos NaN al final de la lista*/  
{  
  var i = 0;  
  while(i < listLength){  
    if(isNaN(array[i]) && !isNaN(array[i+1])){  
      var aux = array[i];  
      array[i] = array[i+1];  
      array[i+1] = aux;  
    }  
      i++;  
  }  
}  
```
### Version 0.0.0  
Inicio del ejercicio datos abstractos: lista con metodos de arrays  
Detalles de la version 0.0.0:  
Reutilizacion del codigo usado en: *Datos Abstractos: Lista*  

