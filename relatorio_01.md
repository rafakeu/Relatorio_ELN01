# Relatório 01

 Estudo das características de um amplificador operacional não ideal e de um circuito amplificador subtrator. 

 >Foram Utilizados os modelos de Ampop LM324N e TL082 nas simulações.

## Seguidor de Tensão

Idealmente temos:

Vout = Vin

Circuito simulado:

![Esquemático Buffer](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_esquematico.png)

E como resultado da simulação

Para o LM324N:

![Buffer LM324N](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_LM324.png)

Podemos observar que Vout não possui o mesmo valor de Vin, considerando que o período da onda é de 1ms temos que a tensão de pico positiva será em t = 0,25ms e a tensão máxima negativa será em t = 0,75ms.

As medidas obtidas nesse pontos são:

Tensão de pico posiva:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_Buffer_Vpos.png)

E tensão de pico negativa:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_Buffer_Vneg.png)


Para o TL082:

![Buffer TL082](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_TL082.png)

Comparando os resultados:

\*Comentario\*

## Amplificador inversor

Circuito simulado:

![Esquemático Amplificador inversor]()

E como resultado da simulação

Para o LM324N:

![Amplificador inversor LM324N]()

Para o TL082:

![Amplificador inversor TL082]()

\*Comentario\*

## Amplificador não-inversor


Circuito simulado:

![Esquemático Amplificador não-inversor]()

E como resultado da simulação

Para o LM324N:

![Amplificador não-inversor LM324N]()

Para o TL082:

![Amplificador não-inversor TL082]()

\*Comentario\*

## Amplificador subtrator


Circuito simulado:

![Esquemático Amplificador subtrator]()

E como resultado da simulação

Para o LM324N:

![Amplificador subtrator LM324N]()

Para o TL082:

![Amplificador subtrator TL082]()

\*Comentario\*
