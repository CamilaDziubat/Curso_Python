## Banco Simples - README
Este é um projeto de um sistema bancário simples implementado em Python. O objetivo do projeto é simular algumas funcionalidades de um banco, como a criação de usuários e contas, depósitos, saques, extratos e listagem de contas, por meio de um menu interativo no terminal. O código foi desenvolvido de forma a ser simples e didático, utilizando funções para realizar operações como depósitos, saques, criação de contas e exibição de extratos.

## Funcionalidades
O sistema oferece as seguintes funcionalidades:

Depositar: Permite o usuário realizar um depósito na conta, aumentando o saldo da conta e gerando um extrato.

Sacar: Permite o usuário realizar um saque, verificando se o saldo é suficiente, se o valor do saque está dentro do limite de saque e se o número máximo de saques foi atingido.

Extrato: Exibe o extrato da conta, com todos os depósitos e saques realizados, bem como o saldo atual da conta.

Criar Usuário: Permite a criação de um novo usuário com informações como nome, CPF, data de nascimento e endereço.

Criar Conta: Cria uma nova conta bancária associada a um usuário já cadastrado no sistema, atribuindo um número de conta e uma agência.

Listar Contas: Exibe uma lista de todas as contas criadas, mostrando a agência, número da conta e o nome do titular da conta.

Sair: Encerra o programa.

## Estrutura do Código
Funções:

menu(): Exibe o menu de opções para o usuário escolher a operação desejada.

depositar(saldo, valor, extrato): Realiza um depósito e atualiza o saldo e o extrato.

sacar(saldo, valor, extrato, limite, numero_saques, limite_saques): Realiza um saque e verifica se é possível realizar a operação, atualizando o saldo e o extrato.

exibir_extrato(saldo, extrato): Exibe o extrato da conta com todas as movimentações realizadas.

criar_usuario(usuarios): Cria um novo usuário, registrando informações como nome, CPF, data de nascimento e endereço.

filtrar_usuario(cpf, usuarios): Filtra o usuário pelo CPF, retornando o usuário caso encontrado.

criar_conta(agencia, numero_conta, usuarios): Cria uma nova conta associada a um usuário e atribui um número de conta.

listar_contas(contas): Exibe todas as contas cadastradas no sistema.

Loop Principal (main()): O programa entra em um loop contínuo até que o usuário escolha a opção de sair (q). Dentro desse loop, ele permite que o usuário interaja com o menu e execute as funcionalidades disponíveis.

## Como Usar
Clone o repositório: Clone este repositório em sua máquina utilizando o seguinte comando:

bash
Copiar
git clone https://github.com/seuusuario/nome-do-repositorio.git
Execute o programa: Navegue até o diretório do repositório e execute o arquivo Python:

nginx
Copiar
python banco_simples.py
Menu de opções: Após executar o programa, um menu será exibido com as opções disponíveis:

d: Depositar

s: Sacar

e: Extrato

nc: Nova conta

lc: Listar contas

nu: Novo usuário

q: Sair

Interação: O programa solicitará as informações necessárias para cada operação, como valores de depósito e saque, CPF do usuário, entre outros. Basta seguir as instruções no terminal.

## Requisitos
Python 3.x
