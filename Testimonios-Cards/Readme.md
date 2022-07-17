# Testimonios Cards

Esta pagina es mi primera practica de FrontEndMentor

pagina del reto: [https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7/hub/testimonials-grid-section-JJd3KTQxt1](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7/hub/testimonials-grid-section-JJd3KTQxt1)

**Tecnologías Usadas en esta practica:**
<img src="Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled.png" alt="html5" width="75"/>

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%201.png)

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%202.png)

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%203.png)

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%204.png)

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%205.png)

1. Distribución

La primero que hice fue la estructura HTML y en el main, usando el grid de bootstrap dividí la pantalla en dos secciones que se dividieron mas adelante

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%206.png)

de forma que lo que tiene relleno son divs y lo relleno de blanco son las tarjetas dentro del div

Ya se habrán dado cuenta que si lo haces de esta manera como indica queda todo unido, así que le di un paddig (p-2 en bootstrap) para que quedaran con sus espacios correspondientes

2.Responsive Design

como lo mencione en la parte anterior dividi las secciones con ayuda del grid de bootstrap, quedando de esta manera

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%207.png)

Esto es para los dispositivos de pantallas mas grandes que lg (960px)

Para los dispositivos de pantallas mas pequeños lo deje en 12 haciendo que se presentara solo una tarjeta a la vez

1. Contenido de las tarjetas

El diseño buscado en las tarjetas se ve asi

 

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%208.png)

como ya tenia los divs hechos con ayuda de la clase card-body de bootstrap fue mas sencillo hacerlo y teniendo la configuración de grid se mas fácil

son dos divs, la parte superior y la parte inferior, la parte superior consta de imagen nombre y verificación 

1. inserte una imagen <img>, después el nombre en un párrafo y en otro las palabras de verificación
2. En el segundo div puse en un párrafo la frase a destacar y en otro párrafo la review completa

***con esto la parte de la estructura quedo completa***

1. Correcciones de diseño

las correcciones de diseño las hice por partes: redefinir colores, ajustar tamaño de la imagen, cambiar fuente tipográfica y estilos de fuente

1. Colores
    
    en el archivo cusom.scss redefiní las variables de bootstrap para cambiar los colores a mi gusto
    
    cuando escogí colores oscuros el color del texto lo cambie a blanco para que se pueda leer
    
2. Ajustar imagen
    
    la imagen se veía un poco grande asi que la ajuste a 50 px, probablemente exista una mejor mañera de hacerlo pero no la conozco en este momento y no tiene repercusiones en el tamaño normal o pantallas pequeñas 
    
3. Fuente tipografica
    
    usando google fonts importe la fuente tipografica “Barlow Semi Condensed”, la enlace al html y al ccs y quedo lista
    

d. estilos de fuente

en el archivo custom.sass cree 4 clases para los estilos del texto: titulos, verificacion,frase, y review

- Titulo: se di un peso de 500 a la fuente
- verificación: le di una opacidad de 50% (0.5 para que sea compatible en navegadores)
- frase: le di un peso de 600 a la fuente
- review: la opacidad la configure a 70% (0.7)

Al final reemplace la variable del color de fondo para que se pudieran ver de mejor manera los bordes de las tarjetas, a lo mejor no lo veo bien por mi pantalla

1. Optimización de código

Después de usar sass se tiene que compilar y como estamos usando bootstrap el archivo generado supera las 4,000 líneas, pero contiene un montón de cosas de bootstrap que no estamos utilizando entonces con ayuda de “Purge CSS”

link de purgecss: [https://purgecss.com/](https://purgecss.com/)

en el archivo package.json configuramos un scrip para usar purgecss

```json
"build": "purgecss --css ./sass/custom.css --content index.html -o ./css/styles.css"
```

lo ejecutamos y tendremos un archivo reducido y optimizado de css de solo las cosas que ocupamos

cambiamos el link de css de bootsrap-sass a el reducido y listo

 Al final quedo de esta menra  y quede contento con el resultado

***versión web***

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%209.png)

***versión móvil*** 

![Untitled](Testimonios%20Cards%20574607057c624d5e9b538e4e5603d9cc/Untitled%2010.png)
