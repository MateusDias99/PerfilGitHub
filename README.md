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
using System.Globalization;
using System.Net.Security;
using System.Reflection;
using System.Threading.Tasks.Dataflow;

int contador_repeticao = 0;


Console.WriteLine("Escreva seu nome:");
Nome = string.Parse(Console.ReadLine());

Console.WriteLine("Escreva sua idade:");
Idade = int.Parse(Console.ReadLine());

Console.WriteLine("Escreva seu Peso:");
Peso = float.Parse(Console.ReadLine());


while (contador_repeticao < 10){  

    if (Nome == "Mateus") 
    {
    Console.WriteLine("Logado: " + Nome, "Com a idade de:"  + Idade,  "Com o peso de: ", + Peso);
    ++contador_repeticao;
    continue;
    }
    else
    {
    Console.WriteLine("Erro ao Logar vc vai receber um DDOS");   
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
