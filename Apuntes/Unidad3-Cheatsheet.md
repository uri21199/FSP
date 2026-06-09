# Cheatsheet — Cinemática del Cuerpo Rígido (Unidad 3)

> Receta paso a paso para encarar **cualquier** problema de cinemática del CR. Pensá esto como un árbol de decisión: empezás arriba y vas bajando según lo que tenga el problema.

> **Notación**: producto vectorial = **∧** (cuña). Posición de A respecto de B = **r̄_{A→B}** (vector que va de B a A). Torque = **τ**.

---

## ⚙️ Antes que nada: dibujá

Sin dibujo no se puede. Hacé esto SIEMPRE antes de cualquier cuenta:

1. **Dibujá el cuerpo** y la situación física (con piso, pared, soga, lo que haya).
2. **Marcá ejes** (x horizontal, y vertical es lo más común).
3. **Marcá los puntos relevantes** con sus letras (A, B, P, CM, contacto, etc.).
4. **Anotá las posiciones de cada punto respecto del CM** o respecto del origen (lo que te convenga).
5. **Dibujá las velocidades conocidas** como flechitas.
6. **Si conocés Ω**, dibujá una flecha curva indicando el sentido (horario/antihorario).

> Si dibujás bien, el problema se resuelve casi solo. Sin dibujo, te perdés siempre.

---

## 🚦 Paso 1 — ¿Qué tipo de movimiento es?

Marcá una opción:

| Tipo | Cómo lo reconocés | Característica clave |
|---|---|---|
| **Traslación pura** | Todos los puntos tienen la misma v̄. No rota. | Ω̄ = 0 |
| **Rotación pura** | Hay un punto fijo del cuerpo (no se mueve). | v̄_i = Ω̄ ∧ r̄_{i→eje} |
| **Rototraslación** | Caso general. v̄_CM ≠ 0 y Ω̄ ≠ 0. | Se necesitan dos datos |

### Pistas del enunciado

- "Pivote fijo" / "eje fijo" / "articulación" → rotación pura.
- "Rueda sin resbalar" / "RSR" → rototraslación con CIR en el contacto.
- "Está cayendo" / "se desliza" → rototraslación.
- "Se traslada paralelo a..." → traslación pura.

---

## 🎯 Paso 2 — Encontrar el CIR (si te sirve)

El **CIR** es el punto con v̄ = 0. Si lo encontrás, todo el problema se reduce a una rotación pura alrededor del CIR, y eso es mucho más fácil.

### ¿Cuándo conviene buscar el CIR?

- Si te piden velocidades de muchos puntos.
- Si conocés vínculos (RSR, escalera apoyada).
- Si conocés v̄ en dos puntos.

### ¿Cómo lo encontrás?

**Opción A — Pivote fijo**: CIR está en el pivote. Listo.

**Opción B — RSR**: CIR está en el **punto de contacto** con la superficie.

**Opción C — Vínculos geométricos**:
- Punto A pegado a una pared → v̄_A vertical → perpendicular a v̄_A es horizontal.
- Punto B pegado al piso → v̄_B horizontal → perpendicular a v̄_B es vertical.
- Trazá las perpendiculares, donde se cortan está el CIR.

**Opción D — Conozco v̄ en dos puntos A y B con direcciones distintas**:
- Trazá una recta perpendicular a v̄_A pasando por A.
- Trazá una recta perpendicular a v̄_B pasando por B.
- Intersección = CIR.

**Opción E — Conozco v̄_CM y Ω̄**:
- Distancia CM-CIR = |v̄_CM| / |Ω̄|
- Dirección: perpendicular a v̄_CM (del lado tal que la rotación reproduzca v̄_CM).

---

## 🌀 Paso 3 — Calcular Ω (si no lo tenés)

Si conocés **el CIR** y **v̄ de algún punto P**:

  **|Ω| = |v̄_P| / d_{P→CIR}**

donde d_{P→CIR} es la distancia del punto P al CIR.

**Signo de Ω**:
- Antihorario visto desde +z → Ω̄ = +Ω k̂ (sale de la hoja)
- Horario visto desde +z → Ω̄ = −Ω k̂ (entra a la hoja)

**Regla mental rápida**: imaginá un tornillo rotando como el cuerpo. La dirección en la que avanza el tornillo = dirección de Ω̄.

---

## ✏️ Paso 4 — Velocidad de cualquier punto

Dos fórmulas, ambas equivalentes:

### Opción A — Si tenés el CIR

  **v̄_P = Ω̄ ∧ r̄_{P→CIR}**

(Más simple porque solo hay un término.)

### Opción B — Si tenés v̄_CM y Ω̄

  **v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}**

(Más general.)

### Cómo calcular Ω̄ ∧ r̄ en 2D (el atajo)

Si Ω̄ = Ω_z k̂ y r̄ = (a, b), entonces:

  **Ω̄ ∧ r̄ = (−Ω_z · b ; Ω_z · a)**

Memorialo así: "intercambio las componentes, le cambio el signo a la primera, y multiplico por Ω_z".

---

## 🚗 Paso 5 — Caso especial: RSR (Rodadura sin resbalar)

Si te dice "rueda sin resbalar", **siempre** usá:

  **|v̄_CM| = |Ω̄| · R** (módulos)
  **|a̅_CM| = |α̅| · R** (módulos)

### Signos en RSR (eje x horizontal, y vertical, piso abajo)

- Si v̄_CM va en +x (a la derecha) → Ω̄ va en −k̂ (horario, entra a la hoja).
- Si v̄_CM va en −x (a la izquierda) → Ω̄ va en +k̂ (antihorario, sale).

### Velocidades de los 4 puntos cardinales en RSR

Para una rueda con CM moviéndose con v̄_CM:

| Punto | |v̄| | Dirección |
|---|---|---|
| Top (arriba) | **2 · v_CM** | horizontal, mismo sentido que CM |
| Contacto (abajo) | **0** | — (es el CIR) |
| Derecha | v_CM · √2 | 45° (abajo si va a la derecha, arriba si va a la izquierda) |
| Izquierda | v_CM · √2 | 45° (arriba si va a la derecha) |

### Trucazo

**En RSR el rozamiento NO disipa energía**, porque actúa en el punto de contacto que tiene v̄ = 0. Eso significa: **conservación de E_mec se aplica**. Si rueda sin resbalar y no hay otras fuerzas no conservativas, podés usar energía libre.

---

## ⚖️ Paso 6 — Rigidez (cuando me dan dos velocidades)

Si tengo v̄ en dos puntos A y B y quiero **verificar** que es CR:

  **v̄_A · û_{A→B} = v̄_B · û_{A→B}**

Donde û_{A→B} es el versor que va de A a B.

**Significado**: las proyecciones de las dos velocidades sobre la línea AB deben ser iguales. Si no, el cuerpo no es rígido.

**Uso típico**: cuando te dan dos velocidades y querés que el cuerpo sea CR, esta ecuación te da una **condición** que te ayuda a despejar incógnitas.

---

## 🚀 Paso 7 — Aceleraciones (cuando las piden)

  **a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω² · r̄_{P→CM}**

Tres términos:

| Término | Qué representa | Dónde apunta |
|---|---|---|
| **a̅_CM** | Aceleración del CM | Lo que sea (dato del problema) |
| **α̅ ∧ r̄_{P→CM}** | Tangencial (cambio de Ω) | Perpendicular a r̄ |
| **−Ω² · r̄_{P→CM}** | Centrípeta | Hacia el CM (radial) |

### En RSR

  |a̅_CM| = |α̅| · R (módulos, con signo opuesto en componentes)

### Trampita típica

**v̄_C (contacto) = 0 en RSR**, pero **a̅_C ≠ 0**. El contacto tiene aceleración puramente centrípeta (apunta hacia el CM) de módulo Ω² · R.

---

## 🗺️ Mapa visual: qué hacer según el problema

```
   ¿Qué te dan?
        │
        ├──► RSR + R + (v̄_CM ó Ω̄)
        │       └──► Usar |v̄_CM| = |Ω̄|·R, CIR en contacto
        │
        ├──► Pivote fijo + Ω̄
        │       └──► Rotación pura, CIR en pivote
        │
        ├──► v̄ en 2 puntos (con direcciones distintas)
        │       └──► CIR por intersección de perpendiculares
        │
        ├──► Vínculos geométricos (escalera, etc.)
        │       └──► Dirección de v̄_A y v̄_B viene del vínculo
        │
        └──► v̄_CM + Ω̄
                └──► Usar v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM} directo
```

---

## ❌ Errores típicos que te puedes evitar

1. **Aplicar |v̄_CM| = |Ω̄|·R sin que sea RSR**: ¡solo vale si rueda sin resbalar!

2. **Confundir el signo de Ω̄**: si la rueda va a la derecha y RSR, Ω̄ **entra** a la hoja (negativo).

3. **Hacer mal Ω̄ ∧ r̄**: usá el atajo (−Ω·b, Ω·a) para no equivocarte.

4. **Cambiar el sentido de r̄_{P→CM}**: r̄_{P→CM} va **del CM al punto P** (la flecha de la notación va al revés que el vector, pero el vector apunta desde el CM hacia P).

5. **Pensar que el CIR es un punto fijo del cuerpo**: cambia en cada instante.

6. **Olvidar la condición de rigidez cuando dan 2 velocidades**: es información que tenés que usar.

7. **En aceleraciones, olvidar el término centrípeta (−Ω²·r̄)**: a̅_P tiene **tres** términos, no dos.

8. **Confundir v̄_CIR = 0 con a̅_CIR = 0**: a̅_CIR ≠ 0 aunque v̄_CIR = 0.

---

## 🧠 Checklist mental al resolver

Antes de empezar a calcular, hacete estas preguntas:

- [ ] ¿Dibujé la situación con todos los datos?
- [ ] ¿Identifiqué el tipo de movimiento (traslación/rotación/rototraslación)?
- [ ] ¿Hay un vínculo (RSR, pivote, pared, piso)?
- [ ] ¿Conozco o puedo encontrar el CIR?
- [ ] ¿Conozco Ω̄ o lo puedo calcular?
- [ ] ¿Qué punto me piden y dónde está respecto del CM (o del CIR)?

Si respondiste todo, el problema se resuelve mecánicamente.

---

## 📐 Cheatsheet de fórmulas (lo mínimo a memorizar)

| Concepto | Fórmula |
|---|---|
| Velocidad de P (general) | **v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}** |
| Velocidad de P (con CIR) | **v̄_P = Ω̄ ∧ r̄_{P→CIR}** |
| Producto vectorial 2D | **Ω·k̂ ∧ (a, b) = (−Ω·b, Ω·a)** |
| RSR | **|v̄_CM| = |Ω̄|·R** ; **|a̅_CM| = |α̅|·R** |
| Distancia CM-CIR | **d = |v̄_CM| / |Ω̄|** |
| Rigidez | **v̄_A · û_{A→B} = v̄_B · û_{A→B}** |
| Aceleración de P | **a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω²·r̄_{P→CM}** |
