# Sudoku 4x4

Una aplicación de consola en Python para jugar Sudoku en una versión de tablero 4x4.

## Descripción

Este proyecto implementa un juego de Sudoku 4x4 que se ejecuta en la consola. El juego incluye:

- Diferentes niveles de dificultad (Fácil y Difícil)
- Múltiples opciones de visualización (Numérica, Letras y Símbolos)
- Sistema de puntuación con bonificación por rachas
- Registro de mejores puntajes

## Características

- **Tipos de visualización**: Elija entre números (1-4), letras (A-D) o símbolos (♠,♥,♦,♣)
- **Niveles de dificultad**: 
  - Fácil: 6 casillas vacías, tablero con bordes de asteriscos
  - Difícil: 10 casillas vacías, tablero con bordes de guiones
- **Sistema de puntuación**: 
  - 10 puntos base por cada tablero resuelto
  - Puntos adicionales por victorias consecutivas: +0, +1, +3, +7... puntos
- **Registro de mejores puntajes**: Guarda los 5 mejores puntajes con nombres de los jugadores

## Requisitos

- Python 3.6 o superior

## Estructura del proyecto

```
sudoku/
├── README.md               # Este archivo
├── main.py                 # Punto de entrada de la aplicación
├── src/                    # Código fuente
│   ├── board/              # Módulos relacionados con el tablero
│   │   ├── board.py        # Lógica del tablero de Sudoku
│   │   └── visualization.py # Visualización del tablero
│   ├── game/               # Lógica principal del juego
│   │   ├── game.py         # Gestión del juego
│   │   ├── difficulty.py   # Manejo de dificultad
│   │   └── scoring.py      # Sistema de puntuación
│   ├── menu/               # Interfaz de usuario
│   │   └── menu.py         # Menú principal
│   └── utils/              # Utilidades
│       ├── constants.py    # Constantes del juego
│       └── file_manager.py # Gestión de archivos
└── data/                   # Datos persistentes
    └── highscores.json     # Registro de mejores puntajes
```

## Cómo jugar

1. Clone el repositorio o descargue los archivos
2. Ejecute el juego con Python: `py main.py`
3. Siga las instrucciones en pantalla:
   - Seleccione el tipo de visualización
   - Elija el nivel de dificultad
   - Complete los tableros para acumular puntos
   - Los tableros se completan ingresando fila, columna y valor separados por espacio

## Reglas del Sudoku 4x4

- Se deben completar los cuadros vacíos con un solo número del 1 al 4
- En una fila no puede haber números repetidos
- En una columna no puede haber números repetidos
- En una región (cuadrado 2x2) no puede haber números repetidos

## Desarrollo

Este proyecto fue desarrollado siguiendo la metodología Scrum, con:
- Historias de usuario priorizadas
- Sprints con tareas asignadas
- Reuniones diarias de seguimiento
- Revisiones y retrospectivas