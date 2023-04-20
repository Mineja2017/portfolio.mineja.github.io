---
title: 3.4 Processing 4
published: true
---

## Introducción

Llegamos al final de la evaluación y con ella a la práctica final explicada en la siguiente presentación y vídeo:

* [Presentación-explicación](https://docs.google.com/presentation/d/1xKL_UFUU_lNY-T53PhrVUZRdCWc5RZuFQYQDxW8yHLo/edit?usp=drive_web&authuser=1  )

* [Video](https://drive.google.com/file/d/1mZUnjNQjsRyqkEr69w9Bgr6jpj6ebaN9/view)

## Instrucciones

Se debe replicar el movimiento de la pelota como se muestra en el video, además se debe procurar que no haya mas de un *"for"* para la creación de la cudricula y de que el programa siga funcionando si se cambian las medidad de la cuadrícula.

## Resultado

```java

int jgg; //contador para el grid
float jgg1 = 0; //Coordenada x
float jgg2 = 0; //Coordenada y
float jgg3; //Varibale que modifica la x
float jgg4; //Variable que modfica la y

void setup() {

  size(500, 500);
  background(255);
}


void grid() { //funcion de las celdas

  for(jgg=0;jgg<=width;jgg=jgg+width/5){
    
    fill(0);
    line(0,jgg,width,jgg);
    line(jgg,0,jgg,height);
  }
}

void ellispemove1() { //Movimiento 1 de la elipse (Esquina-Esquina)

    fill(255);
    square(0,0, width);
    fill(255,0, 0);
    ellipse(0+jgg1,0+jgg2,20,20);
    jgg1 = jgg1+jgg3;
    jgg2 = jgg2+jgg4;
    
    if (jgg1 == width && jgg2==height) { //Segundo movimiento
      
      jgg3 = 0;
      jgg4 = -2;
    }
  
  if (jgg1 == width && jgg2== (3*height/5)){ //Tercer movimiento
  
    jgg4 = -1;
    jgg3 = -2;
  }
  
  if (jgg1 == (3*width/5) && jgg2== (2*height/5)){ //Cuarto movimiento
  
    jgg4 = 0;
    jgg3 = -2;
  }
  
  if (jgg1 == 0 && jgg2== (2*height/5)){ //Quinto movimiento
  
    jgg4 = -2;
    jgg3 = 0;
  }
  
  if (jgg1 == 0 && jgg2==0){ //Primer movimiento
  
    jgg4 = 2;
    jgg3 = 2;
  }
}

void draw() {

  ellispemove1();
  grid();

}

```

## Area de Descargas

|  Descripción   |     Codigo    |
|:---------------|:------------------|
| Entrega|[Enlace a la carpeta con la imagen y el codigo](https://drive.google.com/file/d/16dLwBocHMR7gz0ceaWJmSM8UHJ59UR4l/view) |
