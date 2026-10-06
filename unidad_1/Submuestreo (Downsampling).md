La teoría detrás del Submuestreo o escalado tempotal  (Downsampling) 

Se define f_s ($T = 1/F_s$),}.

Cuando haces $y(n) = x(μ n)$ con un entero $\mu > 1$, estás realizando una compresión temporal o diezmado (downsampling).

 $\mu = 2$, 
x(n) =Xa(nT)

Ejemplo: tenemos μ = 2.

 y(n) = x(2n) = x(2Tn)

• Si $n = 0$, $y(0) = x(0)$
    
• Si $n = 1$, $y(1) = x(2)$
    
• Si $n = 2$, $y(2) = x(4)$

x(n)

<img width="578" height="443" alt="image" src="https://github.com/user-attachments/assets/ccec4602-c9a6-4143-99fe-2c48a082a750" />

y(n) = x(2n)  

<img width="590" height="456" alt="image" src="https://github.com/user-attachments/assets/124c1a0a-c24d-4c31-9529-81c5d9b2dac1" />

Las muestras impares de la señal original desaparecen. Se esta tirando a la basura la mitad de la información. La señal se "comprime" porque ocurre el doble de rápido.

 • Al descartar muestras, la nueva frecuencia de muestreo cae a la mitad: $f_s' = f_s / 2$.
    
 • Como el periodo de muestreo es el inverso de la frecuencia ($T = 1/f_s$), el tiempo entre las muestras que conservas se duplica. El nuevo periodo es $2T$.

Nyquist-Shannon

El teorema de Nyquist establece que tu frecuencia de muestreo debe ser estrictamente mayor al doble de la frecuencia máxima de tu señal: $f_s \ge 2f_{max}$.

Como el downsampling reduce tu $f_s$ a la mitad, corres el riesgo de violar este teorema. Si tu nueva frecuencia $f_s'$ cae por debajo de $2f_{max}$, las frecuencias altas se "disfrazarán" de frecuencias bajas, un fenómeno destructivo llamado Aliasing (solapamiento).

