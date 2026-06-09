# Conclusiones — TP1: Mediciones e Incertezas
**Grupo 4**

---

## 1. Eficiencia de cada instrumento

La eficiencia para medir el volumen de la pieza varía notablemente entre los tres instrumentos utilizados. El calibre demostró ser el más eficiente, con un error relativo del orden del 0,6%, lo que permite obtener un resultado preciso y significativo. La probeta ofrece una precisión intermedia (~10% de error relativo), siendo funcional pero sensible a condiciones de uso. La regla milimetrada resultó completamente inadecuada para esta tarea: su error absoluto propagado (~25 cm³) supera ampliamente el valor medido (~9 cm³), haciendo el resultado no informativo.

---

## 2. Dificultades y fuentes de error por instrumento

- **Regla milimetrada:** La baja apreciación (1 mm) genera errores de lectura inevitables. La dificultad de alinear correctamente la regla con los bordes de la pieza introduce errores sistemáticos adicionales. No es adecuada para piezas pequeñas.

- **Calibre:** Requiere experiencia de uso. La inexperiencia del operador puede llevar a lecturas incorrectas de la escala Vernier, a aplicar presión no uniforme al cerrar las mordazas, o a no identificar correctamente qué parte del calibre usar (externa, interna, profundidad).

- **Probeta:** El principal error proviene de la lectura del menisco y de la alineación visual con la escala (error de paralaje). Además, al sumergir la pieza pueden producirse salpicaduras o pérdida de agua, como ocurrió con el integrante 4, cuya medición fue descartada por este motivo.

---

## 3. Conclusión sobre el instrumento más eficiente

Para la medición del volumen de esta pieza cilíndrica hueca, el **calibre** es el instrumento más eficiente. Su alta apreciación (0,02 mm) permite obtener resultados con errores relativos muy pequeños y detectar diferencias reales entre mediciones de distintos operadores. Sin embargo, su uso requiere mayor cuidado y entrenamiento que los otros instrumentos.

---

## 4. Métodos directos vs. indirectos

La probeta mide el volumen de forma **directa** por desplazamiento de agua, mientras que la regla y el calibre lo obtienen de forma **indirecta** a través de mediciones de dimensiones y cálculo geométrico. Cada enfoque tiene sus ventajas: el método directo es conceptualmente simple y no requiere conocer la geometría de la pieza, pero es sensible a errores de manipulación. El método indirecto permite mayor control sobre las fuentes de error, pero depende de la precisión del instrumento y de la correcta aplicación de la fórmula.

---

## 5. Propagación de errores y su impacto

En los métodos indirectos, el error no se mide directamente sino que se propaga a través de la fórmula de cálculo del volumen. Al intervenir tres magnitudes medidas (D_ext, D_int, h), las incertezas se acumulan. Esto explica por qué la regla, con una apreciación de solo 1 mm, produce un error final tan grande: cada medición individual ya tiene un error relativo del 5–8%, y al propagarse al volumen calculado el resultado se vuelve inutilizable. La propagación de errores es, por tanto, un factor crítico a considerar al elegir el método de medición.

---

## 6. Dispersión entre observadores

Los 10 integrantes midieron la misma pieza obteniendo valores distintos. Con la regla, las diferencias entre observadores quedan enmascaradas por el ruido del error instrumental. Con el calibre, en cambio, la alta precisión hace visibles las diferencias reales de lectura entre personas, poniendo de manifiesto el **error del operador** como fuente de variabilidad significativa. Esto subraya que la precisión de un instrumento no garantiza por sí sola la reproducibilidad de una medición.

---

## 7. Adecuación del instrumento a la escala del objeto

No existe un instrumento universalmente "mejor": la elección adecuada depende de la escala del objeto y de la precisión requerida. Para una pieza de volumen ~10 cm³, una apreciación de 1 mm en la regla resulta demasiado gruesa y hace inviable la medición indirecta del volumen. El principio general es que la apreciación del instrumento debe ser pequeña en relación al tamaño de las magnitudes que se desean medir.

---

## 8. La incerteza como parte esencial de toda medición

Una de las enseñanzas fundamentales de este trabajo práctico es que **reportar un valor numérico sin su incerteza asociada no constituye una medición completa**. Expresar V = 9 cm³ sin indicar ΔV = 25 cm³ (caso de la regla) resultaría engañoso, ya que ocultaría que el resultado carece de significado práctico. Toda medición debe acompañarse de su error para poder ser interpretada y comparada correctamente.

---
