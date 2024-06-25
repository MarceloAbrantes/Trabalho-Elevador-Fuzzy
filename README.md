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

## Inicialização

- Nos primeiros 3 segundos, o motor acelera linearmente até 31,5% de sua potência nominal:
- Após os 3 segundos iniciais, o controle fuzzy ajusta continuamente a potência do motor com base no erro atual e na mudança do erro:
-Nesse caso controle reverso
  
## Interface Gráfica

## Autor
Marcelo Henrique Souza Abrantes- GEC 1538
