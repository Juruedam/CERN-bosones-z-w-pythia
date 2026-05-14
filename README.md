# Procesamiento de datos del CERN y simulación de decaimientos de bosones Z y W

Proyecto académico — Física de partículas computacional · Universidad Nacional de Colombia (2023)

## El problema

Validar empíricamente la masa de los bosones W y Z reproduciendo sus distribuciones
características (momento transversal y masa invariante) tanto desde una **simulación
Monte Carlo** como desde **datos reales** del CERN, y comparar ambos resultados.

## Qué hice?

**Parte 1 — Simulación Monte Carlo (Pythia):**
- Configuré simulaciones en Pythia para procesos de decaimiento de bosones Z y W.
- Generé **100,000 eventos** por bosón y extraje las distribuciones de momento
  transversal (pT) y masa invariante.

**Parte 2 — Procesamiento de datos reales (CERN Open Data):**
- Descargué y procesé datos abiertos del CERN sobre eventos de decaimiento de los
  mismos bosones.
- Construí el pipeline completo de tratamiento: limpieza, filtrado por cortes
  físicos relevantes, y reconstrucción de las mismas dos distribuciones (pT y masa
  invariante) a partir de los datos crudos.

**Parte 3 — Validación cruzada:**
- Comparé las distribuciones de simulación vs. datos reales.
- Verifiqué que la masa invariante en **ambos** casos se centra en la masa
  conocida de cada bosón.

## Resultado

Las distribuciones simuladas y empíricas muestran alta concordancia, y los picos
de masa invariante coinciden con los valores reportados para los bosones W
(~80 GeV) y Z (~91 GeV).

## Por qué es relevante fuera de física de partículas?

Este proyecto demuestra capacidad para:
- Ejecutar simulaciones **Monte Carlo a escala** (cientos de miles de eventos).
- Construir **pipelines de procesamiento de datos masivos** desde fuentes crudas
  reales.
- Aplicar **validación cruzada empírica** entre modelos y datos.

Son las mismas técnicas que se usan en pronóstico financiero, modelado de demanda
energética y cualquier escenario donde haya que validar un modelo contra datos
operacionales.

## Stack técnico

`Python` · `Pythia` · `NumPy` · `pandas` · `Matplotlib` · `Jupyter` · CERN Open
Data · simulación Monte Carlo

## Contenido del repositorio

- `Bosón W/` — notebooks y datos del decaimiento W.
- `Bosón Z/` — notebooks y datos del decaimiento Z.
- `WyZ_Pythia-CERN.pdf` — documento final con metodología y resultados.
