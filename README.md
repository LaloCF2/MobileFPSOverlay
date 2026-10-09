# 📊 FNF V-Slice Mobile FPS Counter

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android%20%7C%20iOS%20%7C%20PC-brightgreen?style=for-the-badge&logo=android" alt="Platform">
  <img src="https://img.shields.io/badge/Base-V--Slice%20(Funkin'%20Crew)-ff69b4?style=for-the-badge" alt="Base">
  <img src="https://img.shields.io/badge/Language-Haxe-orange?style=for-the-badge" alt="Language">
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License">
</p>

---

¡Monitorea el rendimiento de tu juego directamente en la base oficial! **FNF V-Slice Mobile FPS Counter** es un componente avanzado y altamente optimizado, diseñado específicamente para mostrar un contador de fotogramas por segundo (FPS) y consumo de memoria RAM en la versión **V-Slice** de **Friday Night Funkin'**. 

Este script ha sido reescrito desde cero para ofrecer el máximo rendimiento en dispositivos **móviles**, eliminando los problemas de sintaxis y crasheos comunes en Android/iOS, manteniendo al mismo tiempo compatibilidad total con las builds de **escritorio (PC)**.

## ✨ Características Principales

*   ⚙️ **Menú de Opciones Integrado:** Incluye una página nativa dentro del menú de Opciones de V-Slice. Ajusta libremente la escala (tamaño), la opacidad del fondo, y los márgenes de posición (Offset X/Y) sin tocar una sola línea de código.
*   👆 **Alternancia Táctil (Touch Toggle):** ¿Necesitas ver más información en plena partida? Toca el contador de FPS en la pantalla de tu móvil y alternará instantáneamente entre el modo **Simple** y el modo **Avanzado**.
*   🌈 **Resplandor Neón Inteligente:** Activa el *Neon Glow* en los ajustes. El contador emitirá un brillo que cambia de color dinámicamente según tu rendimiento (Cian = Óptimo, Amarillo = Precaución, Rojo = Caída grave de frames). Los límites se calculan automáticamente basándose en la tasa de refresco máxima de tu dispositivo.
*   🎯 **Anti-Distorsión (Zero-Jitter Rendering):** A diferencia de otros contadores que "tiemblan" al actualizar la cámara, este script utiliza posicionamiento matemático exacto de píxeles (`Math.floor`) para mantenerse 100% estático, nítido y sin desenfoques de texto.
*   ⚡ **Detección Automática de Hz:** Detecta si tu pantalla es de 60Hz, 90Hz o 120Hz para sincronizar y ajustar el límite de FPS de forma nativa (con la opción de forzar un límite manual desde el menú).
*   📱 **Ultra-Optimización Móvil:** Código "Bulletproof". Escrito utilizando asignaciones limpias y literales directos en Haxe. Evita fugas de memoria, sobrecarga del *Garbage Collector* y soluciona el clásico error `Unexpected token` de los lectores HScript en V-Slice móvil.

## 🚀 Integración / Cómo usar

Al estar diseñado como un módulo para la base V-Slice, su instalación es rápida y directa mediante la carpeta de `mods`:

1. Descarga los archivos fuente (`.hxc`) desde la sección de [Releases](https://github.com/LaloCF2/MobileFPSOverlay/releases).
2. Copia los scripts y pégalos en la ruta correspondiente según tu sistema operativo:

   * 🤖 **Usuarios Android:** 
     Ruta recomendada: `/storage/emulated/0/Android/data/com.funkycrew.fnf/files/mods/`
   
   * 🍎 **Usuarios iOS:** 
     Ruta recomendada: `iPhone/FNF/mods/`
     
   * 💻 **Usuarios PC:** 
     Pega los archivos en tu carpeta `mods/` ubicada en el directorio raíz de tu juego.

3. Abre el juego, dirígete a **Options -> FPS Custom Config** y personaliza el contador a tu gusto.
