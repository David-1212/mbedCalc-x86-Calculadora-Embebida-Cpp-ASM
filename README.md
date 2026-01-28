# 🧮 EmbedCalc x86 — Calculadora Embebida

Proyecto desarrollado en C++ con integración de ensamblador x86 para la implementación de una calculadora simple en un entorno embebido, enfocado en el aprendizaje de programación de bajo nivel, control de hardware y optimización de recursos.

## 📌 Objetivo del Proyecto

Diseñar una calculadora funcional que combine programación en alto nivel (C++) con rutinas en ensamblador x86 para operaciones críticas, demostrando el uso conjunto de ambos lenguajes en sistemas embebidos.

## ✨ Características

- Operaciones básicas: suma, resta, multiplicación y división
- Rutinas optimizadas en ensamblador x86
- Interfaz por teclado matricial / consola
- Salida en display LCD / terminal
- Manejo directo de registros
- Control de interrupciones
- Bajo consumo de recursos

## 🛠️ Tecnologías Utilizadas

- C++
- Ensamblador x86 (NASM / MASM)
- GCC / MinGW
- Entorno embebido / Emulador
- Microcontrolador / Plataforma x86

## ⚙️ Requisitos

- GCC / G++
- NASM
- Make / CMake
- QEMU / Hardware real (opcional)

## 🔧 Compilación

### Compilación Manual

```bash
nasm -f elf64 calc.asm -o calc.o
g++ -c main.cpp -o main.o
g++ main.o calc.o -o embedcalc
