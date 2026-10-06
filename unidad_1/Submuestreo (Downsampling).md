La teoría detrás del Submuestreo (Downsampling)

Cuando haces $y(n) = x(\mu n)$ con un entero $\mu > 1$, estás realizando una compresión temporal o diezmado (downsampling).

Si $\mu = 2$, tu nueva señal es $y(n) = x(2n)$. Esto significa que:

    • Si $n = 0$, $y(0) = x(0)$
    
    • Si $n = 1$, $y(1) = x(2)$
    
    • Si $n = 2$, $y(2) = x(4)$
    
Como ves, las muestras impares de la señal original desaparecen. Literalmente estás tirando a la basura la mitad de la información. La señal se "comprime" porque ocurre el doble de rápido.
Corrección sobre el tiempo $T$ y la frecuencia:
Mencionas que equivale a $1/2 T$ en vez de $1/T$. Es exactamente al revés:
    • Al descartar muestras, tu nueva frecuencia de muestreo cae a la mitad: $f_s' = f_s / 2$.
    • Como el periodo de muestreo es el inverso de la frecuencia ($T = 1/f_s$), el tiempo entre las muestras que conservas se duplica. Tu nuevo periodo es $2T$.
¿Por qué te mencionan a Nyquist-Shannon?
El teorema de Nyquist establece que tu frecuencia de muestreo debe ser estrictamente mayor al doble de la frecuencia máxima de tu señal: $f_s \ge 2f_{max}$. (A veces se añade un $+1$ o un margen en la práctica para los filtros, pero la base teórica es el doble).
Como el downsampling reduce tu $f_s$ a la mitad, corres el riesgo de violar este teorema. Si tu nueva frecuencia $f_s'$ cae por debajo de $2f_{max}$, las frecuencias altas se "disfrazarán" de frecuencias bajas, un fenómeno destructivo llamado Aliasing (solapamiento).

