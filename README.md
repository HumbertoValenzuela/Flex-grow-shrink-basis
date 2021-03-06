# Flex-grow-shrink-basis
flex-grow: 1; flex-shrink: 0 ; flex-basis: 50%; ShortHand es flex: 1 0 50%;

* Flex-grow: establece que hacer cuando hay espacio sobrante. 
* La propiedad flex-grow se utiliza en los hijos del padre. 
* Grow llena el espacio del elemento, por ejemplo al mover la resolución del DOM este se ajusta 
* Grow Con esto el ancho variará de acuerdo a lo que tenga de width border padding 
* Flex-shrink:1 2 o 3; Al mover la resolución el valor más grande obtendrá un ancho menor
* Flex-basis: Es una base de ancho mínimo. flex-basis: 50%; al elemento 2. Tendrá como mínimo 50%
* flex-basis es mejor agregar flex-grow:1; a todos dará un mejor resultado
* El shorthands es flex: toma 3 parametros: 1) flex-grow 2) flex-shrink 3) flex-basis

```javascript
/* -------------------------------------------------------------------------------------------- */
.elemento-flex {
    padding: 10px;
    background-color: #E53935;
    /* Crecer con Flex**/     
}

.elemento-flex:nth-child(2) {
    background-color: #8E24AA;
}

.elemento-flex:nth-child(3) {
    background-color: #3F51B5;
}
/* -------------------------------------------------------------------------------------------- */
.elemento-flex-grow {
    padding: 10px;
    background-color: #E53935;
    /* Crecer con Flex**/ 
    flex-grow: 1;
}

.elemento-flex-grow:nth-child(2) {
    background-color: #8E24AA;
}

.elemento-flex-grow:nth-child(3) {
    background-color: #3F51B5;
}
/* -------------------------------------------------------------------------------------------- */
.elemento-flex-growvalores {
    padding: 10px;
    background-color: #E53935;
    /* Crecer con Flex**/ 
    flex-grow: 1;
}

.elemento-flex-growvalores:nth-child(2) {
    background-color: #8E24AA;
    flex-grow: 3;
}

.elemento-flex-growvalores:nth-child(3) {
    background-color: #3F51B5;
}
/* -------------------------------------------------------------------------------------------- */
/* -------------------------------------------------------------------------------------------- */
.elemento-flex-shrink {
    padding: 10px;
    background-color: #E53935;
    width: 500px;
}
.elemento-flex-shrink:nth-child(1) {
    flex-shrink: 1;
}
.elemento-flex-shrink:nth-child(2) {
    background-color: #8E24AA;   
    flex-shrink: 2;    
}

.elemento-flex-shrink:nth-child(3) {
    background-color: #3F51B5;
    flex-shrink: 3;
}
/* -------------------------------------------------------------------------------------------- */
/* -------------------------------------------------------------------------------------------- */
.elemento-flex-basis {
    padding: 10px;
    background-color: #E53935;   
    
}

.elemento-flex-basis:nth-child(2) {
    background-color: #8E24AA;   
       flex-basis: 50%;
}

.elemento-flex-basis:nth-child(3) {
    background-color: #3F51B5;
}
/* -------------------------------------------------------------------------------------------- */
/* -------------------------------------------------------------------------------------------- */
.elemento-flex-sharhands {
    padding: 10px;
    background-color: #E53935;  
    flex: 1 0 auto; 
    
}

.elemento-flex-sharhands:nth-child(2) {
    background-color: #8E24AA;  
      
}

.elemento-flex-sharhands:nth-child(3) {
    background-color: #3F51B5;
    /* flex: toma 3 parametros: 1) flex-grow 2) flex-shrink 3) flex-basis  */
    
}
```
