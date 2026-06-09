# Guía de ejercicios graduados — Unidad 3: Cuerpo Rígido (Cinemática)

> 15 ejercicios de cinemática del CR, ordenados de **muy básico** a intermedio. NO hay todavía dinámica ni energía — eso lo agregamos cuando manejes esto. Las respuestas están al final; intentá resolverlos antes de mirarlas.

**Notación**:
- Vectores con flechita: v̄, r̄, Ω̄, etc.
- Versores: î (eje x), ĵ (eje y), k̂ (eje z, saliendo de la hoja).
- Ω positivo (+k̂) = antihorario. Ω negativo (−k̂) = horario.
- Producto vectorial: **∧** (cuña). Atajo: Ω·k̂ ∧ (a, b) = (−Ω·b, Ω·a).
- Posición de A respecto de B: **r̄_{A→B}** (vector que va de B a A).
- Torque: **τ**.

---

## Resumen del progreso

| # | Tema | Nivel |
|---|---|---|
| 1 | Sentido de Ω̄ (identificación) | 🟢 Muy básico |
| 2 | Velocidad en rotación pura (1 punto) | 🟢 Muy básico |
| 3 | Identificar tipo de movimiento | 🟢 Muy básico |
| 4 | CIR en RSR (identificación) | 🟢 Muy básico |
| 5 | Relación |v̄_CM| = |Ω̄|·R en RSR | 🟢 Muy básico |
| 6 | Velocidades de los 4 puntos cardinales (RSR) | 🟡 Básico |
| 7 | Velocidades de extremos en varilla rotando | 🟡 Básico |
| 8 | Rototraslación: v̄ de un punto dado v̄_CM y Ω̄ | 🟡 Básico |
| 9 | RSR con vector Ω̄: encontrar v̄_CM | 🟡 Básico |
| 10 | v̄ de un punto fuera del eje vertical en RSR | 🟡 Básico |
| 11 | Verificación de la condición de rigidez | 🟠 Intermedio bajo |
| 12 | CIR gráfico de una escalera | 🟠 Intermedio bajo |
| 13 | Encontrar v̄_CM y Ω̄ desde v̄ de un punto (RSR) | 🟠 Intermedio bajo |
| 14 | Aceleración en RSR (caso tangencial + centrípeta) | 🟠 Intermedio bajo |
| 15 | Aceleración angular y v̄_CM en función de t | 🟠 Intermedio bajo |

---

# Nivel 1 — Muy básico (reconocer + 1 cuenta directa)

## Ejercicio 1 — Sentido de Ω̄

Para cada caso, indicar si Ω̄ apunta en **+k̂** (sale de la hoja, antihorario) o en **−k̂** (entra a la hoja, horario):

a) Un disco que gira en sentido **antihorario** visto desde el frente.
b) Una rueda de bicicleta que **avanza hacia la derecha** rodando sin resbalar.
c) Una rueda de auto que **frena yendo hacia la izquierda** (rodando sin resbalar).
d) La hélice de un ventilador de techo vista desde abajo, girando en el mismo sentido que las agujas del reloj.

---

## Ejercicio 2 — Velocidad de un punto en rotación pura

Un volante gira alrededor de un eje fijo perpendicular al volante que pasa por su CM. La velocidad angular es **Ω = 8 rad/s**.

a) ¿Cuál es la velocidad (módulo) de un punto que está a **0,15 m del eje**?
b) ¿Cuál es la velocidad de un punto que está a **0,30 m del eje**?
c) ¿Y la velocidad de un punto **sobre el eje mismo**?

---

## Ejercicio 3 — Identificar tipo de movimiento

Para cada situación, indicar si es **traslación pura**, **rotación pura** o **rototraslación**:

a) Una pelota de fútbol en el aire después de un chute, sin efecto.
b) Un trompo girando sobre su punta en un lugar fijo.
c) Una rueda de bicicleta andando por la calle (sin resbalar).
d) Una caja siendo empujada por el piso (no gira, solo se desliza).
e) Una hoja que cae rotando mientras baja.
f) El minutero de un reloj.

---

## Ejercicio 4 — CIR en RSR (identificación)

Para cada caso, indicar dónde está el **CIR**:

a) Una rueda rodando sin resbalar por el piso.
b) Una varilla que rota alrededor de un pivote fijo en su extremo izquierdo.
c) Un disco rotando alrededor de su CM (eje fijo en el CM).
d) Una caja que solo se traslada (no rota).

---

## Ejercicio 5 — RSR: v̄_CM y Ω̄

Una pelota de R = **20 cm** rueda sin resbalar por un plano horizontal.

a) Si |v̄_CM| = 3 m/s (hacia la derecha), ¿cuánto vale |Ω̄|?
b) ¿En qué dirección apunta Ω̄ (+k̂ o −k̂)?
c) Si en otro instante |Ω̄| = 25 rad/s, ¿cuánto vale |v̄_CM|?

---

# Nivel 2 — Básico (aplicación directa de la fórmula maestra)

## Ejercicio 6 — Los 4 puntos cardinales en RSR

Una rueda de R = **10 cm** rueda sin resbalar con **v̄_CM = 5 î m/s** (hacia la derecha).

Los puntos del disco son:
- **T**: top (arriba, a (0, R) del CM)
- **C**: contacto (abajo, a (0, −R) del CM)
- **D**: lado derecho (a (R, 0) del CM)
- **I**: lado izquierdo (a (−R, 0) del CM)

a) Calcular Ω̄ (vector).
b) Calcular las velocidades **v̄_T, v̄_C, v̄_D, v̄_I** (vectores).
c) ¿Cuál es el módulo de v̄_D? ¿Y a qué ángulo respecto del eje x?

---

## Ejercicio 7 — Varilla rotando alrededor de su CM

Una varilla de longitud **L = 0,8 m** rota en el plano xy alrededor de un eje fijo que pasa por su CM (perpendicular a la varilla). En cierto instante, está alineada con el eje x y rota con **Ω̄ = +6 k̂ rad/s** (antihorario). v̄_CM = 0.

a) ¿Dónde están los dos extremos respecto del CM?
b) Calcular la velocidad de cada extremo (vector).
c) ¿Cuánto vale |v̄| en el punto a **L/4 del CM**?

---

## Ejercicio 8 — Rototraslación de un disco

Un disco se mueve con **v̄_CM = (2, 0) m/s** y **Ω̄ = −4 k̂ rad/s**. Radio R = 0,25 m.

a) Calcular la velocidad del punto **top** (a (0, R) del CM).
b) Calcular la velocidad del punto **contacto** (a (0, −R) del CM).
c) ¿El disco rueda sin resbalar? Justificar viendo v̄_contacto.

---

## Ejercicio 9 — RSR desde Ω̄ vectorial

Una rueda de R = **30 cm** rueda sin resbalar sobre un piso horizontal. Su velocidad angular es **Ω̄ = +5 k̂ rad/s**.

a) ¿En qué sentido se traslada la rueda (derecha o izquierda)?
b) Calcular **v̄_CM** (vector).
c) Calcular la velocidad del punto **top** (vector).

---

## Ejercicio 10 — Velocidad de un punto "diagonal" en RSR

Una rueda de R = **0,5 m** rueda sin resbalar con **v̄_CM = 4 î m/s**.

Calcular la velocidad (vector) del punto **P** ubicado a **r̄_{P→CM} = (R/2, R/2) = (0,25 ; 0,25) m** respecto del CM.

> Pista: este punto está en el primer cuadrante respecto del CM, a 45° hacia arriba-derecha del CM.

---

# Nivel 3 — Intermedio bajo (combinar dos conceptos)

## Ejercicio 11 — Verificar rigidez

Dos puntos de un cuerpo (supuestamente rígido):
- A en (0, 2) m, con v̄_A = (3, 1) m/s.
- B en (4, 2) m, con v̄_B = (3, −5) m/s.

a) ¿Cuál es el versor û_{A→B} (de A hacia B)?
b) Calcular v̄_A · û_{A→B} y v̄_B · û_{A→B}.
c) ¿Los datos son compatibles con un cuerpo rígido?

---

## Ejercicio 12 — CIR de una escalera

Una escalera de longitud **L = 3 m** está apoyada en el piso y en una pared (ver figura mental: pared vertical, piso horizontal). El ángulo entre la escalera y el **piso** es **θ = 60°**. El extremo superior A se desliza hacia abajo por la pared con **v̄_A = −1 ĵ m/s**.

Posiciones (origen en la esquina pared-piso):
- A = (0, L sen θ) = (0, ?)
- B = (L cos θ, 0) = (?, 0)

a) Calcular las posiciones de A y B en metros.
b) ¿En qué dirección se mueve A? ¿Y B?
c) Encontrar el **CIR** (intersección de perpendiculares).
d) Calcular Ω̄.
e) Calcular **v̄_B** (vector).

---

## Ejercicio 13 — Encontrar v̄_CM y Ω̄ en RSR desde un punto

Un disco rueda sin resbalar. El **punto del lado derecho** del disco (a (R, 0) del CM) tiene velocidad **v̄_D = (2, −2) m/s**. Radio R = **0,2 m**.

a) Calcular v̄_CM (vector).
b) Calcular Ω̄ (vector).
c) ¿Hacia dónde se traslada el disco?

> Pista: usar la fórmula v̄_D = v̄_CM + Ω̄ ∧ r̄_{D→CM}, y además que el contacto (CIR) tiene v̄ = 0.

---

## Ejercicio 14 — Aceleración del contacto en RSR

Una rueda de **R = 0,1 m** rueda sin resbalar con **Ω̄ = −10 k̂ rad/s** y **α̅ = −20 k̂ rad/s²** (acelerándose).

a) Calcular a̅_CM (módulo y dirección).
b) Calcular **a̅_contacto** (vector) usando la fórmula a̅_P = a̅_CM + α̅ ∧ r̄_{P→CM} − Ω²·r̄_{P→CM}.
c) ¿Es a̅_contacto = 0? ¿Hacia dónde apunta? ¿Cuánto vale su módulo?

---

## Ejercicio 15 — Disco RSR desde el reposo

Una pelota con **R = 5 cm** parte del reposo y comienza a acelerarse angularmente con **α̅ = +8 k̂ rad/s²** (constante).

a) ¿En qué dirección se acelera el CM (+x o −x)?
b) Calcular la magnitud de **a̅_CM**.
c) ¿Cuánto vale **|Ω̄|** después de t = 3 s?
d) ¿Cuánto vale **|v̄_CM|** en t = 3 s? (Verificar con dos métodos: usando |a̅_CM|·t y usando |Ω̄|·R).

---

# Respuestas

## Nivel 1

**Ej. 1**
a) **+k̂** (antihorario → sale).
b) **−k̂** (RSR a la derecha → rotación horaria).
c) **+k̂** (RSR a la izquierda → rotación antihoraria).
d) **Depende de la convención** (caso 3D ambiguo):
   - Si tomás **k̂ = arriba en términos absolutos** (eje z vertical hacia arriba): aplicando la regla de la mano derecha desde abajo, los dedos siguiendo el sentido horario que ves, el pulgar apunta hacia ARRIBA (hacia el techo). Entonces **Ω̄ = +k̂**.
   - Si tomás **k̂ = "saliendo de la hoja desde tu perspectiva mirando hacia arriba"** (k̂ apunta hacia tus ojos, o sea hacia abajo físicamente): entonces **Ω̄ = −k̂** desde esa perspectiva.
   - **Lo importante**: Ω̄ apunta físicamente hacia ARRIBA (hacia el techo). El signo en k̂ depende de cómo orientes el eje z.

**Ej. 2**
a) |v̄| = Ω · r = 8 · 0,15 = **1,2 m/s**.
b) |v̄| = 8 · 0,30 = **2,4 m/s**.
c) En el eje mismo, r = 0, entonces |v̄| = **0 m/s** (el eje es un punto fijo).

**Ej. 3**
a) **Traslación pura** (sin rotación).
b) **Rotación pura** (eje fijo, CM puede no moverse).
c) **Rototraslación** (RSR).
d) **Traslación pura**.
e) **Rototraslación**.
f) **Rotación pura** (eje fijo en el centro del reloj).

**Ej. 4**
a) **En el contacto** con el piso.
b) **En el pivote** (extremo izquierdo).
c) **En el CM** (el CM no se mueve si es el eje fijo).
d) **No existe en sentido finito** (está "en el infinito" — es traslación pura, Ω̄ = 0).

**Ej. 5**
a) |Ω̄| = |v̄_CM|/R = 3/0,20 = **15 rad/s**.
b) Como v̄_CM va a la derecha (+x) y RSR → **Ω̄ en −k̂** (horario).
c) |v̄_CM| = |Ω̄| · R = 25 · 0,20 = **5 m/s**.

---

## Nivel 2

**Ej. 6**
a) Ω̄ = −|v̄_CM|/R k̂ = −(5/0,1) k̂ = **−50 k̂ rad/s** (horario, entra a la hoja).

b) Usando v̄_P = v̄_CM + Ω̄ ∧ r̄_{P→CM}, con el atajo Ω·k̂ ∧ (a, b) = (−Ω·b, Ω·a) y Ω_z = −50:

- T: r̄ = (0, 0,1). Ω̄ ∧ r̄ = (−(−50)·0,1, (−50)·0) = (5, 0). **v̄_T = (5+5, 0) = (10, 0) m/s**.
- C: r̄ = (0, −0,1). Ω̄ ∧ r̄ = (−(−50)·(−0,1), 0) = (−5, 0). **v̄_C = (5−5, 0) = (0, 0) m/s** ✓ (CIR).
- D: r̄ = (0,1, 0). Ω̄ ∧ r̄ = (0, −50·0,1) = (0, −5). **v̄_D = (5, −5) m/s**.
- I: r̄ = (−0,1, 0). Ω̄ ∧ r̄ = (0, −50·(−0,1)) = (0, 5). **v̄_I = (5, 5) m/s**.

c) |v̄_D| = √(25+25) = **5√2 ≈ 7,07 m/s**. Ángulo: arctan(−5/5) = **−45°** (45° por debajo de la horizontal).

**Ej. 7**
a) Extremos en r̄ = (−L/2, 0) = (−0,4, 0) m y r̄ = (L/2, 0) = (0,4, 0) m.

b) Con Ω_z = +6 y atajo (−Ω·b, Ω·a):
- Extremo izquierdo (r̄ = (−0,4, 0)): v̄ = (0, 6·(−0,4)) = **(0, −2,4) m/s**.
- Extremo derecho (r̄ = (0,4, 0)): v̄ = (0, 6·0,4) = **(0, 2,4) m/s**.

c) Punto a L/4 = 0,2 m del CM (digamos hacia la derecha): r̄ = (0,2, 0). v̄ = (0, 6·0,2) = **(0, 1,2) m/s**. Módulo = **1,2 m/s**.

**Ej. 8**
a) T: r̄ = (0, 0,25). Ω̄ ∧ r̄ = (−(−4)·0,25, 0) = (1, 0). **v̄_T = (2+1, 0) = (3, 0) m/s**.

b) C: r̄ = (0, −0,25). Ω̄ ∧ r̄ = (−(−4)·(−0,25), 0) = (−1, 0). **v̄_C = (2−1, 0) = (1, 0) m/s**.

c) v̄_contacto ≠ 0 → **NO rueda sin resbalar**. El contacto se desliza hacia la derecha a 1 m/s. Sería RSR si |v̄_CM| = |Ω̄|·R = 4·0,25 = 1 m/s, pero |v̄_CM| = 2 m/s. Acá |v̄_CM| > |Ω̄|·R, así que el disco "patina" hacia adelante.

**Ej. 9**
a) Ω̄ en +k̂ (antihorario) y RSR → v̄_CM hacia la **izquierda** (−x).
b) |v̄_CM| = |Ω̄| · R = 5 · 0,3 = 1,5 m/s, en −x. **v̄_CM = (−1,5; 0) m/s**.
c) T: r̄ = (0, 0,3). Ω̄ ∧ r̄ = (−5·0,3, 0) = (−1,5, 0). **v̄_T = (−1,5−1,5; 0) = (−3; 0) m/s** (el doble del CM, ✓).

**Ej. 10**
Ω̄ = −|v̄_CM|/R k̂ = −4/0,5 k̂ = −8 k̂ rad/s.
r̄_{P→CM} = (0,25; 0,25).
Ω̄ ∧ r̄ = (−(−8)·0,25 ; −8·0,25) = (2, −2).
**v̄_P = (4+2, 0−2) = (6, −2) m/s**. |v̄_P| = √(36+4) = √40 ≈ **6,32 m/s**.

---

## Nivel 3

**Ej. 11**
a) û_{A→B} = (B − A)/|B − A| = (4, 0)/4 = **(1, 0) = î**.
b) v̄_A · û_{A→B} = (3, 1) · (1, 0) = **3**. v̄_B · û_{A→B} = (3, −5) · (1, 0) = **3**.
c) **Sí, son compatibles con CR**. Las proyecciones sobre AB son iguales (= 3 m/s).

**Ej. 12**
a) A = (0, 3·sen 60°) = (0, 3·√3/2) ≈ **(0; 2,60) m**. B = (3·cos 60°, 0) = **(1,5; 0) m**.
b) A se mueve **vertical hacia abajo**. B se mueve **horizontal hacia la derecha** (saliendo de la pared).
c) Perpendicular a v̄_A (vertical) en A: línea horizontal por A → y = 2,60. Perpendicular a v̄_B (horizontal) en B: línea vertical por B → x = 1,5. **CIR = (1,5; 2,60) m**.
d) d_{A→CIR} = 1,5 (horizontal). |v̄_A| = 1, entonces |Ω̄| = |v̄_A|/d_{A→CIR} = 1/1,5 = **2/3 rad/s ≈ 0,67 rad/s**. Sentido: A baja, B sale → **antihorario → Ω̄ = +2/3 k̂ rad/s**.
e) r̄_{B→CIR} = B − CIR = (0, −2,60). v̄_B = Ω k̂ ∧ (0, −2,60) = (2,60·2/3, 0) ≈ **(1,73; 0) m/s** (horizontal saliendo).

**Ej. 13**
a) Sea v̄_CM = (v_x, v_y) y Ω̄ = Ω_z k̂. Como RSR, contacto C en r̄ = (0, −R) tiene v̄ = 0:
  0 = v̄_CM + Ω̄ ∧ (0, −R) = (v_x + Ω·R, v_y) → v_y = 0 y v_x = −Ω·R.
Aplicamos al punto D en r̄ = (R, 0):
  v̄_D = v̄_CM + Ω̄ ∧ (R, 0) = (v_x, Ω·R) = (−Ω·R, Ω·R) = (2, −2).
De Ω·R = −2 → Ω = −2/0,2 = −10. Y v_x = −(−10)(0,2) = 2.
  **v̄_CM = (2, 0) m/s**.
b) **Ω̄ = −10 k̂ rad/s** (horario).
c) El CM se traslada **hacia la derecha** (+x).

**Ej. 14**
a) En RSR, a_CM_x = −α_z · R = −(−20)·0,1 = **+2 m/s²**. Dirección: **+x**. Módulo: 2 m/s².

b) a̅_C = a̅_CM + α̅ ∧ r̄_{C→CM} − Ω²·r̄_{C→CM}. r̄_{C→CM} = (0, −R) = (0, −0,1).
  α̅ ∧ r̄_{C→CM}: atajo α·k̂ ∧ (a, b) = (−α·b, α·a). Con α_z = −20 y (a, b) = (0, −0,1): (−(−20)·(−0,1), (−20)·0) = (−2, 0).
  −Ω²·r̄_{C→CM} = −100·(0, −0,1) = (0, 10).
  **a̅_C = (2, 0) + (−2, 0) + (0, 10) = (0, 10) m/s²**.

c) **NO es cero**. Apunta puramente en **+ĵ** (hacia arriba, hacia el CM). Módulo = **10 m/s²** = Ω²·R = 100·0,1.

> Lección: aunque v̄_C = 0 (es el CIR), a̅_C ≠ 0. Es puramente centrípeta hacia el CM.

**Ej. 15**
a) α̅ en **+k̂** (antihorario). Por RSR yendo en sentido coherente → v̄_CM (y a̅_CM) van en **−x**.
b) |a̅_CM| = |α̅|·R = 8·0,05 = **0,4 m/s²**.
c) Parte del reposo (Ω̄₀ = 0). Ω̄(t) = α̅·t → |Ω̄| = 8·3 = **24 rad/s**.
d) Método 1: |v̄_CM| = |a̅_CM|·t = 0,4·3 = **1,2 m/s**. Método 2: |v̄_CM| = |Ω̄|·R = 24·0,05 = **1,2 m/s** ✓.

---

# Cómo usar esta guía

1. **Resolvé los ejercicios SIN mirar respuestas**. Si te trabás más de 10 min en uno básico, andá a la **Unidad3-GuiaIntuitiva.md** o al **Unidad3-Cheatsheet.md** y volvé.

2. **Después de cada nivel** (5 ejercicios), reflexioná: ¿qué hice bien? ¿en cuál me trabé? Revisá esa parte del cheatsheet antes de seguir.

3. **Si todos los del Nivel 3 los hacés solo**, ya estás listo para encarar los ejercicios reales de la guía (4, 5, 6, etc.).

4. **No avances** al Nivel 2 hasta no tener el Nivel 1 fluido. La trampa típica es saltar y tener "huecos" conceptuales que te hunden después.

5. Si después de hacer todos te seguís sintiendo perdido, **decímelo y armamos más ejercicios o profundizamos los puntos flojos**.
