# 🃏 Ouite

> Juego de cartas para dos jugadores en la consola de Windows, hecho en C++ con cartas dibujadas en caracteres ASCII extendidos y animación de reparto.

## Sobre el proyecto

**Ouite** es un juego de cartas por rondas para dos jugadores en la misma computadora. Cada jugador recibe 8 cartas; en cada ronda sale una carta al azar y gana puntos quien tenga ese valor en su mano y lo descarte.

## Cómo se juega

1. Se reparten **8 cartas** a cada jugador (valores del 1 al 13, con 4 palos).
2. Antes de empezar eliges cuántas **rondas** jugar (entre 5 y 10) y escribes el nombre de cada jugador.
3. En cada ronda la computadora voltea una **carta al azar** con una animación.
4. Por turnos, cada jugador mira su mano e indica el **valor (1-13)** de la carta que quiere eliminar, o escribe `0` para pasar.
5. Si la carta coincide con la de la mesa, se descarta y suma **1 punto**.
6. Al terminar las rondas, gana quien tenga **más puntos** (o hay empate).

### Menú principal

| Tecla | Opción |
|---|---|
| `J` | Jugar |
| `I` | Instrucciones |
| `C` | Créditos |
| `S` | Salir |

## Características

- Juego local para 2 jugadores con nombres personalizados.
- Rondas configurables (5 a 10).
- Cartas del 1 al 13 con 4 palos, dibujadas carácter por carácter.
- Animación al voltear la carta de la ronda.
- Texto que aparece letra por letra, pantalla de título, instrucciones, créditos y pantalla de despedida.
- Marcador en pantalla y resultado final con ganador o empate.

## Requisitos

- Windows
- Visual Studio con soporte de **C++/CLI** (el código usa `System::Console` y `pch.h`). Se crea como proyecto *CLR Console App*. TODO: indicar versión de Visual Studio / .NET Framework.
- Consola de al menos **105 × 30** caracteres. El programa ajusta el tamaño al iniciar, pero la terminal debe permitirlo.
- Recomendado: `cmd.exe` o la consola clásica de Windows. Los colores usan `SetConsoleTextAttribute`, así que no dependen de secuencias ANSI. TODO: confirmar que se ve bien en Windows Terminal.

## Cómo ejecutarlo

1. Abre la solución en Visual Studio.
2. Compila en modo **Release** (o Debug).
3. Ejecuta el `.exe`.

## Estructura

```
.
├── ouite.cpp       # TODO: ajustar al nombre real del archivo
├── pch.h
└── README.md
```
