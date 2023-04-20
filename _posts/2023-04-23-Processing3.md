---
title: 3.3 Processing 3
published: true
---

## Introducción

La tercera practica consiste en hacer q nuestra figura rebote por la pantalla, se explica en la presentación:

* [Presentación-explicación](https://docs.google.com/presentation/d/1OAGRaGFBAh9BUQRVBT5XnlYus1DpU_KUkRQZ7PC0Qfo/edit?usp=drive_web&authuser=1)

## Instrucciones

A partir de la figura de la practica anterior debemos hacer un efecto de movimiento de esta donde la figura rebote en los bordes de la pantalla y un texto con nuestro nombre que se amplie y se reduzca.

## Resultado

```java

PShape iron;
int jgg = -400; //Variable de movimiento de Ironman
int jgg1 = 1; // Modifica el rebote de ironman
int jgg2 = 30; //Tamaño texto
int jgg3 = 1; // Modifica el movimiento del texto

void setup() {

  size(500, 500);
  iron = loadShape("iron_man_icon.svg");
  background(255);
  noStroke();
}

void draw() {

    fill(255);
    square(0,0, width);
    fill(255,0, 0);
    ellipse(250+jgg, 430, 40,40);
    triangle(200+jgg, 390, 250+jgg, 430, 200+jgg, 450);
    triangle(300+jgg, 390, 250+jgg, 430, 300+jgg, 450);
    shape(iron, 150+jgg, 100);
    
    jgg = jgg + jgg1;
    if (jgg == 150) {
      
      jgg1 = -1;
    }
  
  if (jgg == -150){
  
    jgg1 = 1;
  }
  
  textSize(jgg2);
  text("Jaime García", 170-jgg2, 50);
  jgg2 = jgg2 +jgg3;
  if (jgg2 == 50){
  
    jgg3 = -1;
  }
  
  if (jgg2 == 30){
  
    jgg3 = 1;
  }
}

```

## Area de Descargas

|  Descripción   |     Codigo    |
|:---------------|:------------------|
| Entrega|[Enlace a la carpeta con la imagen y el codigo](https://drive.google.com/file/d/1RIcr2Dgu2ZVFYwAHZyFZ14OfGQJLqbJI/view) |
