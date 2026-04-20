# Integrales de línea complejas: Ejercicios propuestos

## Curva: segmentos rectos

### Ejercicio 1 (Básico)
Calcula  
$$\int_C (z + 1) \, dz$$  
donde $C$ es el segmento recto desde $z=0$ hasta $z=1+i$.

---

### Ejercicio 2 (Conjugado)
Calcula  
$$\int_C \overline{z} \, dz$$  
donde $C$ es el segmento recto desde $z=1$ hasta $z=2i$.

> Nota: $\overline{z}$ es el conjugado.

---

### Ejercicio 3 (Función cuadrática)
Calcula  
$$\int_C z^2 \, dz$$  
donde $C$ es el segmento recto desde $z=i$ hasta $z=2-i$.

---

### Ejercicio 4 (Exponencial real)
Calcula  
$$\int_C e^{z} \, dz$$  
donde $C$ es el segmento recto desde $z=0$ hasta $z=2$.

---

### Ejercicio 5 (Parte imaginaria)
Calcula  
$$\int_C \operatorname{Im}(z) \, dz$$  
donde $C$ es el segmento recto desde $z=1+i$ hasta $z=1+3i$.

---

### Ejercicio 6 (Eje real)
Calcula  
$$\int_C z \, dz$$  
donde $C$ es el segmento recto desde $z=-1$ hasta $z=1$ (sobre el eje real).

---

## Soluciones

<details>
<summary>Haz clic para ver las soluciones</summary>

### Solución 1

**Parametrización:**  
$z(t)=t(1+i),\quad t\in[0,1]$  
$z'(t)=1+i$

**Función sobre la curva:**  
$f(z(t))=t(1+i)+1=(1+t)+it$

**Integral:**  
$$\int_0^1[(1+t)+it](1+i)\,dt=(1+i)\int_0^1(1+t+it)\,dt$$  
$$=(1+i)\left[\int_0^1(1+t)dt+i\int_0^1 t\,dt\right]=(1+i)\left[\frac{3}{2}+i\cdot\frac{1}{2}\right]$$  
$$=(1+i)\left(\frac{3}{2}+\frac{i}{2}\right)=\frac{3}{2}+\frac{i}{2}+\frac{3i}{2}+\frac{i^2}{2}$$  
$$=\frac{3}{2}+2i-\frac{1}{2}=1+2i$$

**Resultado:** $\boxed{1+2i}$

---

### Solución 2

**Parametrización:**  
$z(t)=1+t(2i-1)=(1-t)+i(2t),\quad t\in[0,1]$  
$z'(t)=-1+2i$

**Función sobre la curva:**  
$f(z(t))=\overline{z(t)}=(1-t)-2it$

**Integral:**  
$$\int_0^1[(1-t)-2it](-1+2i)\,dt=(-1+2i)\int_0^1(1-t-2it)\,dt$$  
$$=(-1+2i)\left[\int_0^1(1-t)dt-2i\int_0^1 t\,dt\right]=(-1+2i)\left[\frac{1}{2}-2i\cdot\frac{1}{2}\right]$$  
$$=(-1+2i)\left(\frac{1}{2}-i\right)$$

Multiplicando:  
$(-1)(1/2)=-1/2$  
$(-1)(-i)=i$  
$(2i)(1/2)=i$  
$(2i)(-i)=-2i^2=2$

Suma: $-1/2+i+i+2=\frac{3}{2}+2i$

**Resultado:** $\boxed{\frac{3}{2}+2i}$

---

### Solución 3

**Parametrización:**  
$z(t)=i+t(2-i-i)=i+t(2-2i)=2t+i(1-2t),\quad t\in[0,1]$  
$z'(t)=2-2i$

**Función sobre la curva:**  
$f(z(t))=[2t+i(1-2t)]^2$

Desarrollamos:  
$a=2t,\ b=1-2t$  
$(a+ib)^2=a^2-b^2+2iab$  
$=4t^2-(1-4t+4t^2)+2i(2t)(1-2t)$  
$=4t^2-1+4t-4t^2+4it(1-2t)$  
$=(-1+4t)+4i(t-2t^2)$

**Integral:**  
$$\int_0^1[(-1+4t)+4i(t-2t^2)](2-2i)\,dt=(2-2i)\int_0^1[(-1+4t)+4i(t-2t^2)]\,dt$$

Parte real: $\int_0^1(-1+4t)dt=[-t+2t^2]_0^1=1$  
Parte imaginaria: $\int_0^1 4(t-2t^2)dt=4\left[\frac{t^2}{2}-\frac{2t^3}{3}\right]_0^1=4\left(\frac{1}{2}-\frac{2}{3}\right)=-\frac{2}{3}$

Suma: $1-\frac{2}{3}i$

Multiplicamos por $(2-2i)$:  
$(2-2i)\left(1-\frac{2}{3}i\right)=2-\frac{4}{3}i-2i+\frac{4}{3}i^2$  
$=2-\frac{10}{3}i-\frac{4}{3}=\frac{2}{3}-\frac{10}{3}i$

**Resultado:** $\boxed{\frac{2}{3}-\frac{10}{3}i}$

---

### Solución 4

**Parametrización:**  
$z(t)=2t,\quad t\in[0,1]$  
$z'(t)=2$

**Función sobre la curva:**  
$f(z(t))=e^{2t}$

**Integral:**  
$$\int_0^1 e^{2t}\cdot 2\,dt=2\cdot\frac{e^{2t}}{2}\Big|_0^1=e^2-1$$

**Resultado:** $\boxed{e^2-1}$ (real)

---

### Solución 5

**Parametrización:**  
$z(t)=1+i(1+2t),\quad t\in[0,1]$  
Parte imaginaria: $\operatorname{Im}(z)=1+2t$  
$z'(t)=2i$

**Integral:**  
$$\int_0^1(1+2t)(2i)\,dt=2i\int_0^1(1+2t)dt=2i[t+t^2]_0^1=2i(1+1)=4i$$

**Resultado:** $\boxed{4i}$

---

### Solución 6

**Parametrización:**  
$z(t)=t,\quad t\in[-1,1]$  
$z'(t)=1$  
$f(z(t))=t$

**Integral:**  
$$\int_{-1}^1 t\,dt=0$$  
(por simetría: función impar en intervalo simétrico)

**Resultado:** $\boxed{0}$

</details>
