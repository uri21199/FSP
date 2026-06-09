# Guía de conceptos — Unidad 2: Sistemas de Partículas

> Apunte de estudio para Física de Sistemas de Partículas (FSP / 62.01) — FIUBA. Cubre los temas de la Unidad 2 de la Guía v5: impulso, cantidad de movimiento, centro de masa, choques y momento angular.

---

## Índice

1. [Enfoque general](#0-enfoque-general)
2. [Cantidad de movimiento e impulso](#1-cantidad-de-movimiento-e-impulso-lineal)
3. [Centro de masa](#2-centro-de-masa-cm)
4. [Relación lab — CM (König)](#3-la-relación-lab--cm-konig)
5. [Choques](#4-choques)
6. [Momento angular (cinético)](#5-momento-angular-momento-cinético)
7. [Tabla resumen: qué se conserva](#6-tabla-resumen-que-se-conserva-cuando)
8. [Errores típicos](#7-errores-conceptuales-tipicos)
9. [Plantilla de resolución](#8-plantilla-de-resolución)

---

## 0. Enfoque general

Ante cualquier problema de sistemas de partículas, hacete **siempre estas 4 preguntas en orden**:

1. **¿Cuál es mi sistema?** ¿Qué cuerpos incluyo? ¿La cuerda, el resorte, la rampa?
2. **¿Qué fuerzas son internas y cuáles externas a ese sistema?** Las internas se cancelan de a pares por 3ra de Newton. Las externas son las únicas que pueden cambiar **P**_sistema y **L**_sistema.
3. **¿Hay alguna dirección donde la suma de fuerzas externas sea cero?** Ahí se conserva **esa componente** de **P**.
4. **¿Hay rozamiento que disipa, o choque inelástico?** Si sí → no se conserva la energía cinética. Si no → suele conservarse.

Este checklist mental es la diferencia entre saberse las fórmulas y poder usarlas en un parcial.

---

## 1. Cantidad de movimiento e impulso lineal

### Definiciones

- **Cantidad de movimiento (momento lineal) de una partícula**:

  **p** = m · **v**   [kg·m/s]

- **Cantidad de movimiento de un sistema**:

  **P** = Σ mᵢ · **vᵢ** = M · **v**_CM ,   con M = Σ mᵢ

- **Impulso de una fuerza** entre t₁ y t₂:

  **J** = ∫ **F** dt   [N·s = kg·m/s]

  Si **F** es constante: **J** = **F** · Δt.
  Si **F** = **F**(t) varía: **J** = área bajo la curva F vs t.

### Teorema fundamental (impulso–momento)

**J**_neto = Δ**p** = **p**_final − **p**_inicial

Aplica tanto a una partícula como al sistema (con **P** y la suma de impulsos de las fuerzas externas).

### Diferencias clave (Ej. 1)

| Cantidad | **p** = m·v | **J** = ∫F dt |
|---|---|---|
| Qué describe | Estado de movimiento en un instante | Efecto de una fuerza sobre un intervalo |
| Cuándo lo usás | Momentos antes/después de un choque | Calcular cómo una fuerza variable cambia el estado |
| Unidad | kg·m/s | N·s (idéntica) |

### Conservación de **P** del sistema

- Se conserva ↔ Σ **F**_externas = **0**
- Se conserva la componente x ↔ Σ F_externas,x = 0

> **Truco mental**: en choques, durante el contacto el peso casi nunca importa (Δt es muy chico → su impulso es despreciable frente al de la fuerza del choque). Por eso "se conserva p en choques" aunque haya gravedad.

---

## 2. Centro de masa (CM)

### Definiciones

- **Posición**: **r**_CM = (Σ mᵢ · **rᵢ**) / M
- **Velocidad**: **v**_CM = (Σ mᵢ · **vᵢ**) / M = **P** / M
- **Aceleración**: **a**_CM = (Σ mᵢ · **aᵢ**) / M = **F**_externa_neta / M

### Teorema del centro de masa (FUNDAMENTAL)

Σ **F**_externas = M · **a**_CM

**El CM se mueve como si fuera una partícula con masa total M sobre la que actúan sólo las fuerzas externas.** Las internas no lo afectan.

### Consecuencias prácticas

- Sin fuerzas externas → **v**_CM = constante (Ejs. 9, 11, 16, 19, 21).
- En caída libre / tiro oblicuo → **a**_CM = **g** (aunque el sistema explote, Ej. 26).
- Si las únicas externas son verticales (peso, normal del piso) → la componente horizontal de **v**_CM se conserva (Ej. 18).

### Errores típicos de CM

- **Confundir "CM en reposo" con "todas en reposo"**: las partículas internamente pueden moverse mucho mientras el CM queda quieto (Ejs. 12, 19, 40).
- **Olvidar que la aceleración del CM no depende de las internas**: en la rampa móvil (Ej. 18), la normal entre bloque y rampa es interna → no afecta a_CM_x.

---

## 3. La relación lab — CM (König)

> Esto es lo que más cuesta, prestale tiempo.

### Teorema de König para energía cinética

K_lab = K_CM + (1/2) · M · v_CM²

Donde:

- **K_lab** = energía cinética total medida desde el laboratorio = Σ (1/2) mᵢ vᵢ²
- **K_CM** = energía cinética **interna** = Σ (1/2) mᵢ vᵢ'², con vᵢ' = velocidad de la partícula vista desde el CM
- **(1/2) · M · v_CM²** = energía cinética de traslación del CM

**Interpretación**: la EC total se descompone en "lo que vibra/rota internamente" + "lo que se desplaza como bloque entero".

### Velocidades respecto al CM

**vᵢ'** = **vᵢ** − **v**_CM

(Ejs. 15 y 37 te piden exactamente esto.)

### Teorema de König para momento angular

**L**_O = **L**_CM + **r**_CM × **P**

Donde **L**_CM es el momento angular del sistema **respecto del CM**, calculado con velocidades relativas al CM.

---

## 4. Choques

### Clasificación

| Tipo | ¿Conserva P? | ¿Conserva K? | Coef. restitución e |
|---|---|---|---|
| **Elástico** | Sí | Sí | e = 1 |
| **Inelástico** | Sí | No (parte se disipa) | 0 < e < 1 |
| **Plástico (perf. inelástico)** | Sí | No (máxima pérdida) | e = 0, quedan unidos |

### Coeficiente de restitución (1D)

e = − (v'₂ − v'₁) / (v₂ − v₁) = (velocidad relativa de separación) / (velocidad relativa de aproximación)

### Choque elástico 1D — fórmulas listas (Ejs. 24, 27b)

```
v'₁ = ((m₁ − m₂) · v₁ + 2 · m₂ · v₂) / (m₁ + m₂)
v'₂ = ((m₂ − m₁) · v₂ + 2 · m₁ · v₁) / (m₁ + m₂)
```

Casos límite útiles:

- Si m₁ = m₂ y v₂ = 0 → intercambian velocidades.
- Si m₂ ≫ m₁ y v₂ = 0 → la partícula 1 rebota con v'₁ ≈ −v₁ (como pared).

### Choque plástico 1D (Ejs. 22, 23, 27a, 28)

v_final = (m₁·v₁ + m₂·v₂) / (m₁ + m₂) = v_CM

Después del choque ambas se mueven con la velocidad del CM. Esto es **siempre** así en plásticos.

### Estrategia general para choques

1. **Antes y después**: dibujar dos esquemas con velocidades.
2. **Conservación de P** (vectorial, una ecuación por componente):

   m₁·**v₁** + m₂·**v₂** = m₁·**v'₁** + m₂·**v'₂**

3. **¿Es elástico?** Si sí, agregar la ecuación de K:

   (1/2)·m₁·v₁² + (1/2)·m₂·v₂² = (1/2)·m₁·v'₁² + (1/2)·m₂·v'₂²

4. **¿Es plástico?** Reemplazar v'₁ = v'₂ = v_f.
5. **Resolver el sistema**.

### Trucos para choques 2D (Ejs. 22, 25, 29)

- Una ecuación de conservación **por cada componente** (x e y).
- En choques perpendiculares (Ej. 22 auto-camión): conservás px y py por separado.
- En Ej. 25 (bala rebota a 90°): conviene alinear los ejes con la geometría inicial.

---

## 5. Momento angular (momento cinético)

### Definiciones

- **De una partícula respecto del punto O**:

  **L**_O = **r** × **p** = m · (**r** × **v**)

- **De un sistema respecto de O**:

  **L**_O = Σ mᵢ · (**rᵢ** × **vᵢ**)

**Módulo (caso 2D típico de la guía)**:

|L_O| = m · v · d ,   donde d = distancia perpendicular de la línea de **v** al punto O.

Es decir: sólo importa la componente de **v** perpendicular a **r**.

### Torque (cupla, momento de una fuerza)

**τ**_O = **r** × **F**

### Teorema fundamental (dinámica de rotación)

d**L**_O / dt = Σ **τ**_externos respecto de O

**Si Σ τ_externos = 0 → L_O se conserva.**

### Cuándo conserva L (casos típicos en la guía)

1. **Fuerza central** (siempre dirigida hacia un punto fijo): Tierra–Sol (Ej. 31) — la fuerza gravitatoria pasa siempre por el Sol → τ_Sol = 0 → L_Sol = cte. De ahí salen las leyes de Kepler.
2. **Punto en la línea de la fuerza**: si tomás L respecto al punto de impacto, la fuerza del choque no genera torque (Ej. 35).
3. **Sistema aislado de torques externos**: patinadores con varilla (Ej. 40) — ninguna fuerza horizontal externa → L_CM = cte mientras tiran de la varilla; por eso giran más rápido al acortar el radio.

### Trampa frecuente

El momento angular se calcula **respecto a un punto** (o eje). El mismo movimiento puede tener L distinto respecto a O o respecto al CM. Siempre aclarar el punto de referencia (Ejs. 33, 37, 38 te lo piden explícitamente).

---

## 6. Tabla resumen: qué se conserva cuándo

| Situación | **P** | **L**_O | K | E_mecánica |
|---|---|---|---|---|
| Sistema aislado (sin **F**_ext) | ✅ | ✅ | depende | ✅ si sólo F. conservativas |
| Choque elástico | ✅ | ✅ (resp. punto impacto) | ✅ | ✅ |
| Choque plástico / inelástico | ✅ | ✅ (resp. punto impacto) | ❌ | ❌ |
| Caída libre / tiro oblicuo | ❌ (peso) | ❌ (resp. punto general) | ❌ | ✅ |
| Bloque por rampa móvil (sin roz.) | px ✅, py ❌ | ❌ | depende | ✅ |
| Sistema con rozamiento interno (Ej. 17) | ✅ (si no hay roz. externo) | ✅ | ❌ | ❌ |
| Órbita planetaria (Kepler) | ❌ | ✅ (resp. Sol) | ❌ | ✅ |
| Persona caminando en plataforma | ✅ (si no hay roz. con suelo) | ✅ | ❌ (trabaja energía interna) | ❌ |

> **Regla de oro**: **P** y **L** son magnitudes vectoriales — podés tener una componente que se conserva y otra que no. K es escalar — o se conserva toda o no.

---

## 7. Errores conceptuales típicos

1. **"Como hay gravedad, no se conserva P"** → falso en choques cortos. Lo que importa es si ΔP por la gravedad es comparable con la del choque. En tiempos cortos (ms), no.
2. **"Si se conserva P, se conserva la energía"** → NO. En un plástico se conserva **P** pero se pierde mucha K.
3. **"El CM está donde está la masa más grande"** → no, está en el promedio ponderado.
4. **"Como hay rozamiento, no puedo usar conservación"** → si el rozamiento es **interno** al sistema (bloque sobre carro), P sí se conserva; lo que no se conserva es K.
5. **"Si el sistema explota, el CM se acelera"** → NO. La explosión es interna, no cambia **a**_CM. El CM sigue su trayectoria como si nada (Ej. 26).
6. **Confundir punto de referencia en L**: cambiarlo entre el "antes" y el "después" — siempre usá el mismo punto.
7. **No proyectar antes de igualar**: la conservación de **P** es vectorial. En 2D son **dos** ecuaciones, no una.

---

## 8. Plantilla de resolución

Para cualquier problema, escribí explícitamente:

```
1. SISTEMA: { ... }
2. FUERZAS EXTERNAS sobre el sistema: peso, normal del piso, ...
3. ¿Conserva P?           → Sí / No / Sólo componente x
4. ¿Conserva L (resp. ?)  → ...
5. ¿Conserva E_mec?       → Sí / No  (¿qué disipa?)
6. ECUACIONES (una línea cada una):
   - Conservación de px:   m₁v₁x + m₂v₂x = ...
   - Conservación de py:   ...
   - Conservación de E:    ...  (si aplica)
7. INCÓGNITAS vs ECUACIONES → ¿está determinado?
8. RESOLVER, verificar unidades y signos.
```

Este formato es lo que los profesores de FSP esperan ver. Te ahorra puntos perdidos por "no justificó".

---

## Apéndice: fórmulas de un vistazo

| Concepto | Fórmula |
|---|---|
| Momento lineal (partícula) | **p** = m · **v** |
| Momento lineal (sistema) | **P** = M · **v**_CM |
| Impulso | **J** = ∫ **F** dt = Δ**p** |
| Posición del CM | **r**_CM = (Σ mᵢ **rᵢ**) / M |
| Velocidad del CM | **v**_CM = (Σ mᵢ **vᵢ**) / M |
| Teorema del CM | **F**_ext_neta = M · **a**_CM |
| König (energía) | K_lab = K_CM + (1/2) M v_CM² |
| Velocidad rel. al CM | **vᵢ'** = **vᵢ** − **v**_CM |
| Momento angular | **L**_O = **r** × **p** |
| Módulo (2D) | \|L_O\| = m · v · d (d = distancia perp.) |
| Torque | **τ**_O = **r** × **F** |
| Teorema d**L**/dt | d**L**_O/dt = Σ **τ**_ext |
| Choque elástico 1D | v'₁ = ((m₁−m₂)v₁ + 2m₂v₂)/(m₁+m₂) |
| Choque plástico 1D | v_f = (m₁v₁ + m₂v₂)/(m₁+m₂) |
| Coef. restitución | e = (v'₂ − v'₁) / (v₁ − v₂) |
