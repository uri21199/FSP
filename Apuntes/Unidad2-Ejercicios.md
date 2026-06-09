# Guía de ejercicios graduados — Unidad 2: Sistemas de Partículas

> 20 ejercicios ordenados de menor a mayor dificultad. Cubren impulso, cantidad de movimiento, centro de masa, choques (1D y 2D) y momento angular. Las respuestas numéricas están al final; intentá resolverlos antes de mirarlas.

**Notación**: g = 9,8 m/s² salvo aclaración. Cuando un problema dice "sin rozamiento", asumir μ = 0 y normal entre cuerpos lisa.

---

## Resumen del progreso

| # | Tema | Nivel |
|---|---|---|
| 1 | Impulso F constante | 🟢 Básico |
| 2 | Impulso F(t) variable, área bajo curva | 🟢 Básico |
| 3 | Comparar p y K entre dos cuerpos | 🟢 Básico |
| 4 | Posición y velocidad del CM (1D) | 🟢 Básico |
| 5 | Posición y velocidad del CM (2D vectorial) | 🟢 Básico |
| 6 | Choque plástico 1D | 🟡 Intermedio bajo |
| 7 | Choque elástico 1D | 🟡 Intermedio bajo |
| 8 | Persona en balsa — desplazamiento por CM | 🟡 Intermedio bajo |
| 9 | Separación por resorte (explosión 1D) | 🟡 Intermedio bajo |
| 10 | Pelota rebotando — fuerza media | 🟡 Intermedio bajo |
| 11 | Teorema de König (energía) | 🟠 Intermedio |
| 12 | Choque plástico 2D (autos perpendiculares) | 🟠 Intermedio |
| 13 | Péndulo balístico | 🟠 Intermedio |
| 14 | Granada que explota en 3 fragmentos | 🟠 Intermedio |
| 15 | Momento angular de partícula libre | 🟠 Intermedio |
| 16 | Bloque sobre carro con rozamiento | 🔴 Avanzado |
| 17 | Bloque sobre rampa móvil sin rozamiento | 🔴 Avanzado |
| 18 | Bala atraviesa bloque colgante con loop | 🔴 Avanzado |
| 19 | Patinadores con varilla (L y energía) | 🔴 Avanzado |
| 20 | Choque elástico bola–plano inclinado móvil | 🔴 Avanzado |

---

# Nivel 1 — Básico (definiciones directas)

## Ejercicio 1 — Impulso de fuerza constante

Una caja de **3 kg** está en reposo sobre una mesa sin rozamiento. Se le aplica una fuerza horizontal constante de **12 N** durante **4 s**.

a) Calcular el impulso lineal de la fuerza.
b) Hallar la velocidad final de la caja.
c) Si la fuerza se aplica el mismo tiempo pero ahora la caja venía con velocidad inicial de **2 m/s** en sentido **opuesto** a **F**, ¿cuál es su velocidad final?

---

## Ejercicio 2 — Impulso con fuerza variable

Sobre un cuerpo de **2 kg**, inicialmente en reposo sobre una superficie sin rozamiento, se aplica una fuerza horizontal cuya magnitud:
- crece linealmente desde 0 hasta **20 N** entre t = 0 y t = 5 s,
- se mantiene constante en 20 N entre t = 5 s y t = 10 s.

a) Graficar F(t) y calcular el impulso entre 0 y 10 s.
b) Hallar la velocidad del cuerpo en t = 10 s.
c) ¿Cuál es la fuerza media aplicada en el intervalo?

---

## Ejercicio 3 — Mismo p, distinta K

Un ciclista (m₁ = 75 kg) y un auto (m₂ = 1500 kg) tienen igual módulo de cantidad de movimiento. El auto se mueve a **4 m/s**.

a) Calcular la velocidad del ciclista.
b) Hallar la razón K_ciclista / K_auto.
c) Justificar conceptualmente: si tienen el mismo p, ¿por qué uno tiene mucha más energía cinética?

---

## Ejercicio 4 — Centro de masa 1D

Tres masas están alineadas sobre el eje x:
- m₁ = 2 kg en x₁ = 0 m
- m₂ = 3 kg en x₂ = 4 m
- m₃ = 5 kg en x₃ = 10 m

a) Hallar la posición del CM.
b) Si m₁ comienza a moverse con v₁ = 3 m/s î y las otras dos quedan en reposo, calcular **v**_CM.
c) Si las únicas fuerzas que actúan son entre las partículas, ¿a qué velocidad se mueve el CM en cualquier instante posterior?

---

## Ejercicio 5 — Centro de masa 2D

Dos partículas:
- m₁ = 1 kg en **r₁** = (2, 3) m con **v₁** = (0, 2) m/s
- m₂ = 4 kg en **r₂** = (−1, 0) m con **v₂** = (1, 0) m/s

a) Hallar la posición y velocidad del CM.
b) Calcular la cantidad de movimiento del sistema.
c) Si no hay fuerzas externas, ¿dónde estará el CM dentro de 5 s?

---

# Nivel 2 — Intermedio bajo (conservación 1D directa)

## Ejercicio 6 — Choque plástico 1D

Un vagón de **800 kg** se mueve a **5 m/s** hacia la derecha y choca con un vagón de **1200 kg** que avanza en el mismo sentido a **2 m/s**. Tras el choque quedan enganchados.

a) Hallar la velocidad final del conjunto.
b) Calcular la K perdida en el choque.
c) ¿Qué porcentaje de la K inicial se disipó?

---

## Ejercicio 7 — Choque elástico 1D

Una bola de **2 kg** viaja a **6 m/s** y choca elásticamente de frente con otra bola de **4 kg** en reposo.

a) Hallar las velocidades finales de ambas bolas.
b) Verificar la conservación de K.
c) ¿Qué pasaría si las masas fueran iguales (m₁ = m₂ = 2 kg)?

---

## Ejercicio 8 — Persona en balsa

Una persona de **60 kg** está parada en un extremo de una balsa de **240 kg** y **6 m** de largo. Ambas están en reposo sobre agua sin rozamiento. La persona camina hasta el otro extremo de la balsa.

a) ¿Cuánto se desplaza la balsa respecto al agua?
b) ¿Cuánto se desplaza la persona respecto al agua?
c) Justificar por qué el CM del sistema no se mueve.

---

## Ejercicio 9 — Separación por resorte

Dos carritos de **1 kg** y **3 kg** están en reposo sobre una pista horizontal sin rozamiento, con un resorte comprimido entre ellos (sujeto por una cuerda). Se corta la cuerda y los carritos se separan.

a) Si el carrito de 1 kg sale con **6 m/s** hacia la izquierda, ¿cuál es la velocidad del carrito de 3 kg?
b) ¿Cuánta energía estaba almacenada en el resorte?
c) Si el resorte tiene k = 1500 N/m, ¿cuánto estaba comprimido?

---

## Ejercicio 10 — Pelota rebotando

Una pelota de **0,5 kg** cae verticalmente y golpea el piso con rapidez **8 m/s**. Rebota con rapidez **6 m/s** hacia arriba. El tiempo de contacto es **10 ms**.

a) Calcular el impulso del piso sobre la pelota durante el contacto.
b) Hallar la fuerza media del piso sobre la pelota.
c) Comparar con el impulso del peso durante el contacto. ¿Es despreciable?
d) ¿El choque es elástico?

---

# Nivel 3 — Intermedio (König, 2D, péndulo balístico)

## Ejercicio 11 — Teorema de König

Dos partículas de **2 kg** y **3 kg** se mueven sobre el eje x con velocidades **v₁** = 5 m/s î y **v₂** = −3 m/s î.

a) Calcular **v**_CM.
b) Hallar K_lab (energía cinética desde el laboratorio).
c) Hallar las velocidades respecto al CM (**v₁'** y **v₂'**) y calcular K_CM.
d) Verificar que K_lab = K_CM + (1/2)·M·v_CM².

---

## Ejercicio 12 — Choque 2D plástico

Un auto de **1000 kg** viaja al **este** a **20 m/s** y choca contra un camión de **2000 kg** que viaja al **norte** a **15 m/s** por una calle perpendicular. Tras el choque quedan enganchados (asumir piso sin rozamiento durante el choque).

a) Hallar el vector velocidad final del conjunto (módulo y dirección).
b) Calcular la K perdida en el choque.
c) ¿Qué porcentaje de la K inicial se disipa?

---

## Ejercicio 13 — Péndulo balístico

Una bala de **20 g** se dispara horizontalmente contra un bloque de **4 kg** que cuelga en reposo de una cuerda ideal de **1,5 m**. La bala se incrusta y el conjunto sube hasta una altura **h = 0,12 m**.

a) Hallar la velocidad del conjunto bala + bloque inmediatamente después del impacto.
b) Calcular la velocidad inicial de la bala.
c) ¿Qué porcentaje de la K original de la bala se conserva como K del conjunto justo después del choque?

---

## Ejercicio 14 — Granada que explota

Una granada de **6 kg** vuela horizontalmente con velocidad **(10, 0) m/s** cuando explota en tres fragmentos:
- A (1 kg) sale con velocidad **(15, 8) m/s**
- B (2 kg) sale con velocidad **(4, −12) m/s**
- C (3 kg): ¿?

a) Hallar la velocidad del fragmento C inmediatamente después de la explosión.
b) Calcular la energía liberada por la explosión.
c) Si después de la explosión los fragmentos están en caída libre, ¿cómo se mueve el CM? Justificar.

---

## Ejercicio 15 — Momento angular de partícula libre

Una partícula de **0,5 kg** se mueve a velocidad constante **v** = 4 m/s î a lo largo de la recta y = 3 m (sin fuerzas).

a) Calcular el módulo y dirección de **L** respecto al origen O.
b) ¿Cómo varía **L**_O con el tiempo? Justificar usando d**L**/dt = **τ**_neto.
c) Calcular **L** respecto al punto A = (0, 3) m.
d) ¿Por qué da distinto respecto a O y a A?

---

# Nivel 4 — Avanzado (combinados de parcial)

## Ejercicio 16 — Bloque sobre carro con rozamiento

Un carro de **M = 4 kg** está inicialmente en reposo sobre piso sin rozamiento. Encima del carro hay un bloque de **m = 1 kg** que tiene una velocidad inicial de **v₀ = 3 m/s** respecto al piso. El coeficiente de rozamiento entre bloque y carro es **μ = 0,3**. (No hay rozamiento entre el carro y el piso.)

a) Diagrama de cuerpo libre para el bloque y para el carro mientras el bloque desliza. Identificar los pares de interacción.
b) Hallar las aceleraciones del bloque y del carro respecto al piso.
c) Calcular el tiempo que tardan en alcanzar una velocidad común.
d) ¿Cuál es la velocidad común final?
e) Calcular el desplazamiento del bloque y del carro respecto al piso, y el desplazamiento relativo del bloque respecto al carro.
f) Hallar el trabajo del rozamiento sobre el bloque y sobre el carro. Verificar que la suma iguala ΔK del sistema.
g) Calcular el calor disipado y comparar con el resultado de (f).

---

## Ejercicio 17 — Bloque sobre rampa móvil sin rozamiento

Una rampa curva de masa **M = 8 kg** está apoyada sobre un piso sin rozamiento. Sobre su cara curva (también sin rozamiento) se libera desde el reposo un bloque de **m = 2 kg** a una altura inicial **h = 0,5 m** respecto al piso. La rampa termina en una salida horizontal a nivel del piso.

a) Analizar la conservación: ¿se conserva **P**_x? ¿**P**_y? ¿E_mec? Justificar.
b) Hallar la velocidad del bloque y la velocidad de la rampa cuando el bloque sale por la parte horizontal (h = 0).
c) Calcular el trabajo que la normal entre bloque y rampa realiza sobre el bloque entre el inicio y el final.

---

## Ejercicio 18 — Bala atraviesa bloque colgante (con loop)

Una bala de masa **m = 50 g** lleva velocidad horizontal **V** y atraviesa un bloque de **M = 2 kg** colgado de una cuerda ideal de longitud **L = 1 m** sujeta a un punto fijo. Tras atravesarlo, la bala sale con velocidad **V/3** en la misma dirección. El tiempo de contacto es despreciable.

a) Analizar qué se conserva durante el contacto entre bala y bloque (P, L, K).
b) Calcular la velocidad mínima que debe tener el bloque inmediatamente después del impacto para describir un **círculo completo** (loop) en el plano vertical.
c) Hallar la **V mínima** de la bala para que esto ocurra.
d) En el punto más alto del loop, ¿puede ser nula la velocidad del bloque? Justificar.

---

## Ejercicio 19 — Patinadores con varilla

Dos patinadores de **m = 70 kg** cada uno se mueven sobre hielo sin rozamiento en líneas paralelas separadas **2 m**, en sentidos opuestos y con rapidez **v = 6 m/s**. Cuando se cruzan, ambos toman simultáneamente los extremos de una varilla rígida de masa despreciable de **2 m** de largo.

a) Hallar la velocidad del CM antes y después de tomar la varilla.
b) Calcular **L** respecto al CM antes y después de tomar la varilla.
c) ¿Se conserva la energía cinética en este proceso? Justificar.
d) Posteriormente, los patinadores tiran de la varilla acercándose hasta quedar separados **1 m**. Calcular la nueva rapidez de cada patinador y la nueva K.
e) ¿De dónde proviene la energía extra entre (c) y (d)?

---

## Ejercicio 20 — Choque elástico bola–plano inclinado móvil

Un plano inclinado de masa **M = 3 kg** y ángulo **α = 30°** está en reposo sobre un piso sin rozamiento. Una bola de **m = 1 kg** se mueve horizontalmente con **v₀ = 6 m/s** y choca elásticamente contra la cara inclinada. Después del choque, la bola sale **perpendicular al piso** (verticalmente hacia arriba).

a) Discutir qué se conserva durante el choque: **P**_x, **P**_y, K. Justificar especialmente por qué **P**_y NO se conserva.
b) Hallar la velocidad del plano después del choque.
c) Hallar la rapidez con la que sale la bola.
d) Calcular la altura máxima que alcanza la bola después del choque.

---

# Respuestas (resultados numéricos)

> Si no llegás al mismo resultado, vení y vemos paso a paso ese problema. Aquí solo van los números finales.

## Nivel 1

**Ej. 1** — a) J = 48 N·s. b) v_f = 16 m/s. c) v_f = 14 m/s (la fuerza primero frena los 2 m/s en sentido contrario y luego acelera).

**Ej. 2** — a) J = (1/2)·5·20 + 5·20 = 50 + 100 = **150 N·s**. b) v = 75 m/s. c) F_media = J/Δt = 15 N.

**Ej. 3** — a) v_ciclista = 80 m/s. b) K_ciclista / K_auto = m_auto / m_ciclista = **20**. c) Porque K = p²/(2m): a igual p, menor masa → mayor K.

**Ej. 4** — a) x_CM = (0 + 12 + 50)/10 = **6,2 m**. b) v_CM = (m₁·v₁)/M = (2·3)/10 = **0,6 m/s î**. c) Igual: 0,6 m/s î (no hay F_ext → v_CM se conserva).

**Ej. 5** — a) **r**_CM = (−0,4 , 0,6) m. **v**_CM = (0,8 , 0,4) m/s. b) **P** = M·**v**_CM = 5·(0,8 , 0,4) = (4, 2) kg·m/s. c) **r**_CM(5s) = (−0,4 , 0,6) + 5·(0,8 , 0,4) = (3,6 , 2,6) m.

## Nivel 2

**Ej. 6** — a) v_f = (4000 + 2400)/2000 = **3,2 m/s**. b) K_i = 10000 + 2400 = 12400 J. K_f = 10240 J. **ΔK = −2160 J**. c) Pérdida ≈ 17,4 %.

**Ej. 7** — a) v'₁ = ((2−4)·6)/6 = **−2 m/s**. v'₂ = (2·2·6)/6 = **4 m/s**. b) K_i = 36 J. K_f = 0,5·2·4 + 0,5·4·16 = 4 + 32 = 36 J ✓. c) Con masas iguales: **intercambian velocidades** → v'₁ = 0, v'₂ = 6 m/s.

**Ej. 8** — Planteo: CM no se mueve. Sea Δx_persona y Δx_balsa los desplazamientos respecto al agua, con la balsa en sentido contrario a la persona. La persona se mueve 6 m respecto a la balsa: Δx_persona − Δx_balsa = 6 m (con signos coherentes). Conservación del CM: 60·Δx_p + 240·Δx_b = 0. Resolviendo: **balsa retrocede 1,2 m**, **persona avanza 4,8 m**. c) Sin F_ext horizontal → v_CM = 0 siempre → CM fijo.

**Ej. 9** — a) Conservación P: 0 = 1·(−6) + 3·v₂ → **v₂ = +2 m/s**. b) E_resorte = K_f = (1/2)(1)(36) + (1/2)(3)(4) = **24 J**. c) (1/2)·k·x² = 24 → x² = 48/1500 → **x ≈ 0,179 m ≈ 17,9 cm**.

**Ej. 10** — Tomar +y hacia arriba. Δv = +6 − (−8) = 14 m/s. a) **J_piso = 7 N·s** (hacia arriba). b) F_media = J/Δt = **700 N**. c) J_peso = m·g·Δt = 0,5·9,8·0,01 = 0,049 N·s → despreciable (700 N vs 4,9 N). d) NO es elástico: K_i = 16 J, K_f = 9 J → se pierde 7 J (44 %).

## Nivel 3

**Ej. 11** — a) v_CM = (10 − 9)/5 = **0,2 m/s î**. b) K_lab = 25 + 13,5 = **38,5 J**. c) v₁' = 4,8 m/s, v₂' = −3,2 m/s. K_CM = 23,04 + 15,36 = **38,4 J**. d) (1/2)·M·v_CM² = 0,1 J. K_CM + 0,1 = 38,5 = K_lab ✓.

**Ej. 12** — P_x = 1000·20 = 20000 kg·m/s (este). P_y = 2000·15 = 30000 kg·m/s (norte). v_fx = 20000/3000 ≈ 6,67 m/s; v_fy = 10 m/s. |v_f| = √(44,5 + 100) ≈ **12,02 m/s**. Dirección: θ = arctan(10/6,67) ≈ **56,3°** al N del E. b) K_i = 200000 + 225000 = 425000 J. K_f = (1/2)(3000)(144,5) ≈ 216750 J. **ΔK ≈ −208250 J**. c) ≈ 49 % se disipa.

**Ej. 13** — a) Por energía mec. (después del choque, sólo gravedad): v_después = √(2gh) = √(2·9,8·0,12) ≈ **1,53 m/s**. b) Conservación P (choque plástico): 0,02·v_bala = 4,02·1,53 → **v_bala ≈ 308 m/s**. c) K_inicial ≈ 950 J. K_después_choque ≈ 4,7 J. Razón ≈ **0,5 %** (se pierde 99,5 % en el choque).

**Ej. 14** — a) **P**_inicial = (60, 0). **P**_C = (60 − 15 − 8 , 0 − 8 + 24) = (37, 16) kg·m/s. **v**_C = (37/3 , 16/3) ≈ **(12,33 , 5,33) m/s**. b) K_i = 300 J. K_f = (1/2)(1)(289) + (1/2)(2)(160) + (1/2)(3)(180,6) ≈ 144,5 + 160 + 270,8 = **575,3 J**. Energía liberada ≈ **275,3 J**. c) El CM se mueve como una partícula con caída libre (sólo actúa el peso total): trayectoria parabólica con velocidad inicial (10, 0) y aceleración (0, −g).

**Ej. 15** — a) d = 3 m (distancia perpendicular). |L_O| = m·v·d = 0,5·4·3 = **6 kg·m²/s**. Dirección: **L** = **r** × **p** = (x, 3, 0) × (2, 0, 0) = (0, 0, −6) → en **−k̂**. b) **L**_O es constante: no hay fuerzas → **τ**_O = 0 → d**L**/dt = 0. c) Respecto a A=(0,3): la línea de **v** pasa por A → d = 0 → **L_A = 0**. d) Porque L depende del punto de referencia; sólo cuando el punto está sobre la línea de acción de **v**, L se anula.

## Nivel 4

**Ej. 16** —
a) **DCL bloque**: peso (↓), normal del carro N (↑), rozamiento f hacia atrás. **DCL carro**: peso (↓), normal del piso N_p (↑), normal del bloque N (↓, reacción), rozamiento f hacia adelante (reacción del de arriba).
b) f = μ·m·g = 0,3·1·9,8 = **2,94 N**.
  a_bloque = −f/m = **−2,94 m/s²**.
  a_carro = f/M = **+0,735 m/s²**.
c) v común por conservación de P: 1·3 = 5·v_f → **v_f = 0,6 m/s**.
  t = (3 − 0,6)/2,94 = **0,816 s**.
d) v_común = **0,6 m/s**.
e) Δx_bloque = 3·0,816 − 0,5·2,94·0,816² ≈ **1,47 m**. Δx_carro = 0,5·0,735·0,816² ≈ **0,245 m**. Δx_rel = **1,225 m**.
f) W_f sobre bloque = −2,94·1,47 ≈ **−4,32 J**. W_f sobre carro = +2,94·0,245 ≈ **+0,72 J**. Suma = −3,6 J. ΔK = (1/2)(5)(0,36) − (1/2)(1)(9) = −3,6 J ✓.
g) Q = f·Δx_rel = 2,94·1,225 ≈ **3,6 J** ✓ (iguala el módulo de la pérdida de K).

**Ej. 17** —
a) **P**_x se conserva (no hay F_ext horizontal). **P**_y NO se conserva (normal del piso actúa). E_mec se conserva (no hay rozamiento, normales no trabajan en el sistema total).
b) Inicial: P = 0. Final: 0 = m·v_b + M·v_r → v_r = −(m/M)·v_b = −v_b/4.
  E: m·g·h = (1/2)m·v_b² + (1/2)M·v_r² → 9,8 = v_b² + 4·(v_b/4)² = 1,25·v_b².
  **v_b = 2,8 m/s** (a la derecha). **v_r = −0,7 m/s** (a la izquierda).
c) Sobre el bloque, la normal hace trabajo distinto de cero porque el bloque se mueve. Por teorema W_total = ΔK_bloque: W_peso + W_normal = (1/2)(2)(2,8²) − 0 = 7,84 J. W_peso = m·g·h = 9,8 J. → **W_normal sobre bloque = 7,84 − 9,8 = −1,96 J**.

**Ej. 18** —
a) Durante el contacto (Δt → 0): se conserva **P** del sistema bala+bloque (el impulso del peso y de la cuerda son despreciables). NO se conserva K (es un choque inelástico, queda calor + deformación). **L** respecto al punto de suspensión sí se conserva si el contacto es puntual (la tensión actúa en la línea bloque-pivote).
b) En el punto más alto del loop, condición mínima: peso = fuerza centrípeta → M·g = M·v_arriba²/L → **v_arriba_min = √(gL) = √9,8 ≈ 3,13 m/s**.
  Por conservación de E entre el punto bajo (después del impacto) y el punto alto (altura 2L):
  (1/2)·M·v_post² = (1/2)·M·v_arriba² + M·g·(2L)
  v_post² = v_arriba² + 4gL = gL + 4gL = 5gL = 49 → **v_post = 7 m/s**.
c) Conservación de P en el contacto: m·V = m·(V/3) + M·v_post → (2/3)·m·V = M·v_post → V = (3·M·v_post)/(2·m) = (3·2·7)/(2·0,05) = **V_min = 420 m/s**.
d) No, no puede ser cero: en el punto alto la tensión de la cuerda no puede empujar (sólo tira); si v fuera cero, no habría fuerza centrípeta hacia el centro y el bloque caería antes de cerrar el círculo. La condición límite es justamente T = 0 (sólo gravedad aporta la centrípeta).

**Ej. 19** —
a) Antes: por simetría (masas iguales, velocidades opuestas) **v**_CM = 0. Después de tomar la varilla, la fuerza es interna al sistema → **v**_CM = 0 igual.
b) Antes: cada patinador a 1 m del CM (mitad de la varilla), con velocidad tangencial 6 m/s. |L_CM| = 2·(m·v·d) = 2·(70·6·1) = **840 kg·m²/s**. Después: idéntico (el momento "tomar la varilla" es un par de fuerzas internas que pasan por la línea de los patinadores, no genera torque externo respecto del CM). |L_CM| = **840 kg·m²/s**.
c) K_antes = 2·(1/2·70·36) = **2520 J**. Después del enganche, cada uno hace MCU de radio 1 m con la misma rapidez tangencial (porque L se conservó y r tampoco cambia en el instante del enganche). K_después = **2520 J**. **Se conserva** porque las velocidades ya eran perpendiculares a la varilla → la fuerza axial impulsiva no hace trabajo.
d) Al acortar a r' = 0,5 m, conservación de L: 2·m·v'·r' = 840 → **v' = 12 m/s**.
  K' = 2·(1/2·70·144) = **10080 J**.
e) La energía extra (10080 − 2520 = 7560 J) la aportan los patinadores con el **trabajo de la fuerza muscular** al tirar de la varilla acortando el radio (las fuerzas son ahora radiales, paralelas al desplazamiento → sí trabajan).

**Ej. 20** —
a) **P**_x se conserva: no hay F_ext horizontal. **P**_y NO se conserva: la normal del piso sobre el plano es externa al sistema bola+plano. K se conserva (es elástico).
b) Conservación P_x: m·v₀ = M·V → V = (1·6)/3 = **V = 2 m/s** (el plano se mueve horizontalmente).
c) Conservación K: (1/2)·m·v₀² = (1/2)·m·v_f² + (1/2)·M·V². 18 = 0,5·v_f² + 6 → v_f² = 24 → **v_f = √24 ≈ 4,9 m/s** (vertical hacia arriba).
d) Altura máxima: h_max = v_f²/(2g) = 24/19,6 ≈ **1,22 m**.

---

# Cómo usar esta guía

1. **Resolvé sin mirar las respuestas**. Si te trabás más de 15 min, pasá a la teoría (Unidad2-SistemasParticulas.md) y volvé.
2. **Después de cada nivel** (5 ejercicios), revisá los conceptos que más te costaron antes de pasar al siguiente.
3. **Si todos los del Nivel 4 los hacés solo**, ya estás listo para parcial.
4. **Los ejercicios 16, 17 y 18** son los más típicos de parcial — practicá esos hasta hacerlos de memoria.

Cualquier ejercicio que no te salga, me lo decís y lo desarrollamos paso a paso.
