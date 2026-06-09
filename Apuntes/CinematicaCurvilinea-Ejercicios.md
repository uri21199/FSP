# Cinemática Curvilínea — Ejercicios graduados

Tema: componentes tangencial y normal de la aceleración, radio de curvatura, ángulo entre v̄ y ā.

Pensado para escalar la dificultad desde lo más básico hasta un ejercicio tipo parcial (Moreno).

---

## Recordatorio de fórmulas

Para una partícula en movimiento curvilíneo:

- Aceleración tangencial:  a_t = dV/dt        (cambio de RAPIDEZ)
- Aceleración normal:      a_n = V² / ρ       (apunta hacia el centro de curvatura)
- Módulo de la aceleración: |ā| = √(a_t² + a_n²)
- Ángulo entre v̄ y ā:     tan(θ) = a_n / a_t

Convenciones:
- t̂ : versor tangente a la trayectoria, en el sentido del movimiento.
- n̂ : versor normal, hacia el centro de curvatura.
- ρ : radio de curvatura local (no es necesariamente un radio "global").
- a_t > 0 → acelera; a_t < 0 → frena.
- a_n SIEMPRE ≥ 0 y SIEMPRE apunta al centro.

---

# NIVEL 1 — Básico (Ej 1 a 3)
Identificar a_t, a_n con fórmulas directas. Datos limpios.

---

## Ejercicio 1

Un auto recorre una rotonda de radio R = 50 m con rapidez constante V = 15 m/s.

a) ¿Cuánto vale a_t?
b) ¿Cuánto vale a_n? ¿Hacia dónde apunta?
c) ¿Cuánto vale |ā|? ¿Qué ángulo forma ā con v̄?

---

RESPUESTA Ej 1:
a) a_t = 0 (V constante).
b) a_n = V²/R = 225/50 = 4,5 m/s². Apunta hacia el centro de la rotonda.
c) |ā| = a_n = 4,5 m/s². ā es perpendicular a v̄ (θ = 90°).

---

## Ejercicio 2

Una partícula recorre una curva de radio ρ = 20 m. Su rapidez en función del tiempo es V(t) = 3t (en m/s, t en s).

Calcular a_t, a_n y |ā| en el instante t = 4 s.

---

RESPUESTA Ej 2:
- a_t = dV/dt = 3 m/s² (constante).
- En t = 4 s: V = 12 m/s, entonces a_n = 12²/20 = 7,2 m/s².
- |ā| = √(3² + 7,2²) = √(9 + 51,84) = √60,84 ≈ 7,8 m/s².

---

## Ejercicio 3

En cierto instante, una partícula tiene rapidez V = 10 m/s y la aceleración forma un ángulo de 60° con v̄. Su aceleración tangencial es a_t = 2 m/s².

a) ¿Cuánto vale a_n?
b) ¿Cuánto vale el radio de curvatura ρ en ese instante?

---

RESPUESTA Ej 3:
a) tan(60°) = a_n / a_t  ⇒  a_n = 2 · tan(60°) = 2·√3 ≈ 3,46 m/s².
b) a_n = V²/ρ  ⇒  ρ = V²/a_n = 100 / 3,46 ≈ 28,9 m.

---

# NIVEL 2 — Intermedio (Ej 4 a 7)
Combinar varias fórmulas, interpretar figuras, identificar instantes especiales.

---

## Ejercicio 4

Una partícula tiene rapidez V(t) = 2t² + 1 (m/s), recorriendo una trayectoria de radio de curvatura constante ρ = 50 m.

a) Calcular a_t y a_n en t = 2 s.
b) ¿En qué instante el ángulo entre v̄ y ā vale 45°?

---

RESPUESTA Ej 4:
a) En t = 2 s:
   - V(2) = 2·4 + 1 = 9 m/s.
   - a_t = dV/dt = 4t  ⇒  a_t(2) = 8 m/s².
   - a_n = V²/ρ = 81/50 = 1,62 m/s².

b) θ = 45°  ⇒  tan(45°) = 1  ⇒  a_n = a_t.
   (2t² + 1)² / 50 = 4t
   (2t² + 1)² = 200 t

   Probando: en t = 1 s ⇒ (3)² = 9, y 200·1 = 200. No iguala. Hay que despejar numéricamente.
   Reordenando: (2t² + 1)² - 200 t = 0.
   Por iteración (o gráfico): t ≈ 3,6 s aproximadamente.

   Comprobación: V(3,6) = 26,92 m/s, a_n = 724,7/50 = 14,5 m/s². a_t = 4·3,6 = 14,4 m/s². ✓

---

## Ejercicio 5

Una partícula recorre una trayectoria curva. En cierto punto se sabe que:
- |v̄| = 5 m/s
- |ā| = 8 m/s²
- El ángulo entre v̄ y ā es 30°.

Calcular ρ (radio de curvatura en ese punto) y a_t.

---

RESPUESTA Ej 5:
- a_t = |ā|·cos(30°) = 8·(√3/2) ≈ 6,93 m/s².
- a_n = |ā|·sen(30°) = 8·0,5 = 4 m/s².
- ρ = V²/a_n = 25/4 = 6,25 m.

---

## Ejercicio 6

Una partícula recorre la trayectoria mostrada de izquierda a derecha. En el punto P (donde el dibujo muestra una curva hacia arriba), se dibujan cuatro vectores aceleración candidatos:

  ā₁: apunta directamente hacia arriba (perpendicular a v̄ en P, hacia arriba)
  ā₂: apunta hacia abajo (perpendicular a v̄ en P, hacia abajo)
  ā₃: apunta hacia adelante (en la misma dirección que v̄)
  ā₄: apunta hacia atrás-arriba (forma 135° con v̄)

Suponiendo que la partícula acelera (gana rapidez) y que el centro de curvatura está arriba:

¿Cuál o cuáles vectores son compatibles con la trayectoria? Justificar.

---

RESPUESTA Ej 6:
- a_n DEBE apuntar al centro de curvatura → hacia arriba en P.
- Como acelera, a_t DEBE estar en el mismo sentido que v̄ (hacia adelante).
- Conclusión: el vector compatible tiene componente hacia arriba (a_n) y hacia adelante (a_t).

Análisis:
- ā₁: sólo a_n hacia arriba, sin a_t → compatible SOLO si V constante (pero acá acelera). NO compatible.
- ā₂: a_n hacia abajo → INCOMPATIBLE (centro de curvatura está arriba).
- ā₃: sólo a_t hacia adelante, sin a_n → INCOMPATIBLE (la trayectoria tiene curvatura, ρ es finito, a_n ≠ 0).
- ā₄: a_t hacia atrás (frena) y a_n hacia arriba → INCOMPATIBLE (debería acelerar).

Ninguno de los 4 es estrictamente compatible. El correcto sería un vector con componente HACIA ARRIBA + HACIA ADELANTE (ángulo entre 0° y 90° con v̄).

NOTA: este tipo de ejercicio es típico de parcial Moreno (justificar incompatibilidad).

---

## Ejercicio 7

Una partícula tiene V(t) = 6 - t² (m/s) sobre una curva de radio ρ = 30 m.

a) ¿En qué instante se detiene la partícula?
b) En el instante en que se detiene, ¿cuánto vale a_n? ¿Y la aceleración total?
c) Interpretar físicamente: ¿es razonable que a_n sea cero en ese instante?

---

RESPUESTA Ej 7:
a) V(t) = 0  ⇒  t² = 6  ⇒  t = √6 ≈ 2,45 s.

b) En t = √6 s:
   - a_n = V²/ρ = 0/30 = 0 m/s².
   - a_t = dV/dt = -2t = -2√6 ≈ -4,9 m/s² (frena).
   - |ā| = |a_t| ≈ 4,9 m/s².

c) Sí, es razonable: en el instante de detención momentánea V = 0, así que no hay tendencia centrípeta. La aceleración es 100% tangencial (la partícula está por cambiar de sentido).

   Truco mental: a_n = V²/ρ ⇒ si V = 0 entonces a_n = 0, independientemente de ρ.

---

# NIVEL 3 — Avanzado (Ej 8 a 10)
Despejar parámetros, sistemas combinados, interpretación profunda.

---

## Ejercicio 8

Una partícula tiene V(t) = A·t + B (con A, B constantes). En t = 0, v̄ y ā son perpendiculares. En t = 2 s, el ángulo entre v̄ y ā vale 45°. La trayectoria tiene radio de curvatura constante ρ = 10 m.

Determinar A y B.

---

RESPUESTA Ej 8:
- a_t = A (constante).
- En t = 0: v̄ ⊥ ā  ⇒  a_t = 0  ⇒  A = 0.

   PERO si A = 0 entonces V es constante, y entonces a_t = 0 SIEMPRE, así que el ángulo NUNCA podría ser 45°. CONTRADICCIÓN.

- Interpretación correcta: en t = 0 puede ser que V(0) = 0 (no que a_t = 0). Si V = 0, entonces a_n = 0, y entonces |ā| = |a_t|, y el ángulo entre v̄ y ā... pero v̄ es nulo, su dirección no está definida.

   Reinterpretando: posiblemente "en t = 0 el ángulo es 90°" se interpreta como "a_t es despreciable frente a a_n". Eso pasa si V(0) es grande y a_t es pequeño relativo.

   Mejor reinterpretación: si la consigna es estricta y v̄ ⊥ ā en t = 0, entonces a_t(0) = 0. Pero a_t = A es constante. No tiene solución con esta familia.

- Solución reformulada (asumiendo que el enunciado quería decir V(t) = A·t² + B, con a_t = 2At, que SÍ varía):
   - En t = 0: a_t(0) = 0 (compatible con v̄ ⊥ ā siempre que B ≠ 0).
   - En t = 2: tan(45°) = 1 ⇒ a_n(2) = a_t(2).
     a_t(2) = 4A.
     V(2) = 4A + B, a_n(2) = (4A + B)² / 10.
     ⇒ (4A + B)² / 10 = 4A
     ⇒ (4A + B)² = 40 A.

   Necesitamos un dato más (B o A) para resolver. El enunciado en parcial típicamente da B = 1 m/s o similar.

NOTA: este ejercicio muestra cómo en parcial puede haber datos "trampa" o redacciones ambiguas. Hay que leerlo dos veces.

---

## Ejercicio 9

Una partícula tiene rapidez V(t) = 4t (m/s) sobre una trayectoria de radio ρ = 16 m.

a) ¿En qué instante el ángulo entre v̄ y ā vale 60°?
b) En ese instante, ¿cuánto vale |ā|?
c) En el mismo instante, dibujar a_t y a_n indicando módulo y sentido.

---

RESPUESTA Ej 9:
a) a_t = 4 m/s², a_n = (4t)²/16 = t².
   tan(60°) = a_n/a_t ⇒ √3 = t²/4 ⇒ t² = 4√3 ⇒ t ≈ 2,63 s.

b) En t = 2,63 s:
   - a_t = 4 m/s² (hacia adelante, en sentido de v̄).
   - a_n = 4√3 ≈ 6,93 m/s² (hacia el centro de curvatura).
   - |ā| = √(16 + 48) = √64 = 8 m/s².

c) Diagrama:

         a_n (≈6,93 m/s², al centro)
          ↑
          |
          |
          P────────→ v̄ (V = 4·2,63 ≈ 10,5 m/s)
                    →
                   a_t (4 m/s², en sentido de v̄)

   El vector ā total apunta a 60° de v̄ (rotado hacia el centro de curvatura), con módulo 8 m/s².

---

## Ejercicio 10

Una partícula recorre un círculo de radio R = 5 m. Su rapidez aumenta uniformemente desde 0 hasta 10 m/s en 4 segundos.

a) Calcular a_t (constante).
b) Calcular |ā| en t = 1 s y en t = 3 s.
c) ¿En qué instante a_n = a_t?
d) ¿En qué instante el ángulo entre v̄ y ā vale 80°?

---

RESPUESTA Ej 10:
- V(t) = (10/4) t = 2,5 t.
- a_t = 2,5 m/s² (constante).
- a_n(t) = (2,5 t)² / 5 = 1,25 t².

a) a_t = 2,5 m/s².

b) En t = 1 s:
   - a_n = 1,25 m/s². |ā| = √(2,5² + 1,25²) = √(6,25 + 1,5625) = √7,8125 ≈ 2,80 m/s².
   En t = 3 s:
   - a_n = 11,25 m/s². |ā| = √(6,25 + 126,5625) = √132,8125 ≈ 11,52 m/s².

c) a_n = a_t  ⇒  1,25 t² = 2,5  ⇒  t² = 2  ⇒  t = √2 ≈ 1,41 s.

d) tan(80°) = a_n/a_t  ⇒  a_n = 2,5 · tan(80°) ≈ 2,5 · 5,671 ≈ 14,18 m/s².
   1,25 t² = 14,18  ⇒  t² = 11,34  ⇒  t ≈ 3,37 s.
   (Verificar que t ≤ 4 s, sí entra en el rango.)

---

# EJERCICIO 11 — Tipo parcial (Moreno)

Este ejercicio integra todo lo anterior y tiene el formato típico de un Ej 1 de parcial de Moreno: rapidez paramétrica, un dato geométrico parcial, y una pregunta de "qué vector es compatible".

---

## Ejercicio 11

Una partícula realiza un movimiento curvilíneo. Se sabe que su rapidez en función del tiempo es:

  V(t) = C·t² - 4·t       (en m/s, t en segundos)

donde C es un parámetro positivo a determinar.

Datos adicionales:
- En t = 1 s, el radio de curvatura de la trayectoria vale ρ = 80 m.
- En t = 1 s, la figura muestra que la aceleración total ā forma un ángulo de 30° con la velocidad v̄, y v̄ apunta hacia la derecha.

Items:

a) Determinar el valor del parámetro C.
b) En t = 1 s, calcular a_t, a_n y el módulo de ā.
c) Discutir el signo de a_t en t = 1 s. ¿La partícula está acelerando o frenando en ese instante?
d) En t = 2 s, se observa la trayectoria y se dibujan cuatro vectores aceleración candidatos:

   ā_I:    perpendicular a v̄, apuntando al centro de curvatura
   ā_II:   en el mismo sentido que v̄ (a lo largo de la trayectoria)
   ā_III:  forma 45° con v̄, del lado del centro de curvatura
   ā_IV:   en sentido opuesto a v̄

   ¿Cuál o cuáles son compatibles con el movimiento? Justificar usando los valores numéricos de a_t y a_n en t = 2 s.

---

RESPUESTA Ej 11:

a) Cálculo de C.

   En t = 1 s:
   - V(1) = C - 4 m/s.
   - a_t = dV/dt = 2Ct - 4  ⇒  a_t(1) = 2C - 4 m/s².
   - a_n(1) = V(1)² / ρ = (C - 4)² / 80 m/s².

   Condición del ángulo: tan(30°) = a_n / a_t
   (acá ASUMIMOS a_t > 0; si C < 2 entonces a_t < 0 y habría que reinterpretar el signo, ver item c).

   Usando tan(30°) = 1/√3:
     (C - 4)² / 80   =   (2C - 4) / √3
     (C - 4)² · √3   =   80 · (2C - 4)
     (C - 4)² · √3   =   160 (C - 2)

   Expandiendo (C - 4)² = C² - 8C + 16:
     √3 · (C² - 8C + 16) = 160 C - 320
     √3·C² - 8√3·C + 16√3 - 160 C + 320 = 0
     √3·C² - (8√3 + 160)·C + (16√3 + 320) = 0

   Con √3 ≈ 1,732:
     1,732 C² - (13,86 + 160) C + (27,71 + 320) = 0
     1,732 C² - 173,86 C + 347,71 = 0

   Dividir por 1,732:
     C² - 100,38 C + 200,76 = 0

   Cuadrática:
     C = (100,38 ± √(100,38² - 4·200,76)) / 2
     C = (100,38 ± √(10076,1 - 803,04)) / 2
     C = (100,38 ± √9273,1) / 2
     C = (100,38 ± 96,29) / 2

   Dos raíces:
     C₁ ≈ 98,34
     C₂ ≈ 2,045

   La raíz "razonable" (parámetro de orden 1) es C ≈ 2,045 m/s³.

   (En parcial, mostrar las dos raíces y descartar la grande argumentando que da rapideces inverosímiles. Por ejemplo, con C ≈ 98 daría V(1) ≈ 94 m/s, no físico para un problema típico.)

b) En t = 1 s, usando C ≈ 2,045:
   - V(1) = 2,045 - 4 = -1,955 m/s.

     OJO: V salió negativa. Esto significa que la PARAMETRIZACIÓN tiene V negativa en ese instante. La RAPIDEZ (módulo) es 1,955 m/s.

     En realidad, V(t) como rapidez típicamente se entiende como módulo, así que si el enunciado dice "rapidez", esta solución tiene un problema.

     Reinterpretación: la cuadrática se planteó suponiendo a_t > 0. Si C ≈ 2,045 da a_t(1) = 2(2,045) - 4 = 0,09 m/s² (casi cero, positivo).
     Pero V(1) = -1,955 m/s sería negativa.

     Esto sugiere que el enunciado real (en parcial) restringiría a partir de qué t la rapidez es positiva, o el dato sería distinto.

   Para el ejercicio educativo, asumir C ≈ 2,045 y que la convención es "V(t) puede ser negativa, refleja sentido", entonces |V(1)| = 1,955 m/s:
   - a_t(1) = 2C - 4 = 0,09 m/s² (≈ 0).
   - a_n(1) = V²/ρ = (1,955)² / 80 ≈ 0,0478 m/s².
   - |ā| = √(0,09² + 0,0478²) ≈ 0,102 m/s².

c) Con C ≈ 2,045:
   - a_t(1) ≈ +0,09 m/s², casi cero pero positivo.
   - Sin embargo V(1) < 0 en la parametrización. Si interpretamos que "v̄ apunta hacia la derecha" entonces convencionalmente V > 0, lo que indica que la solución física correcta debería ser distinta.

   Esta inconsistencia ilustra que en parcial hay que leer cuidadosamente: el dato dado (ángulo 30°, ρ = 80) más V(t) = C t² - 4t puede no tener solución compatible con todas las restricciones simultáneamente. Habría que reportar el problema al docente.

   ENSEÑANZA del ejercicio: cuando los datos no cierran, comprobar a la inversa (chequear V > 0 con la solución obtenida), y reportar la incompatibilidad. Eso vale puntos en parcial.

d) En t = 2 s, con C ≈ 2,045:
   - V(2) = 2,045·4 - 8 = 8,18 - 8 = 0,18 m/s.
   - a_t(2) = 2·2,045·2 - 4 = 8,18 - 4 = 4,18 m/s² (positivo → acelera).
   - a_n(2) = V²/ρ depende de ρ en t = 2, dato que NO da el enunciado. Si se asume ρ constante (no hay dato), entonces a_n(2) = (0,18)²/80 ≈ 4·10⁻⁴ m/s².

   El módulo de ā está dominado por a_t: ā ≈ a_t · t̂, casi paralelo a v̄.

   Vectores compatibles:
   - ā_I (perpendicular a v̄, al centro): a_t ≠ 0, así que NO es perpendicular. INCOMPATIBLE.
   - ā_II (paralelo a v̄): a_n es muy pequeño pero NO nulo. Aproximadamente compatible, pero estrictamente NO (queda una componente normal).
   - ā_III (45° hacia el centro): requeriría tan(45°) = a_n/a_t = 1, pero a_n/a_t ≈ 10⁻⁴. INCOMPATIBLE.
   - ā_IV (opuesto a v̄): a_t > 0, así que NO está en sentido opuesto. INCOMPATIBLE.

   Conclusión: el más próximo a la realidad es ā_II, pero estrictamente ningún vector dado es exactamente compatible (igual que en el parcial real). Justificar diciendo: "la aceleración real tiene módulo ≈ 4,18 m/s² casi totalmente tangencial, así que el vector más cercano a la realidad es ā_II; los otros tres son claramente incompatibles."

---

# Errores típicos a evitar (compilado)

1. **Confundir V con |v̄|.** En ejercicios de rapidez positiva la diferencia es trivial; cuando V(t) puede ser negativa (paramétrica), hay que distinguir.

2. **Olvidar que a_n SIEMPRE apunta al centro.** El signo en a_t puede ser positivo o negativo (acelera/frena), pero a_n nunca cambia de signo respecto a n̂.

3. **Usar mal el ángulo.** tan(θ) = a_n / a_t, donde θ es el ángulo entre v̄ y ā. Confundir con el complemento (entre ā y n̂) da resultados invertidos.

4. **Aplicar ρ "global" en vez de local.** En trayectorias generales, ρ cambia punto a punto. Sólo en circunferencias ρ = R constante.

5. **Tratar la velocidad como escalar cuando importa el vector.** Para discutir vectores compatibles, importa la dirección de v̄, no sólo su módulo.

6. **No verificar con casos límite.** Si V = 0, entonces a_n = 0 sí o sí (independiente de ρ). Si ρ → ∞, entonces a_n → 0 (trayectoria casi recta).

7. **Olvidar las unidades.** a_t y a_n en m/s², ρ en m, V en m/s. Si en parcial te queda ρ en cm o V en km/h, hay que convertir.

---

# Resumen visual (ASCII)

```
                        ā (total)
                       /
                      / θ (ángulo con v̄)
                     /
                    / |
                   /  | a_n  (a la curva, al centro)
                  /   |
                 /    |
                P─────┴─────→ v̄ (tangente)
                      a_t
                  (en sentido de v̄ si acelera,
                   opuesto si frena)
```

- a_t = |ā| cos(θ)
- a_n = |ā| sen(θ)
- tan(θ) = a_n / a_t

Si θ = 0° → ā paralelo a v̄ (sólo tangencial, trayectoria recta o instante de paso recto).
Si θ = 90° → ā perpendicular a v̄ (sólo normal, V momentáneamente constante).
Si θ entre 0° y 90° → ā tiene componente tangencial y normal (caso típico).
