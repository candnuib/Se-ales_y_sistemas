La teoría detrás del Submuestreo (Downsampling)

Cuando haces $y(n) = x(μ n)$ con un entero $\mu > 1$, estás realizando una compresión temporal o diezmado (downsampling).

 $\mu = 2$, 
x(n) =Xa(nT)

    Ejemplo: tenemos μ = 2 la señal es y(n) = x(2n). Esto significa que:

    
 y(n) = x(2n) = x(2Tn)

• Si $n = 0$, $y(0) = x(0)$
    
• Si $n = 1$, $y(1) = x(2)$
    
• Si $n = 2$, $y(2) = x(4)$


    
Las muestras impares de la señal original desaparecen. Se esta tirando a la basura la mitad de la información. La señal se "comprime" porque ocurre el doble de rápido.

 • Al descartar muestras, la nueva frecuencia de muestreo cae a la mitad: $f_s' = f_s / 2$.
    
 • Como el periodo de muestreo es el inverso de la frecuencia ($T = 1/f_s$), el tiempo entre las muestras que conservas se duplica. El nuevo periodo es $2T$.

Nyquist-Shannon

El teorema de Nyquist establece que tu frecuencia de muestreo debe ser estrictamente mayor al doble de la frecuencia máxima de tu señal: $f_s \ge 2f_{max}$.

Como el downsampling reduce tu $f_s$ a la mitad, corres el riesgo de violar este teorema. Si tu nueva frecuencia $f_s'$ cae por debajo de $2f_{max}$, las frecuencias altas se "disfrazarán" de frecuencias bajas, un fenómeno destructivo llamado Aliasing (solapamiento).

