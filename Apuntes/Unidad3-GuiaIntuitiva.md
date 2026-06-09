# Cuerpo Rígido desde cero — Guía intuitiva

> Esta guía es el "por qué" y el "cómo lo veo" de la Unidad 3. Si **Unidad3-CuerpoRigido.md** te tira las fórmulas, esta te explica la película antes. Leela en orden, no saltees.

> **Notación**: producto vectorial = **∧** (cuña). Posición de A respecto de B = **r̄_{A→B}** (vector que va de B hacia A). Torque = **τ**.

---

## Índice

0. [El cambio mental](#capitulo-0--el-cambio-mental)
1. [La velocidad angular Ω̄](#capitulo-1--velocidad-angular)
2. [El producto vectorial Ω̄ ∧ r̄ sin trauma](#capitulo-2--producto-vectorial)
3. [La fórmula maestra](#capitulo-3--la-formula-maestra)
4. [El CIR: el truco que lo simplifica todo](#capitulo-4--el-cir)
5. [Rodar sin resbalar (RSR)](#capitulo-5--rsr)
6. [Rigidez: por qué no podés inventar cualquier velocidad](#capitulo-6--rigidez)
7. [Aceleraciones](#capitulo-7--aceleraciones)
8. [Volvamos al Ej. 4 con todo claro](#capitulo-8--ej-4)
9. [Volvamos al Ej. 5 con todo claro](#capitulo-9--ej-5)

---

<a id="capitulo-0--el-cambio-mental"></a>

## Capítulo 0 — El cambio mental

### ¿Qué es un cuerpo rígido?

Antes viste:

- **Partículas** (U1): un punto con masa.
- **Sistemas de partículas** (U2): muchos puntos, cada uno con su velocidad.

Un **cuerpo rígido** (CR) es un sistema de partículas con una sola regla extra: **las distancias entre las partículas no cambian**. Una rueda, una pelota, una varilla, una mesa. NO un slime, NO una soga estirable, NO una nube de humo.

### La gran simplificación

Una rueda tiene millones de partículas. En principio, deberías tener millones de velocidades para describirla. Pero como es rígida, **solo necesitás 2 datos**:

1. **v̄_CM** — velocidad del centro de masa.
2. **Ω̄** — velocidad angular (cuánto gira y para qué lado).

Con esos 2 datos, sabés la velocidad de **cualquier punto** del cuerpo. Esa es la idea central de toda la unidad. Todo lo demás es "cómo calculo cosas con esos dos datos".

> Si en algún momento te perdés, volvé a esta frase: **un CR plano se describe con v̄_CM y Ω̄, y nada más**.

---

<a id="capitulo-1--velocidad-angular"></a>

## Capítulo 1 — La velocidad angular Ω̄ (y por qué es un vector)

### Ω̄ no es solo un número

Cuando algo gira, hay dos cosas que importan: **qué tan rápido** y **para qué lado**. Para meter las dos en un solo objeto matemático, usamos un vector.

- **Módulo de Ω̄** = cuántos radianes barre por segundo (rad/s).
- **Dirección de Ω̄** = a lo largo del eje de rotación.
- **Sentido de Ω̄** = lo da la **regla de la mano derecha**.

### Regla de la mano derecha (en 2D)

Cerrá la mano derecha. Los **dedos** siguen el sentido de la rotación. El **pulgar** apunta en la dirección de Ω̄.

Para una rueda mirada de frente (plano de la hoja):

```
   Antihorario              Horario
   (Ω̄ sale de la hoja)      (Ω̄ entra a la hoja)

       ↑                        ↑
      ╱─╲ ←                  → ╱─╲
     │   │                     │   │
      ╲─╱ →                  ← ╲─╱
       ↓                        ↓

   Ω̄ = +Ω k̂                Ω̄ = −Ω k̂
   "Ω positivo"             "Ω negativo"
```

> **Regla mental rápida**: si gira como las agujas del reloj **mirando la pantalla**, Ω̄ entra a la hoja (negativo). Si gira al revés, sale (positivo).

### Concepto clave

**Ω̄ es la misma para TODOS los puntos del cuerpo**. Si la rueda gira a 10 rad/s, cada partícula de la rueda "rota" a 10 rad/s alrededor del CM. La rueda entera comparte un único Ω̄.

Lo que SÍ cambia entre partículas es su **velocidad lineal**: el borde se mueve más rápido que un punto cerca del centro. Eso lo da el producto vectorial.

---

<a id="capitulo-2--producto-vectorial"></a>

## Capítulo 2 — El producto vectorial Ω̄ ∧ r̄ sin trauma

### ¿Por qué aparece este bicho?

Cuando un cuerpo rota alrededor de un punto, la velocidad lineal de cada partícula depende de **a qué distancia está del eje** y **en qué dirección**. El producto vectorial Ω̄ ∧ r̄ es **la fórmula** que combina esas dos cosas:

  **v̄ = Ω̄ ∧ r̄**

donde **r̄** es la posición de la partícula respecto del eje de rotación.

### Reglas mecánicas de Ω̄ ∧ r̄ en 2D

En 2D, Ω̄ = Ω_z k̂ (sale o entra a la hoja) y **r̄** = (r_x, r_y, 0) (en el plano).

El cálculo es directo:

  **Ω̄ ∧ r̄** = Ω_z k̂ ∧ (r_x î + r_y ĵ)
            = Ω_z r_x (k̂ ∧ î) + Ω_z r_y (k̂ ∧ ĵ)
            = Ω_z r_x ĵ − Ω_z r_y î
            = (−Ω_z · r_y ; Ω_z · r_x)

> **Atajo memorizable**: si Ω̄ = Ω_z k̂ y r̄ = (a, b), entonces **Ω̄ ∧ r̄ = (−Ω_z·b ; Ω_z·a)**.
> Es **rotar (a, b) 90° antihorario** y multiplicar por Ω_z.

### Versores básicos (memorizalos sí o sí)

  î ∧ ĵ = k̂
  ĵ ∧ k̂ = î
  k̂ ∧ î = ĵ

(Ciclo: î → ĵ → k̂ → î. Si vas en orden cíclico, da positivo. Si vas al revés, negativo.)

Y por antisimetría:
  ĵ ∧ î = −k̂, etc.

### Intuición geométrica

**Ω̄ ∧ r̄** te da un vector que es:
- **Perpendicular a r̄** (en 2D, perpendicular en el plano).
- **Módulo** = |Ω̄| · |r̄| (cuando son perpendiculares).
- **Sentido** = el que da la mano derecha.

```
        Ω̄ sale (antihorario)
                
              v̄ = Ω̄ ∧ r̄
              ↑   (perpendicular a r̄,
              │    en el sentido de rotación)
              │
       ●──────●  ← partícula en r̄
       eje
```

Si me decís "el cuerpo gira con Ω̄ antihorario, y este punto está a distancia r a la derecha del eje", **automáticamente** sabés que la velocidad apunta hacia arriba.

---

<a id="capitulo-3--la-formula-maestra"></a>

## Capítulo 3 — La fórmula maestra

### Cómo combinar traslación + rotación

Un cuerpo que rota Y se traslada (rototraslación, lo más general en 2D) tiene cualquier punto P con velocidad:

  **v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}**

Donde:
- **v̄_CM**: traslación pura (lo que tendría P si el cuerpo no rotara).
- **Ω̄ ∧ r̄_{P→CM}**: lo que aporta la rotación, con r̄_{P→CM} = vector que va **del CM al punto P** (posición de P medida desde el CM).

### Por qué funciona (idea intuitiva)

Imaginate que el CM "lleva al cuerpo de paseo" con velocidad v̄_CM. Si el cuerpo solo trasladara (sin rotar), todo punto tendría velocidad v̄_CM. Eso es la parte fácil.

Pero además el cuerpo rota alrededor del CM con velocidad angular Ω̄. Esa rotación le agrega a cada partícula una velocidad **adicional** Ω̄ ∧ r̄_{P→CM} (igual que en rotación pura, pero medido desde el CM).

**Suma las dos**: traslación + rotación = velocidad total del punto P. Eso es la fórmula maestra.

```
                    ↑ (Ω̄ ∧ r̄_{P→CM}): aporte de la rotación
                    │
                    │
         CM ────→ P ─────→  velocidad final v̄_P
              v̄_CM
              (aporte de la traslación,
               igual para todos los puntos)
```

### En coordenadas

Si **v̄_CM** = (v_x, v_y), Ω̄ = Ω_z k̂, y r̄_{P→CM} = (a, b):

  **v̄_P** = (v_x − Ω_z · b ; v_y + Ω_z · a)

Es la suma componente a componente. **Eso es todo el cálculo de cinemática del CR**.

---

<a id="capitulo-4--el-cir"></a>

## Capítulo 4 — El CIR: el truco que lo simplifica todo

### Definición

El **Centro Instantáneo de Rotación (CIR)** es **el único punto del cuerpo (real o imaginario) cuya velocidad en ese instante es CERO**.

Sí, leíste bien: aunque todo el cuerpo se esté moviendo, hay un punto cuya velocidad instantánea es nula.

### ¿Por qué existe ese punto?

Pensá una rueda de auto andando. El centro va a velocidad v̄. El punto de arriba va al doble (2v̄). El punto que toca el piso... como la rueda no resbala, ese punto **no se mueve respecto del piso en ese instante**. Su velocidad es cero. **Ese es el CIR**.

```
            ↑ v̄_top = 2v̄
            ●
           ╱╲
          ╱  ╲
         ●----●  ← centro: v̄
          ╲  ╱
           ╲╱
            ●  ← contacto: v̄ = 0 (CIR)
         ───────
```

### ¿Por qué es tan útil?

Si conocés el CIR, el cuerpo entero se comporta como si **estuviera rotando puramente alrededor del CIR** en ese instante. Y la rotación pura es **mucho más fácil** que la rototraslación:

  **v̄_punto = Ω̄ ∧ r̄_{punto→CIR}**

Sin término de traslación. Directo.

Esto te ahorra el lío de calcular la fórmula maestra para cada punto. Si encontrás el CIR, calculás todas las velocidades como si fuera una rueda alrededor de un eje fijo.

### Cómo encontrar el CIR — 3 métodos

#### Método 1 — Gráfico (conocés v̄ en dos puntos)

**La velocidad de un punto es siempre perpendicular al segmento que va del CIR a ese punto** (porque está rotando alrededor del CIR).

→ Trazá la perpendicular a v̄_A pasando por A.
→ Trazá la perpendicular a v̄_B pasando por B.
→ **Donde se cortan, está el CIR.**

```
                v̄_A
                ↑
                │
                A ───────┐
                         │ (perpendicular a v̄_A)
                         │
                         ●  ← CIR
                         │
                B ───────┘ (perpendicular a v̄_B)
                ↑
                │
                v̄_B
```

#### Método 2 — Si rueda sin resbalar (RSR)

El CIR está en el **punto de contacto** con la superficie.

#### Método 3 — Analítico (conocés v̄_CM y Ω̄)

  Distancia CM a CIR: **d = |v̄_CM| / |Ω̄|**
  Dirección: perpendicular a v̄_CM, del lado tal que rotando alrededor del CIR reproduzca v̄_CM.

### CIR vs punto material

El CIR **NO es un punto fijo del cuerpo**. Cambia en cada instante. Es un concepto matemático ("el punto que en este instante tiene v̄ = 0"), no una partícula que estés siguiendo.

> Ejemplo: en una rueda RSR, el CIR es siempre el punto de contacto. Pero **el punto de contacto cambia** todo el tiempo (es una partícula distinta de la rueda en cada instante).

---

<a id="capitulo-5--rsr"></a>

## Capítulo 5 — Rodar sin resbalar (RSR)

### El concepto

Una rueda **rueda sin resbalar** (RSR) si el punto de contacto con el piso **no desliza** respecto del piso. Es decir, en cada instante, **v̄_contacto = 0**.

Eso implica que el CIR está en el contacto.

### La relación fundamental

Con CIR en el contacto y rotando con Ω̄, el CM está a distancia R del CIR. Entonces:

  **|v̄_CM| = |Ω̄| · R**          (en módulo)

Si derivás en el tiempo:

  **|a̅_CM| = |α̅| · R**          (en módulo)

Estas son **las dos ecuaciones de vínculo de RSR**. Aparecen en casi todos los problemas de rodadura.

### Cuidado con los signos

En vectores, hay que poner los signos a mano según la geometría. Si la rueda está sobre el piso (eje y hacia arriba, x hacia la derecha):

- CIR (= contacto) está en r̄_{contacto→CM} = (0, −R).
- Para que v̄_contacto = 0, si v̄_CM = v_x î, entonces Ω̄ = −(v_x/R) k̂.

**Si la rueda va a la derecha (v̄_CM > 0), Ω̄ apunta hacia adentro de la hoja (negativo)**. Lo verificás con la mano derecha: dedos rotando como las agujas del reloj → pulgar entra. Cuadra.

### Velocidades de los 4 puntos clave (en RSR)

Para una rueda RSR de radio R con CM moviéndose a v̄_CM:

```
                  ↑ v̄_D = 2·v̄_CM (horizontal)
                  D
                ╱ │ ╲
               ╱  │  ╲
              ●   ●   ●
             A│   CM  B↘
                       v̄_B = v_CM·√2 (45° abajo-derecha)
              ●        
             ↗│       
             v̄_A = v_CM·√2 (45° arriba-derecha) 
              C
              ●  ← v̄_C = 0 (CIR)
           ════════════ piso
```

Reglas para memorizar:
- **Top**: el doble del CM.
- **Contacto**: cero.
- **Lados**: √2 veces el CM, a 45°.

> **Por qué √2 a 45°**: el punto del costado está a distancia √2·R del CIR (Pitágoras: R hacia arriba + R hacia el costado). Y como rota alrededor del CIR, |v̄| = Ω · √2·R = √2 · v_CM. La dirección sale perpendicular al segmento CIR→punto, que está a 45°.

### El gran resultado: rozamiento estático en RSR NO disipa

En RSR, el rozamiento es **estático** (no dinámico, porque no hay deslizamiento). Y el rozamiento estático actúa **en el punto de contacto, que tiene v̄ = 0**. Trabajo = fuerza × velocidad = fuerza × 0 = **0**.

> Esto es contraintuitivo: aunque hay rozamiento (y de hecho es el que hace que la rueda ruede), **no le quita energía**. Toda la energía se conserva.

Cuando hagas energía, recordá: RSR → conservación de E_mec. Sin RSR (rueda deslizando) → el rozamiento dinámico SÍ disipa.

---

<a id="capitulo-6--rigidez"></a>

## Capítulo 6 — Rigidez: por qué no podés inventar cualquier velocidad

### El problema

Imaginate que te doy dos puntos A y B de un "supuesto" cuerpo rígido, con velocidades v̄_A y v̄_B inventadas. ¿Eso siempre puede ser un cuerpo rígido? **No**.

Si A y B están a distancia fija (rígido), no pueden alejarse ni acercarse. Si vos les das velocidades arbitrarias, **es posible que el cuerpo se "estire" o "comprima"** entre A y B, lo cual viola rigidez.

### La condición de rigidez

Las velocidades de dos puntos A y B de un CR cumplen:

  **v̄_A · û_{A→B} = v̄_B · û_{A→B}**

Donde û_{A→B} es el versor que va de A a B.

**Traducción**: la **proyección** de v̄_A y v̄_B sobre la línea que los une debe ser **igual**.

### Por qué

Si v̄_A y v̄_B tuvieran proyecciones distintas sobre AB, eso significa que A se mueve "hacia B" más rápido (o más lento) de lo que B se mueve "alejándose de A". Eso comprime o estira el segmento AB. ¡Eso no es rígido!

```
   Caso rígido: las proyecciones sobre AB son iguales

          v̄_A
          ↘
           A ─────────→─────────── B
                                   ↘  v̄_B
                                   
          proyección v̄_A sobre AB = proyección v̄_B sobre AB ✓


   Caso NO rígido: A se acerca a B (o B se aleja de A)

          v̄_A
          ↗
           A ─────────→─────────── B
                                   ↗  v̄_B
                                   
          A "persigue" a B → distancia disminuye → NO rígido
```

### Cómo se usa en problemas

Cuando te dan dos velocidades sin Ω̄, podés:
1. **Verificar rigidez** (que la condición se cumpla).
2. **Usarla como una ecuación más** para despejar incógnitas.

En el Ej. 4 lo usaste para verificar que los datos eran consistentes con un CR.

---

<a id="capitulo-7--aceleraciones"></a>

## Capítulo 7 — Aceleraciones

### La fórmula maestra para a̅

Si derivás en el tiempo la fórmula maestra de v̄, te queda:

  **a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω² · r̄_{P→CM}**

Tres términos:
1. **a̅_CM**: aceleración del CM (cuánto se acelera el cuerpo en su conjunto).
2. **α̅ ∧ r̄_{P→CM}**: aceleración **tangencial** (debida a que Ω̄ está cambiando). α̅ = dΩ̄/dt.
3. **−Ω² · r̄_{P→CM}**: aceleración **centrípeta** (apunta hacia el CM, porque P "orbita" alrededor del CM).

### Por qué hay un Ω² (centrípeta)

Aunque Ω̄ fuera constante, un punto que rota describe un círculo y necesita aceleración centrípeta para mantenerlo. **Esa aceleración apunta al centro de la rotación** (el CM, en este caso) y tiene módulo Ω²·r.

Es el mismo Ω²·r que viste para movimiento circular en U1, solo que ahora respecto del CM.

### El CIR tiene a̅ ≠ 0

Cuidado: **v̄_CIR = 0 NO significa que a̅_CIR = 0**. El CIR es el "punto que justo en ese instante está quieto", pero **un instante después ya no es el mismo punto** (porque el CIR se mueve a otro lugar). El punto material que era el CIR sí se acelera.

Para el caso típico de RSR, el contacto tiene:

  **|a̅_contacto| = Ω² · R** apuntando hacia el CM (puramente centrípeta).

(Los términos tangenciales se cancelan exactamente con a̅_CM, lo viste en el ejercicio 5.)

---

<a id="capitulo-8--ej-4"></a>

## Capítulo 8 — Volvamos al Ej. 4 con todo claro

### Lo que te daban

Un cilindro de R = 0,3 m. En cierto instante:
- v̄_CM = −10 ĵ m/s (CM bajando)
- v̄_P = 20 m/s en la dirección de la figura, con α = 60° desde el eje y (P arriba del CM)

### Lo que te pedían

(a) Tipo de movimiento + rigidez. (b) CIR gráfico. (c) CIR analítico.

### El plan de ataque (lo que harías ahora con todo claro)

**Paso 1: armar las velocidades en coordenadas**

v̄_CM = (0; −10) m/s (puramente hacia abajo).

v̄_P = 20 m/s, a 60° desde el eje +y, inclinada hacia abajo-derecha:
  v̄_P = (20·sen 60° ; −20·cos 60°) = (10√3 ; −10) m/s.

**Paso 2: rigidez**

P está justo arriba del CM. El versor de CM a P es **ĵ**. Las proyecciones sobre **ĵ**:
- v̄_CM · ĵ = −10
- v̄_P · ĵ = −10

Iguales → **rige rigidez**.

**Paso 3: tipo de movimiento**

v̄_CM ≠ 0 → hay traslación. v̄_P ≠ v̄_CM → hay rotación. **Es rototraslación**.

**Paso 4: CIR gráfico**

- v̄_CM apunta hacia abajo. La perpendicular a v̄_CM por el CM es el **eje x** (horizontal).
- v̄_P apunta abajo-derecha a 30° del eje x. La perpendicular a v̄_P por P sube-baja perpendicular a esa dirección.
- Donde se cortan, está el CIR. Por inspección: sobre el eje x, **a la izquierda del CM**.

**Paso 5: CIR analítico**

Calculás Ω̄ usando v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM} con r̄_{P→CM} = (0, R):

Ω k̂ ∧ R ĵ = Ω·R·(k̂ ∧ ĵ) = −Ω·R î

(10√3 ; −10) = (0; −10) + (−Ω·R ; 0)
Componente x: 10√3 = −Ω·0,3 → Ω = −10√3/0,3 = −100√3/3 ≈ −57,74 rad/s.

(Negativo = horario, entra a la hoja.)

CIR: punto donde v̄ = 0. Ponés r̄_{CIR→CM} = (x, y), v̄ = 0:

0 = v̄_CM + Ω̄ ∧ r̄_{CIR→CM}
0 = (0; −10) + (−Ω·y ; Ω·x)

x: −Ω·y = 0 → y = 0
y: −10 + Ω·x = 0 → x = 10/Ω = −√3/10 ≈ −0,173 m

CIR a (−0,173; 0) m. **Coincide con la inspección gráfica**: sobre el eje x, a la izquierda del CM, dentro del cuerpo (porque |x| < R).

### Lección del ejercicio

El truco era darse cuenta de que **rigidez es una restricción REAL** sobre los datos. La condición v̄_P · ĵ = v̄_CM · ĵ es lo que une los dos datos, y de ahí salen todas las demás cuentas.

---

<a id="capitulo-9--ej-5"></a>

## Capítulo 9 — Volvamos al Ej. 5 con todo claro

### Lo que te daban

Un disco de R = 0,1 m **rodando sin resbalar** en el piso. Puntos A (izq), B (der), C (contacto), D (top). Datos:
- v̄_A · î = 1 m/s
- α̅ = −20 k̂ rad/s² (acelera angularmente, horario)

### El plan de ataque

**Paso 1: explotar RSR para encontrar v̄_CM y Ω̄**

Como RSR, **CIR = C (contacto)**. Eso es lo más potente: si encontrás un dato (v̄_A), podés sacar Ω̄ directo viendo distancia A−CIR.

Pero el método más mecánico es:

- r̄_{A→CM} = (−R, 0). Aplicás v̄_A = v̄_CM + Ω̄ ∧ r̄_{A→CM}:
  Ω k̂ ∧ (−R î) = −Ω·R (k̂ ∧ î) = −Ω·R ĵ
  v̄_A = (v_CM_x; 0) + (0; −Ω·R) = (v_CM_x; −Ω·R)
  
- v_A_x = v_CM_x → **v_CM_x = 1 m/s**.

- Por RSR (CIR en C, a (0, −R) del CM): v̄_C = 0 = v̄_CM + Ω̄ ∧ (0, −R) = (v_CM_x + Ω·R; 0)
  → Ω = −v_CM_x / R = −10 rad/s.

→ Ω̄ = −10 k̂ rad/s (horario, coherente con disco rodando a la derecha).

**Paso 2: calcular velocidades de los puntos**

Usando v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}, con el atajo Ω̄ ∧ (a, b) = (−Ω_z·b ; Ω_z·a) = (10·b ; −10·a):

| Punto | r̄/CM | Ω̄ ∧ r̄ | v̄ = v̄_CM + Ω̄ ∧ r̄ |
|---|---|---|---|
| A | (−R, 0) | (0, 1) | (1, 1) m/s |
| B | (R, 0) | (0, −1) | (1, −1) m/s |
| C | (0, −R) | (−1, 0) | (0, 0) m/s ✓ |
| D | (0, R) | (1, 0) | (2, 0) m/s |
| CM | (0, 0) | (0, 0) | (1, 0) m/s |

Reconocés los patrones:
- D al doble (= 2 m/s) ✓
- A y B a √2 (módulo √2 ≈ 1,41) ✓
- C en cero ✓ (CIR)

**Paso 3: calcular a̅_CM**

Por RSR derivado: |a̅_CM| = |α̅| · R en módulo, signo opuesto. Más cuidadoso:

a_C en x = 0 (RSR derivada): a_CM_x + α_z · R = 0 → a_CM_x = −α_z·R = −(−20)·0,1 = **2 m/s²**.

a̅_CM = (2, 0) m/s².

**Paso 4: aceleraciones de los puntos**

Fórmula: a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω² · r̄_{P→CM}.

Con α_z = −20 y Ω² = 100:
- α̅ ∧ (a, b) = (−α_z·b ; α_z·a) = (20·b ; −20·a)
- −Ω²·(a, b) = (−100a ; −100b)

| Punto | r̄/CM | α̅ ∧ r̄ | −Ω²·r̄ | a̅ = suma de los tres |
|---|---|---|---|---|
| A | (−R, 0) | (0, 2) | (10, 0) | (12, 2) m/s² |
| B | (R, 0) | (0, −2) | (−10, 0) | (−8, −2) m/s² |
| C | (0, −R) | (−2, 0) | (0, 10) | (0, 10) m/s² |
| D | (0, R) | (2, 0) | (0, −10) | (4, −10) m/s² |
| CM | (0, 0) | (0, 0) | (0, 0) | (2, 0) m/s² |

**Observación clave**: a̅_C = (0, 10) m/s². No es cero, es puramente centrípeta hacia el CM (apunta hacia arriba, hacia el centro del disco). Es Ω²·R = 100·0,1 = 10. Cuadra.

### Lección del ejercicio

En RSR, el CIR está en el contacto y eso te da **|v̄_CM| = |Ω̄|·R** y **|a̅_CM| = |α̅|·R**. Esas dos relaciones bajan dramáticamente la dificultad: una vez que las usás, todo es aplicar la fórmula maestra con valores conocidos.

---

## Checklist mental para problemas de cinemática del CR

Cada vez que abrís un problema de cuerpo rígido, hacete estas preguntas en orden:

1. **¿Qué tipo de movimiento?** Traslación pura / rotación pura / rototraslación.
2. **¿Conozco v̄_CM y Ω̄?** Si sí, puedo calcular cualquier punto con la fórmula maestra.
3. **¿Hay vínculos?** RSR (|v̄_CM| = |Ω̄|·R), pivote fijo (CIR ahí), etc.
4. **¿Me sirve el CIR?** Si conozco v̄ en dos puntos no paralelas, sí. Si rueda sin resbalar, está en el contacto.
5. **¿Me piden aceleraciones?** Usá la otra fórmula maestra con tres términos: a̅_CM + α̅ ∧ r̄ − Ω²·r̄.

> Tip: si te sentís perdido, dibujá. Hace un esquema con los datos, marcá vectores con flechitas, marcá el CIR si lo encontrás. La mitad de los problemas se resuelven con un buen dibujo.

---

## Resumen ultra-comprimido (la guía dentro de la guía)

| Cosa | Fórmula | Cuándo |
|---|---|---|
| Velocidad de cualquier P | **v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}** | Siempre |
| Aceleración de cualquier P | **a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω² · r̄_{P→CM}** | Siempre |
| Si conozco CIR | **v̄_P = Ω̄ ∧ r̄_{P→CIR}** | Si encontré el CIR |
| RSR | **|v̄_CM| = |Ω̄| · R** ; **|a̅_CM| = |α̅| · R** (módulos) | Rueda sin resbalar |
| Rigidez | **v̄_A · û_{A→B} = v̄_B · û_{A→B}** | Verificar / ecuación extra |
| CIR (gráfico) | Intersección de perpendiculares a v̄_A y v̄_B | Conozco 2 velocidades |
| Distancia CM-CIR | **d = |v̄_CM| / |Ω̄|** | Conozco v̄_CM y Ω̄ |

Con esto en la cabeza, los próximos ejercicios deberían fluir mucho mejor.
