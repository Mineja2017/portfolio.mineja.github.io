---
title: 3.1 Processing 1
published: true
---

## Introducción

Para comenzar la tercera evaluación se expliará processing que en este caso se usará con JAVA. Podemos descargarlo desde [aquí](https://processing.org/download) y se adjunta esta presentación a modo de introduccion y explicación:

* [Presentación](https://docs.google.com/presentation/d/1hiomSoA2434bbqRuy96HOiNQXeKl4XY3S4YxsTp1oO8/edit#slide=id.p)

## Instrucciones

Se debe crear una figura esquematíca del superheroe *Iron Man* mediante la utilización de las formas explicadas. Además se deberá incluir un pequeño guiño o detalle extra (Corbata, gafas, lazos....)

## Resultado

Para esta práctica he utilizado una funcion que importa una imagen *".svg"* para luego editarla.

```java

PShape iron;

void setup() {

  size(500, 500);
  iron = loadShape("iron_man_icon.svg");
}

void draw() {

  noStroke();
  fill(255,0, 0);
  ellipse(250, 430, 40,40);
  triangle(200, 390, 250, 430, 200, 450);
  triangle(300, 390, 250, 430, 300, 450);
  shape(iron, 150, 100);
}

```

## Area de Descargas

|  Descripción   |     Codigo    |
|:---------------|:------------------|
| Entrega|[Enlace a la carpeta con la imagen y el codigo](https://drive.google.com/file/d/1cczKepKNeiobfeePCqjk-vw2PctHJ2zf/view) |
