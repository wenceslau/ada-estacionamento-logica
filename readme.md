# ADA Estacionamento - Logica de Programação

## Descrição
Projeto de estacionamento para a disciplina de Laboratório de Programação.

---
## Objetivo

- Aplicar os conceitos de lógica de programação em um projeto prático.  
- Usar estruturas de controle, estruturas de repetição e arrays.  
- Fazer cálculos matemáticos simples e medianos com os tipos primitivos do Java.  
- Usar o conceito de métodos para separar funcionalidades.  
- Usar a API java.time para manipulação de datas e horas.   
- Ler e interpretar enunciados.

---
## Enunciado

### $${\color{red}Requisitos funcionais}$$
Criação de um sistema de estacionamento para controlar veículos em um estacionamento. 

O sistema deve ser capaz de:

- Permitir a entrada de veículos no estacionamento
- Permitir a saída de veículos do estacionamento
- Controlar o tempo de permanência de cada veículo no estacionamento
- Controlar a lotação do estacionamento
- Calcular o valor a ser pago pelo cliente
- Exibir um relatório com as informações de todos os veículos que passaram pelo estacionamento

### $${\color{red}Regras de negócio}$$

> **RN1** - O estacionamento possui um limite de vagas que deve ser informado no momento da inicialização.

> **RN2** - O estacionamento não deve permitir a entrada de veículos quando estiver lotado.

> **RN3** - O estacionamento possui um valor fixo de R$ 5,00 para a primeira hora e R$ 6,00 para cada hora adicional.
>
> - De 0 a 5 minutos não é cobrado nenhum valor.
>
> - Acima de 5 minutos é cobrado o valor de uma hora.
>
> - Acima de 1 hora é cobrado o valor de uma hora e mais o valor da hora adicional. 
> - Exemplo 1: 1h e 4 minutos = R$ 5,00 (1 hora) + R$ 6,00 (4 minutos) = R$ 11,00
> - Exemplo 2: 1h e 59 minutos = R% 5,00 (1 horas) + R$ 6,00 (59 minuto) = R$ 11,00
> - Exemplo 3: 2h e 1 minuto = R$ 5,00 (1 hora) + R$ 6,00 (1 hora) + R$ 6,00 (1 minuto) = R$ 17,00
             
### $${\color{red}Comportamento}$$

- O sistema deve ser capaz de identificar se o estacionamento está lotado


- Para cada veículo que entrar no estacionamento, o sistema deve solicitar a placa do veículo


- O sistema deve ser capaz de identificar se o veículo já está no estacionamento


- Para o veiculo que entrar no estacionamento, exibir a mensagem:
    > Entrada do veículo placa: XXX-0000 realizada.

- Para o veiculo que sair do estacionamento, exibir a mensagem:

    > Saída do veículo placa: XXX-0000. Tempo de permanência: X minutos. Valor a pagar: Z,00

- Apos o registro de entrada ou saida de um veículo e após exibir a mensagem correspondente
o sistema deve exibir um relatório com os veículos que estão no estacionamento e os que já saíram.

  > VEÍCULOS ESTACIONADOS:
  > 
  > Placa CCC-1234 	 Hora de entrada: dd/MM/yyyy HH:mm:ss.  
  > Placa AAA-1234 	 Hora de entrada: dd/MM/yyyy HH:mm:ss.
  >   
  > REGISTROS DE SAÍDAS:
  > 
  > Placa BBB-1234 - tempo permanência: X minutos - valor cobrado: X.XX

### $${\color{red}Estrutura do projeto}$$

O projeto deve ser construído em Java em uma única classe e métodos estáticos.  
O sistema deve exibir um menu com as opções:

    1 - Registrar placa de veículo
    2 - Sair

Para armazenar os dados o sistema deve usar **Arrays**.  
Para a entrada de dados o sistema deve usar a classe **Scanner**.  
Para controlar de tempo o sistema deve usar a **API java.time do Java**.  
Para o cálculo de valor a ser pago pode se usar a **API java.math do Java**, ou fazer o cálculo manualmente.

### $${\color{red}Entrega}$$
O projeto deve ser entregue via LMS em um arquivo compactado com o nome do aluno.

### $${\color{red}Demonstração}$$

![img.png](img.png)

![img_1.png](img_1.png)1

![img_2.png](img_2.png)
