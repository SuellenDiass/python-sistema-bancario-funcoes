<p> <h1 align="center">Sistema Bancário com Funções Python</h1></p>


Esse projeto trata-se de um desfio proposto pelo mentor Guilherme Carvalho do curso Formação Python Developer da Dio.me, onde nesse desafio, a gente pôde melhorar um Sistema Bancário que já estava pronto usando funções em Python. A ideia era deixar o sistema mais organizado e eficiente, então criamos funções especiais para as operações de depósito, saque e extrato. A parte legal foi que também pudemos reorganizar o código que já existia, dividindo ele em pedaços menores que podem ser usados de novo em outras partes do sistema. Isso deixa tudo mais fácil de cuidar e entender. Aprendemos a usar conceitos avançados de programação e a criar soluções mais  eficientes com Python. Foi bem legal!


Explicação da estrutura do código:


```python
import textwrap

def menu():
    # ... (definição do menu)
    return input(textwrap.dedent(menu))

def depositar(saldo, valor, extrato, /):
    # ... (lógica para depósito)
    return saldo, extrato

def sacar(*, saldo, valor, extrato, limite, numero_saques, limite_saques):
    # ... (lógica para saque)
    return saldo, extrato

def exibir_extrato(saldo, /, *, extrato):
    # ... (exibir extrato)
    
def criar_usuario(usuarios):
    # ... (criar usuário)
    
def filtrar_usuario(cpf, usuarios):
    # ... (filtrar usuário)
    
def criar_conta(agencia, numero_conta, usuarios):
    # ... (criar conta)
    
def listar_contas(contas):
    # ... (listar contas)

def main():
    # ... (inicialização de variáveis)
    
    while True:
        opcao = menu()
        if opcao == "d":
            # ... (chamada para depósito)
        elif opcao == "s":
            # ... (chamada para saque)
        elif opcao == "e":
            # ... (chamada para exibir extrato)
        elif opcao == "nu":
            # ... (chamada para criar usuário)
        elif opcao == "nc":
            # ... (chamada para criar conta)
        elif opcao == "lc":
            # ... (chamada para listar contas)
        elif opcao == "q":
            break
        else:
            print("Operação inválida, por favor selecione novamente a operação desejada.")

main()
```

Uma descrição da estrutura e funcionamento do código:

1. **Importação de Módulos**: O código começa importando o módulo `textwrap`, que é usado para formatar e exibir texto de forma adequada.

2. **Definição de Funções**:
   - `menu()`: Essa função exibe o menu para o usuário e retorna a opção escolhida.
   - `depositar(saldo, valor, extrato, /)`: Realiza a operação de depósito e atualiza o saldo e extrato.
   - `sacar(*, saldo, valor, extrato, limite, numero_saques, limite_saques)`: Realiza a operação de saque, verificando várias condições antes de executar a transação.
   - `exibir_extrato(saldo, /, *, extrato)`: Exibe o extrato da conta, incluindo o saldo e as transações realizadas.
   - `criar_usuario(usuarios)`: Cria um novo usuário com informações fornecidas pelo usuário.
   - `filtrar_usuario(cpf, usuarios)`: Filtra um usuário por CPF na lista de usuários.
   - `criar_conta(agencia, numero_conta, usuarios)`: Cria uma nova conta associada a um usuário existente.
   - `listar_contas(contas)`: Exibe uma lista das contas existentes.

3. **Função `main()`**: Esta é a função principal do programa. Inicializa várias variáveis necessárias para controlar informações como saldo, limite, extrato, número de saques, lista de usuários e lista de contas.

4. **Loop Principal**: O loop `while True` é executado continuamente até que o usuário escolha sair (`opcao == "q"`). Dentro deste loop, o programa exibe o menu, coleta a opção do usuário e chama a função correspondente com base na opção selecionada.

Cada função é projetada para executar uma tarefa específica e modularizar o código, o que torna o programa mais legível e mais fácil de manter. O código segue uma estrutura organizada para gerenciar as operações bancárias e interações com o usuário.



#### Curso Formação Python Developer da Dio.me administrado pelo mentor Guilherme Carvalho/Python Consultant, Oak Solution

[DIO](https://www.dio.me/).