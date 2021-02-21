# SnakeIA

### Neural Network

Cada snake contém uma rede neural. A rede neural tem uma camada de entrada de 24 neurônios, 2 camadas ocultas de 8 neurônios e uma camada de saída de 4 neurônios. Observação: a rede agora pode ser personalizada com o número de camadas ocultas e também com o número de neurônios nas camadas ocultas.

### Visão
---
A snake pode ver em 8 direções. Em cada uma dessas direções, a cobra procura 3 coisas:

* Distância até a comida 
* Distância até o seu corpo
* Distância até a parede

3 x 8 direções = 24 inputs. Os 4 outputs são simplesmente as direções em que a snake pode se mover.

### Evolução
---
A cada geração, é criada uma população de 2.000 snakes. Sempre que uma snake morre verificamos se sua pontuação foi melhor , se sim, salvamos.A melhor snake da geração sofre a mutação. Isso é repetido para criar uma nova população de 2.000 novas snakes.


### Pontuação
---
A pontuação de uma cobra depende de quanto a snake permanece viva. No entanto, existe a possibilidade de que uma snake possa desenvolver uma estratégia em que ela faz um loop em um determinado padrão e nunca morre. Para evitar isso, cada snake pode realizar 200 movimentos. Cada vez que ele come, esse contador é resetado. Isso significa que as cobras que evoluíram para entrar em loops acabarão morrendo.

### Crossover  e mutação
---
Quando termina o ciclo da geração a melhor snake é  selecionada para reprodução, o que acontece é que os cérebros das snakes se cruzam. O que isso significa é que parte do cérebro de um dos pais é misturada com parte dos segundos pais e o cérebro resultante é atribuído ao filho. Após o cruzamento, o cérebro também sofre mutação de acordo com uma taxa de mutação. A taxa de mutação determina quanto do cérebro será alterado aleatoriamente.
