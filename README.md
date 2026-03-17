# Wild Gunman - Shooter 2D (SFML)

<p align="center">
  Juego de disparos inspirado en el clásico Wild Gunman, desarrollado en C++ con SFML.
</p>

<p align="center">

![C++](https://img.shields.io/badge/language-C%2B%2B-blue)
![SFML](https://img.shields.io/badge/library-SFML-green)
![Game](https://img.shields.io/badge/type-shooter-orange)
![IDE](https://img.shields.io/badge/IDE-Visual%20Studio-purple)

</p>

---

## Descripción

Juego de disparos en 2D donde el jugador debe reaccionar rápidamente para eliminar enemigos que aparecen en ventanas de un saloon.

El jugador utiliza la mira del mouse para apuntar y disparar.  
El objetivo es eliminar enemigos evitando disparar a inocentes.

El juego termina cuando:

- Se eliminan **10 enemigos (victoria)**  
- Se pierden **todas las vidas (derrota)**  

---

## Mecánicas del Juego

- Aparición aleatoria de personajes en ventanas
- Sistema de disparo con mouse
- Diferenciación entre **enemigos** e **inocentes**
- Sistema de vidas y puntaje
- Enemigos que disparan automáticamente si no reaccionás a tiempo
- Efecto visual de disparo (Bang)
- Pantallas de inicio y final

---

## Controles

| Acción | Control |
|------|--------|
| Apuntar | Mouse |
| Disparar | Click izquierdo |
| Comenzar juego | Barra espaciadora |
| Salir | ESC |

---

## Reglas del Juego

- Disparar a un enemigo: **+1 punto**
- Disparar a un inocente: **-1 vida y penalización de puntos**
- Si el enemigo dispara: **-1 vida**
- Ganás al eliminar **10 enemigos**
- Perdés al quedarte sin vidas

---

## Tecnologías Utilizadas

- C++
- SFML (Graphics, Window, System, Audio)
- Programación Orientada a Objetos
- Visual Studio

---

## Arquitectura del Proyecto

El juego está estructurado en múltiples clases:


### Game
Controla el flujo completo del juego:
- Inicio
- Gameplay
- Pantalla final

### Inicio
Pantalla inicial con instrucciones del juego.

### Saloon
Escena principal donde ocurre el gameplay:
- Manejo de ventanas
- Spawn de personajes
- Sistema de disparos
- Control de vidas y puntos

### Personaje
Representa los personajes del juego:
- Enemigos
- Inocentes
- Manejo de sprites y colisiones con el mouse

### PlayerCrosshair
Controla la mira del jugador:
- Posición con el mouse
- Renderizado del cursor personalizado

### Bang
Efecto visual de disparo.

### Final
Pantalla de resultado:
- Victoria o derrota
- Muestra puntaje y vidas restantes

---


## Gameplay

El jugador debe reaccionar rápidamente cuando aparece un personaje en pantalla.

- Si dispara a un enemigo → suma puntos  
- Si dispara a un inocente → pierde vida  
- Si tarda demasiado → el enemigo dispara  

La dificultad está en la velocidad de reacción.

---

## Capturas de Pantalla

<p align="center">

<img src="https://github.com/user-attachments/assets/597d98e3-57b8-4c3d-8fb3-9bc811e892a7"
width="30%"
style="border:3px solid #555; margin:10px; border-radius:8px;">

<img src="https://github.com/user-attachments/assets/036e8750-0a47-4a9b-a0f1-8e229af96662"
width="30%"
style="border:3px solid #555; margin:10px; border-radius:8px;">

<img src="https://github.com/user-attachments/assets/b9bad25f-db4e-4f94-a19a-11dc3c4c0af3"
width="30%"
style="border:3px solid #555; margin:10px; border-radius:8px;">

</p>


---

## Autor

Lucas Boffa  
Tecnicatura en Diseño y Desarrollo de Videojuegos  
UNL
