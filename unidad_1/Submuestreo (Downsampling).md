La teoría detrás del Submuestreo o escalado tempotal  (Downsampling) 

Se define fs  

T = 1 / fs

Teorema de Nyquist-Shannon

fs = 2 f + 1

Submuestrear o escalar el tiempo emplica reemplazar ¨n" en una señal por  (μ n) donde μ = entero.

y(n) = x(μ n) 

x(n) = Xa(n T)

Ejemplo: tenemos μ = 2.

 y(n) = x(2n) = x(2Tn)

• Si $n = 0$, $y(0) = x(0)$
    
• Si $n = 1$, $y(1) = x(2)$
    
• Si $n = 2$, $y(2) = x(4)$

• Si $n = -1$, $y(-1) = x(-2)$
    
• Si $n = -2$, $y(-2) = x(-4)$

x(n)

<img width="578" height="443" alt="image" src="https://github.com/user-attachments/assets/ccec4602-c9a6-4143-99fe-2c48a082a750" />

y(n) = x(2n)  

<img width="590" height="456" alt="image" src="https://github.com/user-attachments/assets/124c1a0a-c24d-4c31-9529-81c5d9b2dac1" />

Las muestras impares de la señal original desaparecen. Se esta tirando a la basura la mitad de la información. La señal se "comprime" porque ocurre el doble de rápido.

