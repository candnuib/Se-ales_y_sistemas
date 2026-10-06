Transformacion en tiempo.

x (n) -> x (n - k) donde k = entero

Si K es positivo resulta en un atraso de k muestras.

Si K es negativo resulta en un adelanto de k muestras.

Señal original:

<img width="594" height="457" alt="image" src="https://github.com/user-attachments/assets/79c1028f-24f6-41ee-81d5-c728fb00f398" />

Caso -> k = 3 -> Por lo tanto x (n - 3) ->  Atraso de 3 muestras.

<img width="599" height="457" alt="image" src="https://github.com/user-attachments/assets/0a5b928b-14f4-45f6-9792-acc7e49586e6" />

Caso -> k = -2 -> Por lo tanto x (n - (-2)) ->  Adelanto de 2 muestras.

<img width="603" height="462" alt="image" src="https://github.com/user-attachments/assets/118d1db0-a4f9-4d26-9217-e1d76200ad96" />

Nota: Solo se puede adelantar si la señal esta almacenada en memoria, en tiempo real no.

TDk [X(n)] = x(n - k)

*   Reflexion. (Folding Displacement)

FD[x(n)] = x(-n)

Señal original: x(n)

<img width="579" height="458" alt="image" src="https://github.com/user-attachments/assets/58942870-c270-4152-b732-7159336014e7" />

Señal refeljada: x(-n)

<img width="584" height="465" alt="image" src="https://github.com/user-attachments/assets/bbe8c0a6-6ecf-41ec-b927-32c2cfa56edb" />

DESPLAZAMIENTO EN TIEMPO Y REFLEXION TEMPORAL.

No son conmutativas

TDk[FD[x(n)]] ≠ FD[TDk[x(n)]]

Ejemplo: Sea la señal x(n) con una K = 2

<img width="581" height="437" alt="image" src="https://github.com/user-attachments/assets/f6b52310-9d43-4b7b-92ee-d1a6cee58b60" />

El el primer caso se empezara por FD[x(n)]

<img width="598" height="465" alt="image" src="https://github.com/user-attachments/assets/1234684d-89f2-4306-b349-010891d4db63" />

Despues a el resultado se le aplica un atraso de 2.

TD2 [FD[x(n)]] = x(n - k); K=2

<img width="596" height="449" alt="image" src="https://github.com/user-attachments/assets/2c79baed-265f-4894-b4eb-66dd025b82ff" />

En el segundo caso se empezara por TD2[x(n)] 

<img width="590" height="449" alt="image" src="https://github.com/user-attachments/assets/dbd892d3-7ceb-4de7-98cb-3d35c5b8def8" />

Despues a el resultado se le aplicara la reflexion FD[TD2[x(n)]]

<img width="617" height="476" alt="image" src="https://github.com/user-attachments/assets/f77f0ad0-d4f8-47f1-9a30-1f3f604904f9" />

