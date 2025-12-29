---
title: "Corriendo bajo la lluvia"
author: "David Figuer"
date: 2025-12-03
layout: articles
status: published
category: "Dinámica de Fluidos"
tags: ["física", ]
image: "images/bajo_lluvia.png"
summary: Empieza a llover. Estás a unos metros de casa y te haces la eterna pregunta ¿corro o camino?  
---

[TOC]

## ¿Te mojas menos si corres bajo la lluvia?

Empieza a llover. Estás a unos metros de casa y te haces la eterna pregunta: **¿corro o camino?**  
Parece una tontería, pero detrás hay física.  
Si corres, pasas menos tiempo bajo la lluvia, aunque podrías chocar con más gotas de frente.  
Si caminas, te cruzas con menos gotas por segundo, pero estás más tiempo expuesto.  

Veamos qué dice la física cuando ponemos números y ecuaciones encima de la mesa.

![](../images/bajo_lluvia.png)

## Planteamiento del problema

Supongamos una persona de altura $h$ y anchura $w$ que recorre una distancia total $D$ bajo una lluvia que cae verticalmente con velocidad $v_g$.  
La persona se mueve horizontalmente con velocidad $v$.

La lluvia está formada por gotas con una densidad volumétrica $n_g$ (número de gotas por metro cúbico).

Queremos saber el volumen total de agua, $V_{\text{total}}$, que impacta a la persona durante el recorrido, separando los aportes desde arriba y desde el frente.

Podemos pensar en la lluvia como un flujo continuo de gotas que atraviesa una superficie. El flujo de gotas por unidad de área y tiempo es:

$$
\Phi = n_g\, v_g.
$$

Cada superficie del cuerpo intercepta parte de ese flujo, y el volumen total de agua recibido será proporcional al área expuesta, al flujo y al tiempo de exposición.

---

## Agua que cae desde arriba

El área horizontal expuesta (cabeza, hombros...) la llamaremos:

$$
A_{\text{arriba}} = w\, L_p,
$$

donde $L_p$ es una longitud efectiva del cuerpo vista desde arriba.

El volumen de agua que cae sobre esa superficie durante el tiempo $t$ que la persona está bajo la lluvia es:

$$
V_{\text{arriba}} = A_{\text{arriba}}\, n_g\, v_g\, t.
$$

El tiempo total de exposición es:

$$
t = \frac{D}{v}.
$$

Sustituyendo:

$$
V_{\text{arriba}} = A_{\text{arriba}}\, n_g\, v_g\, \frac{D}{v}.
$$

Este resultado es claro: **a mayor velocidad $v$, menor tiempo bajo la lluvia, y por tanto, menor agua recibida desde arriba.**

---

## Agua que llega de frente

El área frontal aproximada del cuerpo es:

$$
A_{\text{frente}} = h\, w.
$$

La persona atraviesa un volumen de aire igual a $A_{\text{frente}} D$, y cada metro cúbico contiene $n_g$ gotas. Por tanto:

$$
V_{\text{frente}} = A_{\text{frente}}\, n_g\, D.
$$

Este término **no depende de la velocidad**.  
Avances lento o rápido, atraviesas el mismo volumen de aire lleno de gotas.

---

## Volumen total de agua recibido

Sumando ambos aportes:

$$
V_{\text{total}} = V_{\text{arriba}} + V_{\text{frente}}
= A_{\text{arriba}}\, n_g\, v_g\, \frac{D}{v}
+ A_{\text{frente}}\, n_g\, D.
$$

Conclusión preliminar:  
**Correr (aumentar $v$) reduce el primer término, pero el segundo permanece constante.**

---

## Ejemplo numérico

Supongamos:

- $h = 1.7\ \text{m}$  
- $w = 0.5\ \text{m}$  
- $L_p = 0.5\ \text{m}$  
- $D = 100\ \text{m}$  
- $v_g = 4\ \text{m/s}$  
- $n_g = 100\ \text{gotas/m}^3$

Con estos valores:

$$
V_{\text{arriba}} = 0.5 \times 0.5 \times 100 \times 4 \times \frac{100}{v}
= \frac{10000}{v},
$$

$$
V_{\text{frente}} = 1.7 \times 0.5 \times 100 \times 100 = 8500.
$$

Tabla comparativa (en unidades arbitrarias):

| Velocidad | $V_{\text{arriba}}$ | $V_{\text{total}}$ |
|----------|---------------------|---------------------|
| 1 m/s (caminar) | 10000 | 18500 |
| 5 m/s (correr) | 2000 | 10500 |
| 10 m/s (sprint olímpico) | 1000 | 9500 |

Conclusión:  
**Correr reduce claramente la cantidad total de agua recibida.**

---

## ¿Y si la lluvia cae más rápido o más lento?

La velocidad de caída $v_g$ depende del tamaño de las gotas:

- Lluvia fina: $v_g \approx 1\ \text{m/s}$  
- Lluvia normal: $v_g \approx 4\ \text{m/s}$  
- Lluvia fuerte: $v_g \approx 7\ \text{m/s}$  

Si la intensidad total de lluvia es constante, el producto $n_g v_g$ se mantiene aproximadamente.

Entonces:

$$
V_{\text{arriba}} \propto \frac{1}{v}, \qquad V_{\text{frente}} \approx \text{constante}.
$$

La conclusión no cambia: **la clave es reducir el tiempo bajo la lluvia.**

---

## ¿Y si corres en la misma dirección del viento?

Si la lluvia tiene velocidad horizontal $v_{g,h}$ además de la vertical, la velocidad relativa entre persona y gotas es $|v - v_{g,h}|$.

El volumen total sería:

$$
V_{\text{total}}(v) =
A_{\text{arriba}} n_g v_g \frac{D}{v}
+ A_{\text{frente}} n_g |v - v_{g,h}| \frac{D}{v}.
$$

Si corres a la misma velocidad que la componente horizontal de la lluvia ($v = v_{g,h}$), entonces:

$$
V_{\text{total}}(v_{g,h}) =
A_{\text{arriba}} n_g v_g \frac{D}{v_{g,h}}.
$$

En ese punto, **la lluvia te cae verticalmente** en tu marco: ya no te mojas de frente.

---

# Conclusión: el tiempo es el factor clave

La lluvia no perdona, pero la física ayuda:  
**sí, te mojas menos si corres**, porque el agua que llega desde arriba disminuye proporcionalmente al tiempo de exposición, mientras que la que llega de frente apenas cambia.

En definitiva:

**Corre. La física (y tu secadora) te lo agradecerán.**
