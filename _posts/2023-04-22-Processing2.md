---
title: 3.2 Processing 2
published: true
---

## Introducción

Continuamos con la segunda práctica del trimestre y con el video de muestra de los que debemos hacer:

* [Video de ejemplo](https://drive.google.com/file/d/1Dwl8yT34ZdeNwM2fKsGM7RKoerZpLn4Y/view)
* [Presentación-explicación](https://docs.google.com/presentation/d/1ujVJv77c0yl8c3EG2Z8Z4Jzfh2VNHiQ1XuCzLsl3d2o/edit?usp=drive_web&authuser=1)

## Instrucciones

A partir de la figura de la practica anterior debemos hacer un efecto de movimiento de esta donde esta entre y salga de la panatalla.

## Resultado

```java

PShape iron;
int jgg = -400;

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
    jgg ++;
  
}

```

## Area de Descargas

|  Descripción   |     Codigo    |
|:---------------|:------------------|
| Entrega|[Enlace a la carpeta con la imagen y el codigo](https://drive.google.com/file/d/1e-ioFmA1nYZk13k-fZf1vQ46-G6X9rkE/view) |
