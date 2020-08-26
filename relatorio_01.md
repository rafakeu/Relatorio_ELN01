# Relatório 01

 Estudo das características de um amplificador operacional não ideal e de um circuito amplificador subtrator. 

 >Foram Utilizados os modelos SPICE dos Ampops LM324N e TL082 nas simulações.

## Seguidor de Tensão

Idealmente temos:

Vout = Vin

Circuito simulado:

![Esquemático Buffer](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_esquematico.png)

E como resultado da simulação,

para o LM324N:

![Buffer LM324N](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_LM324.png)

Podemos observar que Vout não possui o mesmo valor de Vin, considerando que o período da onda é de 1ms temos que a tensão de pico positiva será em t = 0,25ms e a tensão máxima negativa será em t = 0,75ms.

As medidas obtidas nesse pontos são:

tensão de pico positiva:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_Buffer_Vpos.png)

E tensão de pico negativa:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_Buffer_Vneg.png)


para o TL082:

![Buffer TL082](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_TL082.png)

A diferença entre Vin e Vout representa um valor despresível ao comparar com a dimensão de Vin e Vout. Então podemos dizer: Vin = Vout.    


![Buffer TL082](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Buffer_comparacao.png)

As divergências encontradas entre os valores calculados e simulados pode ser explicada pela presença de tensões de offset, devido a imperfeições CC do ampop.  

## Amplificador inversor

Circuito Ideal:

Vout = - (R2/R1) * Vin

Com R2 = 20k e R1 = 2k

Vout = 10 * Vin

Circuito simulado:

![Esquemático Amplificador inversor](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/inversor_esquematico.png)

E como resultado da simulação

Para o LM324N:

![Amplificador inversor LM324N](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/inversor_LM324N.png)

para Vin = 0,5 v obtivemos:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_inversor_Vpos.png)

e para Vin = -0,5 v:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/LM324_inversor_Vneg.png)

A saturação positiva ocorreu apartir de Vin = 1,08 v: 


![Saturação Positiva](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/sat_pos_LM324N.png)

Onde Vout = 10,76 v representando 90% do valor de alimentação.

Já a saturação negativa ocorreu apartir de Vin = 1,14 v:

![Saturação negativa](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/Sat_neg_LM324N.png)

Onde Vout = -11,32 v representando 94% do valor de alimentação.

Para o TL082:

![Amplificador inversor TL082](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/inversor_TL082.png)


para Vin = 0,5 v obtivemos:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/TL082_inversor_Vpos.png)

e para Vin = -0,5 v:

![Medidas obtidas](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/TL082_inversor_Vneg.png)

Apartir do valor de Vin = 1,05 v é possivel verificar que há uma saturação observando um pequeno ceifamento na forma de onda: 

![Ceifamento](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/inversor_TL082_sat.png)

Vout satura, e assume o valor de +/-10,37 V o que representa 86% do valor de alimentação.

imperfeição:

![Imperfeição](https://github.com/rafakeu/Relatorio_ELN01/blob/master/img/inversor_LM324N_imperfeicao.png)

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

