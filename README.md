## Controle Fuzzy PD para Elevador

## Descrição do Projeto

Projeto implementa um sistema de controle PD baseado em lógica fuzzy para controlar a posição e a velocidade de um elevador. O objetivo é garantir uma operação segura e eficiente do elevador, permitindo o controle preciso de sua movimentação entre os andares.

![image](https://github.com/MarceloAbrantes/Trabalho-Elevador-Fuzzy/assets/99184020/c531d6ea-226c-4fb1-861b-e7c1257129e9)


## Estrutura do Edifício

-O edifício possui 11 andares e 36 metros de altura.

-O elevador começa na altura 4 metros.

-Vai até 32 metros

-Possui 9 andares com o terreo

## Etapas de controle Fuzzy
1. **Definição de Variáveis:** Primeiro, são definidas as variáveis fuzzy que serão usadas no sistema de controle: Erro, deltaErro e p_motor.

2. **Funções de Pertinência:** As funções de pertinência são definidas para classificar os valores das variáveis.
   
3. **Definição das Regras Fuzzy:** determinam como as variáveis de entrada (Erro e DeltaErro) se combinam para influenciar a variável de saída (p_motor).
   
5. **Controle:** inicializa as variáveis e executa o sistema fuzzy para controlar a posição do elevador.

## Informações sobre a Inicialização

- Nos primeiros 3 segundos, o motor acelera linearmente até 31,5% de sua potência nominal:
- Após os 3 segundos iniciais, o controle fuzzy ajusta continuamente a potência do motor com base no erro atual e na mudança do erro:
-Nesse caso controle reverso
  
## Interface Gráfica

Funções:

1. **simular_elevador(andarAtual, andarDeslocado):** 

-Inicia a simulação do movimento do elevador.

-Define a posição inicial do elevador e calcula o erro de altura inicial.

-Simula a aceleração do motor nos primeiros 3 segundos, onde a potência do motor aumenta linearmente até 31,5%.

- Usa controle fuzzy para ajustar continuamente a posição do elevador em relação ao andar desejado.

- Retorna um array posicao que registra a posição do elevador ao longo do tempo.


3. **plotar_grafico(posicao, setpoint):** Plota o movimento real do elevador em relação ao tempo, mostrando também o andar desejado.

-Plota um gráfico que mostra a posição real do elevador ao longo do tempo.

-Adiciona uma linha de referência (setpoint) indicando o andar desejado.
   
3. **chamar_elevador(andar):**
  
-Interface para chamar o elevador para um andar específico através de botões em uma interface gráfica.

-Atualiza dinamicamente o gráfico conforme o elevador se move em resposta aos comandos.
   
4. **tkinter:**
   
- Cria uma interface gráfica simples usando tkinter.
  
- Exibe botões para cada andar, permitindo que o usuário chame o elevador diretamente clicando no botão correspondente.

## Autor
Marcelo Henrique Souza Abrantes- GEC 1538
