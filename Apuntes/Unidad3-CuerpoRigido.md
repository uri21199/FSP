# Guía de conceptos — Unidad 3: Cuerpo Rígido

> Apunte de estudio para Física de Sistemas de Partículas (FSP / 62.01) — FIUBA. Cubre cinemática del CR (CIR, rodadura), momento de inercia, dinámica, energía y equilibrio.

> **Notación**: producto vectorial = **∧** (cuña). Posición de A respecto de B = **r̄_{A→B}** (vector que va de B a A). Torque = **τ**.

---

## Índice

1. [Enfoque general](#0-enfoque-general)
2. [Cinemática del CR](#1-cinematica-del-cr)
3. [Centro instantáneo de rotación (CIR)](#2-centro-instantaneo-de-rotacion-cir)
4. [Rodadura — RSR vs deslizar](#3-rodadura-rsr-vs-deslizar)
5. [Momento de inercia + Steiner](#4-momento-de-inercia-y-steiner)
6. [Dinámica del CR](#5-dinamica-del-cr)
7. [Trabajo y energía en CR](#6-trabajo-y-energia-en-cr)
8. [Equilibrio del CR](#7-equilibrio-del-cr)
9. [Errores conceptuales típicos](#8-errores-conceptuales-tipicos)
10. [Plantilla de resolución](#9-plantilla-de-resolucion)
11. [Apéndice: fórmulas](#apendice-formulas-clave)

---

## 0. Enfoque general

Un cuerpo rígido (CR) es un sistema de partículas donde **las distancias entre cualquier par de partículas no cambian**. Esto agrega una restricción muy fuerte: el cuerpo entero queda descrito por:

- La **velocidad de un punto** (típicamente el CM): **v**_CM
- La **velocidad angular**: **Ω** (común al cuerpo entero)

Con estos dos datos podés calcular la velocidad de **cualquier** punto del cuerpo.

Ante un problema de CR, hacete **siempre estas 4 preguntas**:

1. **¿Qué tipo de movimiento tiene el cuerpo?** Traslación pura, rotación pura, o rototraslación.
2. **¿Hay vínculos?** RSR, pivote fijo, soga, apoyo en pared/piso, etc.
3. **¿Necesito cinemática o dinámica?** (Velocidades/posiciones, o fuerzas/torques)
4. **¿Hay rozamiento?** Si lo hay, ¿es estático (RSR) o dinámico (desliza)? El primero **no disipa**, el segundo sí.

---

## 1. Cinemática del CR

### Tipos de movimiento

| Movimiento | Característica | Ω | v de los puntos |
|---|---|---|---|
| **Traslación pura** | Todas las partículas tienen igual **v** y **a** | Ω = 0 | v_punto = v_CM |
| **Rotación pura** | Alrededor de un eje fijo en el espacio | Ω ≠ 0 | v_punto = Ω ∧ r̄ (r̄ medido desde el eje) |
| **Rototraslación** | Combinación: trasladar + rotar | Ω ≠ 0 | (ver ecuación general abajo) |

### Ecuación general de la cinemática del CR (fundamental)

Para cualquier par de puntos P y Q del cuerpo:

  **v**_P = **v**_Q + **Ω** ∧ **r**_{P→Q}

Donde **r**_{P→Q} es el vector que va **de Q a P**.

Caso típico (P respecto del CM):
  **v**_P = **v**_CM + **Ω** ∧ **r**_{P→CM}

Para aceleración (2D, plano):
  **a**_P = **a**_CM + **α** ∧ **r**_{P→CM} − Ω² · **r**_{P→CM}

Donde:
- **α** ∧ **r**_{P→CM} = componente **tangencial** (cambio de Ω)
- −Ω² · **r**_{P→CM} = componente **centrípeta** (apunta hacia el CM)

### Condición de rigidez

Para dos puntos cualesquiera A y B del cuerpo, **sus velocidades proyectadas sobre la línea AB deben ser iguales** (si fueran distintas, A y B se acercarían/alejarían y no sería rígido).

  **v**_A · û_AB = **v**_B · û_AB

(donde û_AB es el versor de A hacia B)

Esto te sirve cuando te dan dos velocidades y querés verificar si el cuerpo es rígido (Ej. 1 de la guía).

---

## 2. Centro instantáneo de rotación (CIR)

### Definición

El **CIR** es el punto (real o imaginario) del cuerpo cuya velocidad en ese instante es **cero**. Es decir:

  **v**_CIR = **0**

Como consecuencia, el cuerpo entero **rota instantáneamente alrededor del CIR**:

  **v**_cualquier_punto = **Ω** ∧ **r**_{punto→CIR}

> **Importante**: el CIR cambia de un instante al siguiente. **No es un punto material** del cuerpo (a menos que coincida momentáneamente con uno).

### Por qué es útil

Te convierte una rototraslación en una **rotación pura "equivalente" alrededor del CIR**. Eso permite calcular velocidades de cualquier punto como si fuera rotación pura → mucho más simple.

### Cómo encontrarlo — 3 métodos

#### Método 1 — Gráfico (cuando conocés dos velocidades)

Si conocés **v** en dos puntos A y B del cuerpo (no paralelas):

1. Dibujá la perpendicular a **v**_A pasando por A.
2. Dibujá la perpendicular a **v**_B pasando por B.
3. **El CIR es la intersección**.

```
        v_A
         ↑
         A ─ ─ ─ ─ ─ ┐ (perp. a v_A)
                     │
                     │
                     ●  CIR (intersección)
                     │
         B ─ ─ ─ ─ ─ ┘ (perp. a v_B)
         ↑
        v_B
```

Razón: la velocidad de cualquier punto del cuerpo es perpendicular al vector que va del CIR a ese punto.

#### Método 2 — Analítico (conociendo v_CM y Ω)

  **r**_CIR = **r**_CM + (**Ω** ∧ **v**_CM) / Ω²

En 2D (módulo y dirección):
- Distancia del CM al CIR: **d = |v_CM| / |Ω|**
- Dirección: perpendicular a **v**_CM, del lado donde la rotación alrededor del CIR reproduce v_CM.

#### Método 3 — Caso especial RSR

Si el cuerpo rueda sin deslizar sobre una superficie, **el CIR está en el punto de contacto**.

### Casos típicos

| Movimiento | Dónde está el CIR |
|---|---|
| Traslación pura (Ω = 0) | "En el infinito" (no existe en sentido finito) |
| Rotación pura | En el eje fijo |
| Rodadura RSR | En el punto de contacto |
| Rodadura deslizando | Por debajo del piso (si v_CM > Ω·R) o por arriba (si v_CM < Ω·R) |

---

## 3. Rodadura — RSR vs deslizar

### Condición de RSR (Rodar Sin Resbalar)

  **v_CM = Ω · R**       (relación entre módulos)

Esto sale de que el CIR está en el punto de contacto, así que v_contacto = 0.

También vale para aceleraciones:
  **a_CM = α · R**

### Velocidades y aceleraciones de puntos típicos en RSR

Para un disco/cilindro de radio R rodando sin deslizar:

```
                  ●  T (top)
                / │ \
               /  │  \
         B ●     ● CM     ● F
               \  │  /
                \ │ /
                  ●  C (contacto)
              ═════════
```

| Punto | Velocidad (módulo) | Dirección |
|---|---|---|
| Centro (CM) | v_CM | horizontal, sentido del movimiento |
| Top (T) | **2 · v_CM** | horizontal, sentido del movimiento |
| Contacto (C) | **0** (es el CIR) | — |
| Front (F) | v_CM · √2 | a 45° hacia arriba-adelante |
| Back (B) | v_CM · √2 | a 45° hacia arriba-atrás |

> **Truco**: para cualquier punto del cuerpo, usá **v_punto = Ω ∧ r_{punto→CIR}**. Con CIR en el contacto, podés sacar todo.

### Si NO rueda sin deslizar (rueda deslizando)

Dos casos:

#### Caso A: v_CM > Ω·R (deslizamiento "hacia adelante")
- El punto de contacto se mueve **hacia adelante** respecto del piso.
- Rozamiento sobre el cuerpo: **hacia atrás** (oponiéndose al deslizamiento).
- Ejemplo: ruedas de auto frenando en hielo.

#### Caso B: v_CM < Ω·R (deslizamiento "hacia atrás", patinaje)
- El punto de contacto se mueve **hacia atrás** respecto del piso.
- Rozamiento sobre el cuerpo: **hacia adelante**.
- Ejemplo: ruedas de auto acelerando con neumáticos pelados.

En cualquier caso de deslizamiento, el rozamiento es **dinámico** (f_d = μ_d · N) y **DISIPA energía**.

### Resumen rozamiento en rodadura

| Situación | Tipo de rozamiento | ¿Disipa? |
|---|---|---|
| RSR | Estático (f_s ≤ μ_s · N) | **NO** (W = 0) |
| Rueda deslizando | Dinámico (f_d = μ_d · N) | **SÍ** |

---

## 4. Momento de inercia y Steiner

### Definición

  **I = Σ mᵢ · rᵢ²**    (sumatoria, para sistema discreto)
  **I = ∫ r² dm**       (integral, para cuerpo continuo)

Donde r = distancia perpendicular de cada partícula al eje.

**Es lo análogo a la masa para movimientos rotacionales.** Mide la "inercia rotacional": cuánto cuesta cambiar Ω.

### Tabla de momentos de inercia (eje por CM, perpendicular)

| Cuerpo | I_CM |
|---|---|
| Aro o tubo cilíndrico delgado (radio R) | M · R² |
| Disco o cilindro macizo (radio R) | (1/2) · M · R² |
| Esfera maciza (radio R) | (2/5) · M · R² |
| Esfera hueca (radio R) | (2/3) · M · R² |
| Barra delgada (eje ⊥ por el CM, largo L) | (1/12) · M · L² |
| Barra delgada (eje ⊥ por un extremo, largo L) | (1/3) · M · L² |
| Placa rectangular (a × b, eje ⊥ por CM) | (1/12) · M · (a² + b²) |

### Teorema de Steiner (ejes paralelos)

  **I_eje = I_CM + M · d²**

Donde d = distancia perpendicular entre el eje (que NO pasa por el CM) y un eje paralelo que sí pasa por el CM.

**Reglas importantes**:
- Steiner **solo vale entre ejes paralelos**.
- El I respecto a un eje por el CM es **siempre el mínimo** entre todos los ejes paralelos posibles.
- Si te dan I respecto a un eje fuera del CM y querés el I respecto a un eje paralelo en otra ubicación: pasá primero por el CM (calculá I_CM, después aplicá Steiner al nuevo).

### Radio de giro

  **R_g = √(I/M)**     →     **I = M · R_g²**

Es la distancia a la que tendrías que concentrar toda la masa M para obtener el mismo I.

### CR compuestos (Ejs. 9, 11)

Para un cuerpo formado por varias piezas:

  I_total = Σ I_pieza_i      (cada I respecto del MISMO eje)

Si las piezas tienen su I_CM tabulado, usá Steiner para llevarlas al eje común.

---

## 5. Dinámica del CR

### Las dos ecuaciones fundamentales

Para describir el movimiento de un CR necesitás **dos ecuaciones** (porque tiene 2 grados de libertad en movimiento plano: traslación + rotación):

**(1) Traslación del CM**:
  **Σ F**_ext = M · **a**_CM

(igual que para sistemas de partículas)

**(2) Rotación**:
  **Σ τ**_X = I_X · **α**

Donde τ_X es la suma de **torques externos** respecto del punto X, y I_X es el momento de inercia respecto al eje por X.

### ¿Respecto a qué punto X?

La ecuación (2) **es válida en general respecto a**:
- **El CM** (siempre válida, sin excepciones).
- **Un punto fijo en el espacio** (típicamente un pivote).
- **El CIR** (en algunos casos — con cuidado, sobre todo si acelera).

> **Regla práctica para parcial**: si el cuerpo tiene un **pivote fijo**, tomá momentos **respecto al pivote** (te ahorra tener que conocer la fuerza de vínculo, que sale después de a_CM).
> Si rueda libre, tomá momentos **respecto al CM**.

### Cómo plantear un problema de dinámica de CR

1. **DCL** del cuerpo: dibujar TODAS las fuerzas externas con su punto de aplicación.
2. Escribir **F_neta = M · a_CM** (componente a componente).
3. Elegir un punto X y escribir **τ_X = I_X · α**.
4. Si hay vínculos (RSR, pivote, soga), agregar las **ecuaciones de vínculo**:
   - RSR: a_CM = α · R
   - Cuerda inextensible: a_bloque = a_punto_cuerda_del_CR
5. Resolver el sistema (típicamente 3 ecuaciones, 3 incógnitas: 2 componentes de a_CM y α; o a_CM, α, f).

### Caso típico — esfera RSR por plano inclinado (Ej. 27)

Plano inclinado de ángulo α. Esfera maciza con I_CM = (2/5)·M·R².

- DCL: peso (Mg ↓), normal (⊥ plano), rozamiento f (estático, opone al movimiento relativo).
- Eje x = pendiente abajo:
  Σ F_x: M·g·sin(α) − f = M·a_CM
- Torque respecto al CM (la normal y el peso no torquean porque pasan por el CM):
  Σ τ_CM: f · R = I_CM · α = (2/5)·M·R²·α
- RSR: a_CM = α · R → α = a_CM / R
- Resolviendo:
  f = (2/5)·M·a_CM
  M·g·sin(α) − (2/5)·M·a_CM = M·a_CM
  g·sin(α) = (7/5)·a_CM
  **a_CM = (5/7) · g · sin(α)**

> Comparalo con un bloque sin rotar: a = g·sin(α). El cilindro/esfera baja **más lento** porque parte de la energía se va a rotación.

---

## 6. Trabajo y energía en CR

### Energía cinética total

  **K = K_traslación + K_rotación = (1/2)·M·v_CM² + (1/2)·I_CM·Ω²**

> Esta es la **fórmula clave**. Tiene **dos términos**, no uno solo. Olvidarse de cualquiera de los dos es el error #1 en parciales.

### Caso especial: RSR

Como v_CM = Ω·R:

  K = (1/2)·M·v_CM² + (1/2)·I_CM·(v_CM/R)²
  K = (1/2)·v_CM² · (M + I_CM/R²)

Para una esfera maciza (I_CM = (2/5)·M·R²):
  K = (1/2)·v_CM² · M · (1 + 2/5) = (7/10)·M·v_CM²

(O sea: 5/7 de K es traslación, 2/7 es rotación.)

### Trabajo de un torque

  **W_τ = ∫ τ · dθ**

Si τ es constante: W_τ = τ · Δθ

Si conocés Ω inicial y final:
  W_τ = ΔK_rotación = (1/2)·I·(Ω_f² − Ω_i²)

### Trabajo del rozamiento en RSR — el concepto MÁS importante de la unidad

**Pregunta**: si la pelota baja una rampa rodando sin resbalar, ¿el rozamiento le quita energía?

**Respuesta**: **NO**. El rozamiento estático en RSR **no hace trabajo**, ni positivo ni negativo.

#### ¿Por qué?

El trabajo de una fuerza es W = ∫ **F** · **v**_contacto dt. En RSR, el punto de contacto entre cuerpo y piso tiene **velocidad instantánea cero** (es el CIR). Entonces:

  W_rozamiento_estático_RSR = ∫ f · 0 dt = **0**

#### Lo que SÍ hace el rozamiento estático

Aunque no hace trabajo (no disipa), el rozamiento sí:
- **Aplica una fuerza** sobre el cuerpo (entra en F = M·a).
- **Genera un torque** respecto del CM (entra en τ = I·α).

Es lo que permite que la pelota ruede en lugar de simplemente deslizar.

#### Energía conservada en RSR

Como no hay disipación, **E_mec se conserva**. Esto permite atacar el problema por energía:

  m·g·h_inicial = (1/2)·M·v_CM² + (1/2)·I_CM·Ω²

Súper útil cuando solo te piden la velocidad final.

### Trabajo del rozamiento cuando NO es RSR

Si el cuerpo rueda deslizando, el rozamiento es dinámico y:

  W_f = −f · Δx_relativo

Donde Δx_relativo es el desplazamiento del punto de contacto respecto al piso. **SÍ disipa energía** (igual que en Ej. 16 de Unidad 2 con bloque sobre carro).

---

## 7. Equilibrio del CR

Un CR está en equilibrio si:

  **Σ F**_ext = **0**       (no se traslada)
  **Σ τ**_ext = **0**       (no rota)

La segunda ecuación vale **respecto a CUALQUIER punto** (en equilibrio dan todas lo mismo). Eso lo aprovechás eligiendo el punto astutamente.

### Estrategia para problemas de estática

1. **DCL completo**: todas las fuerzas con su punto de aplicación.
2. **Identificá incógnitas**: tensiones, reacciones en vínculos, ángulos, distancias.
3. **Componentes de F = 0**: una ecuación por cada eje (típicamente x e y).
4. **Σ τ = 0**: elegir el punto de momentos donde se anulen **el mayor número de incógnitas** (típicamente donde se cruzan varias líneas de acción).

> **Truco clásico**: si una incógnita actúa en un punto X, tomá momentos respecto a X → esa incógnita no aparece.

### Tipos de vínculos típicos

| Vínculo | Reacciones |
|---|---|
| Apoyo en superficie lisa | Solo normal (⊥ superficie) |
| Apoyo en superficie con rozamiento | Normal + fuerza tangente (≤ μ·N) |
| Articulación / pivote | Reacción de dirección desconocida (2 componentes) |
| Soga ideal | Tensión en dirección de la soga (solo tira) |
| Pared lisa | Normal perpendicular a la pared |

### Ejemplo — escalera apoyada (Ej. 17)

Escalera de masa M en pared lisa y piso con rozamiento, ángulo α con el piso. Pintor de masa m a distancia d desde el pie.

Incógnitas: N_piso, N_pared, f.

Ecuaciones:
1. Σ F_x: f − N_pared = 0
2. Σ F_y: N_piso − M·g − m·g = 0
3. Σ τ_pie_de_la_escalera = 0: M·g·(L/2)·cos(α) + m·g·d·cos(α) − N_pared·L·sin(α) = 0

(Tomé el pie como pivote → N_piso y f no aparecen, ya despejé directamente N_pared.)

Para que **no resbale**: f ≤ μ·N_piso. Esto te da el ángulo mínimo.

---

## 8. Errores conceptuales típicos

1. **Usar v = Ω·R sin verificar RSR**: solo vale cuando el CIR está en el punto de contacto. Si rueda deslizando, ¡FALSO!

2. **Olvidar el término rotacional de K**: K_total = (1/2)·M·v² + (1/2)·I·Ω². Si solo escribís (1/2)·M·v², subestimás la energía.

3. **No usar Steiner cuando corresponde**: si el eje no pasa por el CM, tenés que sumar M·d². Por ejemplo, en una barra pivoteada en un extremo, I = (1/3)·M·L², no (1/12)·M·L².

4. **Confundirse en dirección del rozamiento**: en RSR, el rozamiento es estático y va en el sentido que **evita el deslizamiento que tendería a ocurrir**. Si la rueda sube una rampa, el rozamiento va hacia arriba; si baja, hacia arriba también (parece raro pero es así).

5. **Pensar que rozamiento estático NO puede acelerar el cuerpo**: sí puede. No disipa, pero sí aplica fuerza y torque.

6. **Confundir torque respecto del CIR con torque respecto del CM**: no son iguales. La ecuación τ = I·α es más confiable aplicada al CM.

7. **CIR como "punto material"**: no lo es. Es un punto matemático que cambia de instante a instante.

8. **Tratar a la rampa móvil como fija** (Ej. 35): si la base se mueve, hay que considerar el CIR en el marco del laboratorio, NO en el marco de la rampa.

9. **Asumir que dos cuerpos con misma masa y radio tienen mismo I**: NO. Disco macizo = (1/2)MR², aro = MR², esfera maciza = (2/5)MR². La distribución importa.

---

## 9. Plantilla de resolución

### Para cinemática (encontrar v de puntos, CIR)

```
1. ¿Qué tipo de movimiento es? Traslación / rotación / rototraslación.
2. Dato: v_CM y Ω (o algunos puntos)
3. Si me piden CIR: aplico método gráfico o analítico.
4. v_punto = v_CM + Ω ∧ r_{punto→CM}
5. Verifico: ¿tiene sentido la dirección?
```

### Para dinámica (encontrar a, α, fuerzas)

```
1. SISTEMA: ¿qué cuerpo(s) considero?
2. DCL: todas las fuerzas con su punto de aplicación.
3. ¿Hay vínculos? RSR, pivote, soga.
4. Ecuaciones:
   - F_x = M·a_CM_x
   - F_y = M·a_CM_y
   - τ_punto = I_punto · α
   - Ecuaciones de vínculo (RSR: a = α·R)
5. Verifico número de incógnitas vs ecuaciones.
6. Resuelvo.
7. Verifico signos y unidades.
```

### Para energía (encontrar v finales)

```
1. ¿Se conserva E_mec?
   - Sí, si no hay rozamiento dinámico ni choques inelásticos.
   - RSR: SÍ se conserva (rozamiento estático no disipa).
2. Estados inicial y final.
3. K_total = (1/2)·M·v_CM² + (1/2)·I_CM·Ω² (¡los dos términos!)
4. Si RSR: usar v_CM = Ω·R para reducir incógnitas.
5. Igualar E_i = E_f y despejar.
```

### Para equilibrio (estática)

```
1. DCL.
2. Σ F_x = 0, Σ F_y = 0.
3. Σ τ_X = 0 (elegir X astutamente).
4. Verificar número de ecuaciones vs incógnitas.
5. Si pide condición límite (no desliza, no vuelca): igualdad f = μ·N en el límite.
```

---

## Apéndice: fórmulas clave

### Cinemática

| Concepto | Fórmula |
|---|---|
| Ec. general velocidad | **v**_P = **v**_Q + **Ω** ∧ **r**_{P→Q} |
| Ec. general aceleración (2D) | **a**_P = **a**_CM + **α** ∧ **r**_{P→CM} − Ω²·**r**_{P→CM} |
| Condición de rigidez | **v**_A · û_AB = **v**_B · û_AB |
| CIR (analítico) | **r**_CIR = **r**_CM + (**Ω** ∧ **v**_CM) / Ω² |
| Distancia CM-CIR (2D) | d = \|v_CM\| / \|Ω\| |
| Condición de RSR | v_CM = Ω · R   ;   a_CM = α · R |

### Momento de inercia

| Concepto | Fórmula |
|---|---|
| Definición | I = Σ mᵢ·rᵢ²  =  ∫ r² dm |
| Steiner | I_eje = I_CM + M·d² |
| Radio de giro | R_g = √(I/M)   ;   I = M·R_g² |
| Aro/tubo | I_CM = M·R² |
| Disco/cilindro macizo | I_CM = (1/2)·M·R² |
| Esfera maciza | I_CM = (2/5)·M·R² |
| Esfera hueca | I_CM = (2/3)·M·R² |
| Barra (eje por CM) | I = (1/12)·M·L² |
| Barra (eje por extremo) | I = (1/3)·M·L² |

### Dinámica

| Concepto | Fórmula |
|---|---|
| Traslación | Σ **F**_ext = M · **a**_CM |
| Rotación | Σ **τ**_X = I_X · **α** |
| Torque de una fuerza | **τ** = **r** ∧ **F** |
| Momento angular CR | **L**_CM = I_CM · **Ω** |
| König (energía) | K = K_CM + (1/2)·M·v_CM² |

### Energía y trabajo

| Concepto | Fórmula |
|---|---|
| K total CR | K = (1/2)·M·v_CM² + (1/2)·I_CM·Ω² |
| K en RSR (cilindro/disco) | K = (3/4)·M·v_CM² |
| K en RSR (esfera maciza) | K = (7/10)·M·v_CM² |
| K en RSR (aro) | K = M·v_CM² |
| Trabajo de un torque | W_τ = ∫ τ dθ ; constante: τ·Δθ |
| Trabajo rozamiento (RSR) | W = 0 (no disipa) |
| Trabajo rozamiento (desliza) | W = −f · Δx_relativo |

### Equilibrio

| Condición | Ecuación |
|---|---|
| Equilibrio traslacional | Σ **F**_ext = **0** |
| Equilibrio rotacional | Σ **τ**_X = **0** (respecto a CUALQUIER X) |
| Rozamiento límite | f_máx = μ_s · N |
