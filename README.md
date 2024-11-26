# Mandelbrot
## Números complexos:
![Numeros complexos](complexNumbers.png)

## Fórmula Mandelbrot
![Formula](formula.png)

### Exemplo:
Z0 = 0;<br>
z1 = (Z0)^2 + 1 = 1;<br>
z2 = (z1)^2 + 1 = 2;<br>
z3 = (z2)^2 + 1 = 5;<br>
z4 = (z3)^2 + 1 = 26<br>
Não está no conjunto<br>
<br>
Z0 = 0;<br>
z1 = (Z0)^2 - 1 = - 1;<br>
z2 = (Z1)^2 - 1 = 0;<br>
z3 = (Z2)^2 - 1 = - 1;<br>
Está no conjunto<br>

## Configurações do processador:
12th Gen Intel(R) Core(TM) i5-12500H 3.10 GHz - 12 núcleos

## Mudanças realizadas no código:
- Mudança simples do código main para facilitar a geração de uma média do tempo de execução gasto para gerar uma imagem, tanto para single como para multi-thread.
![gif da mudança](gif.gif)

## Resultados obtidos:
### Executando sem alterar os parâmetros:
#### Resultados:
| Threads | Tempo em ms | Speedup      |
|---------|-------------|--------------|
| 1       | 4069        | 0            |
| 2       | 1735        | 2.345244957  |
| 3       | 1713        | 2.375364857  |
| 4       | 1145        | 3.55371179   |
| 5       | 1080        | 3.767592593  |
| 6       | 856         | 4.753504673  |
| 7       | 788         | 5.163705584  |
| 8       | 681         | 5.975036711  |
#### Gráfico:
![gráfico dos tempos de execução](grafico1.png)

### Executando com 3k interações:
#### Resultados:
| Threads | Tempo em ms | Speedup      |
|---------|-------------|--------------|
| 1       | 11868       | 0            |
| 2       | 5111        | 2.322050479  |
| 3       | 5060        | 2.345454545  |
| 4       | 3320        | 3.574698795  |
| 5       | 3108        | 3.818532819  |
| 6       | 2510        | 4.728286853  |
| 7       | 2288        | 5.187062937  |
| 8       | 1995        | 5.94887218   |

#### Gráfico:
![gráfico dos tempos de execução](grafico2.png)

## Referências:
[Sounds of the Madelbrot Set](https://www.youtube.com/watch?v=GiAj9WW1OfQ&t=354s)<br>
[What's so special about the Mandelbrot Set? - Numberphile](https://www.youtube.com/watch?v=FFftmWSzgmk)