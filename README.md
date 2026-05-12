# TIPS-E1N1K0:

## ABSTRACT = RESUMEN:

Some tips.<br>
Algunos tips.


## INDEX = INDICE:

### CMD:
  - CREA UNA LISTA.txt DESDE UNA LISTA DIR:
    dir /b > lista. txt
    Partes del comando:
    dir: es el comando para listar el contenido de un directorio.
    /b: indica que queremos obtener una lista simplificada, solo con los nombres de archivo, sin información adicional.
    >: sirve para redireccionar la salida del comando a un archivo en lugar de mostrarla en pantalla.
    lista.txt: es el nombre del archivo de texto donde se guardará la lista. Si no existe, se creará. Si existe, su contenido será sobreescrito.


### COMENTARIOS:
PYTHON: # o """ y cierra con """<br>
REACT: /* y cierra con */


### VSC:
Guardar: Ctrl + s<br>
Seleccionar todo: Ctrl + A <br>
Dejar seleccion en comentarios :mantener apretado Ctrl + k + c<br>
Quitar seleccion en comentarios :mantener apretado Ctrl + k + u<br>
ctrl + f5 to run your Python code without debugging<br>


### WORD:
  - QUITAR ESPACIOS EN BLANCO DUPLICADOS:<br>
     Seleccionar texto => Reemplazar => Buscar: ( ){2,} => Reemplazar: \1 => Usar caracteres comodin.
    
  - ELIMINAR ESPACIOS EN BLANCO AL INICIO:<br>
    Seleccionar texto => Reemplazar => Buscar: ^\s+ => Reemplazar:  => Usar caracteres comodin.
  
  - ELIMINAR ESPACIOS EN BLANCO AL FINAL:<br>
    Seleccionar texto => Reemplazar => Buscar: \s+$ => Reemplazar:  => Usar caracteres comodin.
  
  - CAMBIAR FORMATO DE FECHA:
    Seleccionar texto => Reemplazar => Buscar: (\d{2})/(\d{2})/(\d{4}) => Reemplazar: \2/\1/\3 => Usar caracteres comodin.<br>
    Reordena una fecha en formato DD/MM/YYYY a MM/DD/YYYY. (\d{2}) captura el día, (\d{2}) captura el mes y (\d{4}) captura el año. \2, \1 y \3 representan los grupos capturados en ese orden.
    
  - RESALTAR TEXTO:
  - Seleccionar texto => Reemplazar => Buscar: palabra => Reemplazar: <span style="background-color: yellow;">palabra</span> => Usar caracteres comodin.  
    
    
  - CODIGO:
  - "^" denota el inicio de un párrafo.<br>
  - "\s+" representa uno o más espacios en blanco.<br>
  - "$" denota el final de un párrafo.<br>

### POWER BI:
(Pagina as number) as table =><br>
let
    Origen = Web.Page(Web.Contents("https://www.unglobalcompact.org/what-is-gc/participants/search?page="& Number.ToText(Pagina))),
    Data0 = Origen{0}[Data]
in
    Data0

Generar tabla 
{1..349}
Cambiar nombre de columna generada a pagina

Nueva columna
TraeTabla([pagina])

Expandir

CALCULAR EL TOTAL IGNORANDO FILTROS ((Usando DAX):<br>
Total Tabla = CALCULATE(SUM(Carpeta[Tabla]), ALL(Carpeta))<br>

MEDIDA DE PORCENTAJE TOTAL CON FORMATO % (Usando DAX):<br>
% Tabla =  
FORMAT( 
    DIVIDE( 
        SUM(Skyscrapers[Tabla]),  
        CALCULATE(SUM(Skyscrapers[Tabla]), ALL(Carpeta)) 
    ),  
    "0.00%" 
)
     
## Where users can get help with your project = Donde los usuarios pueden encontrar ayuda con el proyecto:
   Pueden escribirme a e1n1k0programa@gmail.com<br><br>
	 You can contact me at e1n1k0programa@gmail.com
  


