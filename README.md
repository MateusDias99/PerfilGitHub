# **|Mateus Dias|**

<i>Bem-vindo ao meu perfil! Sou apaixonado por resolver problemas através da programação e estou sempre buscando aprender novas tecnologias.

Às vezes, as soluções inesperadas são vistas como características em vez de erros 🤓</i>

## **_➡Tecnologias usadas_**

  [✔️]HTML
   [✔️]CSS
    [✔️]Python
     [✔️]Django
      [✔️]C#  

## **_➡Projetos_**
      
 ✔️ _HTML_ 
~~~
Código em Breve
~~~
 ✔️ _CSS_
~~~
Código em Breve
~~~
 ✔️ _Python_
~~~

Código em Atualizações....

lista_super_mercado = []

while True:
    print("Seja bem-vindo ao Controle de lista para Compras...")
    Produto = input("Digite o nome do produto para acresecentar ou remover:  ")
    Digitado = input("Digite a opção [1] Excluir 1 produto  [2] Acrescentar [3] Verificar [5] Excluir Quantidade [4] Fechar: ")

    try:
        Digitado = int(Digitado)
        if Digitado == 1:
            if lista_super_mercado:
                item_removido = lista_super_mercado.pop(0)
                print(f"Produto {item_removido} removido.")
                print(lista_super_mercado)
            else:
                print("A lista está vazia. Nenhum item para remover.")
        elif Digitado == 2:
            lista_super_mercado.append(Produto)
            print(f"Produto {Produto} adicionado.")
            quantidade = int(input(f"Adicione a quantidade: "))
            lista_super_mercado.append(quantidade)
            print(lista_super_mercado)
        elif Digitado == 3:
            print(lista_super_mercado)
        elif Digitado == 4:
            print("Fechando o Controle de lista para Compras. Até logo!")
            break
        elif int(Digitado) == 5:
            lista_super_mercado.clear()
            print("Todos os itens foram removidos.")
            print(lista_super_mercado)
        else:
            print("Opção inválida. Digite um número entre 1 e 4.")

    except ValueError:
        print("Digite um número válido.")
        continue
~~~
 ✔️ _Django_ 
~~~
Código em Breve
~~~
 ✔️ _C#_ 
 Em teste...
~~~
using System;

namespace App
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Variáveis.
            char cafe = ('\u2615');
            char coracao = ('\u2764');

            //  Painel do Senai
            Console.WriteLine($"║{cafe} Exercícios Senai {coracao} ║");

            // Calculadora
            Console.WriteLine("╔════════════════════════════╗");
            Console.WriteLine("║      Calculadora          ║");
            Console.WriteLine("╠════════════════════════════╣");
            Console.WriteLine("║       [7] [8] [9]   [÷]    ║");
            Console.WriteLine("║       [4] [5] [6]   [×]    ║");
            Console.WriteLine("║       [1] [2] [3]   [-]    ║");
            Console.WriteLine("║       [0] [.] [=]   [+]    ║");
            Console.WriteLine("╚════════════════════════════╝");

            // Entrada da decisão do usuário
            Console.Write("Digite o número da operação que deseja realizar [1] Baskara ou [2] Operações de: (+-*/)\nDigite:");
            double decisaoUsuario;
            if (double.TryParse(Console.ReadLine(), out decisaoUsuario))
            {
                if (decisaoUsuario == 1)
                {
                    int loop = 0;

                    while (loop < 3)
                    {
                        Console.WriteLine("Lembre-se de ter a fórmula de Baskara em mãos!");
                        Console.Write($"Digite o valor  do  número  B: ");
                        double coeficienteB;
                        if (!double.TryParse(Console.ReadLine(), out coeficienteB))
                        {
                            Console.WriteLine("Valor inválido para B. Por favor, insira um número válido.");
                            ++loop;
                            
                        }

                        Console.Write($"Digite o valor de A: ");
                        double coeficienteA;
                        if (!double.TryParse(Console.ReadLine(), out coeficienteA))
                        {
                            Console.WriteLine($"Valor inválido para A. Por favor, insira um número válido, você tem ({3 - loop}) tentativas restantes.");
                            ++loop;
                            
                        }

                        Console.Write($"Digite o valor de C: ");
                        double coeficienteC;
                        if (!double.TryParse(Console.ReadLine(), out coeficienteC))
                        {
                            Console.WriteLine($"Valor inválido para C. Por favor, insira um número válido, você tem ({3 - loop}) tentativas restantes.");
                            ++loop;
                            
                        }

                        double delta = Math.Pow(-coeficienteB, 2) - 4 * coeficienteA * coeficienteC;

                        if (delta < 0)
                        {
                            Console.WriteLine($"A equação de delta é menor que 0, onde o resultado de delta é  {delta}, sendo assim a operação não possui um valor real");
                            continue;
                        }
                        else
                        {
                            double raiz1 = (-coeficienteB + Math.Sqrt(delta)) / (2 * coeficienteA);
                            double raiz2 = (-coeficienteB - Math.Sqrt(delta)) / (2 * coeficienteA);

                            Console.WriteLine($"As raízes da equação são: {raiz1} e {raiz2}");
                        }

                        Console.WriteLine("\nPressione qualquer tecla para continuar...");
                        Console.ReadKey(true);
                        break;
                    }
                }
                else if (decisaoUsuario == 2)
                {
                    Console.Write("Digite o primeiro número: ");
                    double numero1;
                    if (!double.TryParse(Console.ReadLine(), out numero1))
                    {
                        Console.WriteLine("Valor inválido para o primeiro número. Por favor, insira um número válido.");
                        return;
                    }

                    Console.Write("Digite o segundo número: ");
                    double numero2;
                    if (!double.TryParse(Console.ReadLine(), out numero2))
                    {
                        Console.WriteLine("Valor inválido para o segundo número. Por favor, insira um número válido.");
                        return;
                    }

                    Console.Write("Digite a operação desejada (+-*/): ");
                    char operacao = Console.ReadKey().KeyChar;

                    double resultado = 0;

                    switch (operacao)
                    {
                        case '+':
                            resultado = numero1 + numero2;
                            break;
                        case '-':
                            resultado = numero1 - numero2;
                            break;
                        case '*':
                            resultado = numero1 * numero2;
                            break;
                        case '/':
                            if (numero2 != 0)
                            {
                                resultado = numero1 / numero2;
                            }
                            else
                            {
                                Console.WriteLine("Não é possível dividir por zero.");
                                return;
                            }
                            break;
                        default:
                            Console.WriteLine("Operação inválida. Por favor, insira uma operação válida (+-*/).");
                            return;
                    }

                    Console.WriteLine($"\nO resultado da operação é: {resultado}");
                }
                else
                {
                    Console.WriteLine("Opção inválida. Por favor, insira um número válido.");
                }
            }
            else
            {
                Console.WriteLine("Opção inválida. Por favor, insira um número válido.");
            }

            Console.WriteLine("\nPressione qualquer tecla para encerrar o programa...");
            Console.ReadKey(true);
        }
    }
}
~~~

## **_➡Estatísticas do GitHub_**

![Estatísticas do GitHub](https://github-readme-stats.vercel.app/api?username=MateusDias99&show_icons=true&count_private=true&theme=dracula&hide_border=true)

## **_➡Linguagem Mais Utilizada_**

![Linguagem Mais Utilizada](https://github-readme-stats.vercel.app/api/top-langs/?username=MateusDias99&layout=compact&theme=dracula&hide_border=true&langs_count=1&hide=jupyter%20notebook)

## **_➡Entre em Contato_**

| Nome          | Contato          |
| ------------- | -----------------|
| Mateus Dias   |[LinkedIn](https://www.linkedin.com/in/mateus-moraes-dias-429403250/)     |


<i>Fique à vontade para explorar meus repositórios e entrar em contato!<i> 😊

![Dia a Dia!](https://miro.medium.com/v2/resize:fit:1000/1*dxbvVHJkUh5HagZ7HI0nFw.gif)
