# Explorando-Scharp
Curso Alura
using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Olá, Mundo!");
        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}


using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Projeto 2 - Criando Variáveis");

        // idade variável valor inteiro. 
        int idade;

        // idade variável valor inteiro = 27
        idade = 27;
        Console.WriteLine("Minha idade é" + idade);

        // idade variável valor inteiro = 22
        idade = 27 - 5;
        Console.WriteLine(idade);

        // idade variável valor inteiro = 4
        idade = 5 * 2 - 6;
        Console.WriteLine(idade);

        //idade variável valor inteiro = 9
        // Obs: Resolver primeiro a conta entre parentes.
        idade = (5 - 2) * 3;
        Console.WriteLine(idade);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}
using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Projeto 3 - Variáveis Ponto Flutuantes");

        //Variável do tipo double;
        //Aceita números com pontos e vírgula;
        double salario;
        salario = 3000.10;
        salario = 3000;

        //Idade do tipo double
        //Obs: DOUBLE aceita números interios, entretanto INT não aceita números com pontos. 
        double idade;
        idade = 7.0 / 5;

        Console.WriteLine(idade);

        Console.WriteLine(salario);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        double salario;
        salario = 3000.15;
        Console.WriteLine(salario);

        int salarioInteiro;
        salarioInteiro = (int)salario;
        Console.WriteLine(salarioInteiro);

        // O long é uma variável de 64 bits.
        long x;
        x = 20000000000000000;
        Console.WriteLine(x);

        // O short é uma variável de 32 bits.
        short y;
        y = 15000;
        Console.WriteLine(y);

        // O float é uma variável de 16 bits. 
        float altura;
        altura = 1.62f;
        Console.WriteLine(altura);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando o projeto 5 - Caracteres e textos");

        //Variável do tipo char, inserir aspas simples.
        char letra = 'a';
        Console.WriteLine(letra);

        //Convertendo variável do tipo int para o tipo char.
        letra = (char)65;
        Console.WriteLine(letra);

        letra = (char)(65 + 1);
        Console.WriteLine(letra);

        letra = (char)(86 + 2);
        Console.WriteLine(letra);

        //string passar o texto com aspas duplas.
        string primeiraFrase = "Alura - Cursos de Tecnologia ";
        Console.WriteLine(primeiraFrase + 2022);

        //Consegue adicionar uma string com o campo de texto vazio.
        string vazia = "";
        Console.WriteLine(vazia);

        //Consegue adicionar um char com o campo de texto vazio, entretanto precisa dar um espaço.
        letra = ' ';

        //Adicionando o @ no texto de string, o mesmo vira uma lista. 
        string cursos = @"Cursos Disponíveis: 
        -Go 
        -C# 
        -Python 
        -Java";
        Console.WriteLine(cursos);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
        
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 6 - Atribuições de Variáveis");

        int idade = 22;
        int idadeFelippe = idade;

        Console.WriteLine(idadeFelippe);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}


using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 7 - Condicionais");

        int idadeFelippe = 16;
        int quantidadePessoas = 2;

        if (idadeFelippe >= 18)
        {
            Console.WriteLine("Pode entrar!");
        }
        else
        {
            if (quantidadePessoas > 0)
            {
                Console.WriteLine("Ele está acompanhado. Pode entrar!");
            }
            else 
            {
                Console.WriteLine("Não pode entrar");
            }
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 8 - Condicionais2");

        int idadeFelippe = 16;
        int quantidadePessoas = 2;

        bool acompanhado = quantidadePessoas > 1;
        bool grupo = true;

        if (idadeFelippe >= 18 || grupo)
        {
            Console.WriteLine("Pode entrar!");
        }
        else
        {
            Console.WriteLine("Não pode entrar");
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 8 - Condicionais2");

        int idadeFelippe = 16;
        int quantidadePessoas = 2;

        bool acompanhado = quantidadePessoas > 1;

        string textoAdicional;

        if (acompanhado == true)
        {
            textoAdicional = "João está acompanhado";
        }
        else
        {
            textoAdicional = "João não está acompanhado";
        }

        if (idadeFelippe >= 18 || acompanhado)
        {
            Console.WriteLine(textoAdicional);
            Console.WriteLine("Pode entrar!");
        }
        else
        {
            Console.WriteLine("Não pode entrar");
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 10 - Calcula Poupança");

        double investimento = 1000;

        // Rendimento de 0.5% ao (0.005) mês

        //mês 1
        investimento = investimento + investimento * 0.005;
        //mês 2
        investimento = investimento + investimento * 0.005;
        //mês 3
        investimento = investimento + investimento * 0.005;

        Console.WriteLine(investimento);

        int mes = 1;

        while (mes <= 12)
        {
            investimento = investimento + investimento * 0.005;
            Console.WriteLine("No mês " + investimento + "Você tem R$ " + investimento);

            // mes = mes + 1;
            mes += 1;
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 11 - Calcula Poupança");

        double investimento = 1000;

        for (int mes = 1; mes <= 12; mes = mes + 1)
        {
            investimento += 1.005;
            Console.WriteLine("No mes " + mes + "Você tem R$ " + investimento); 
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}

using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 12 - Investimento a longo prazo");

        double fatorRendimento = 1.005;
        double investimento = 1000;

        for (int anos = 1; anos <= 5; anos++)
        {
            for (int mes = 1; mes <= 12; mes++)
            {
                investimento *= fatorRendimento;
            }

            fatorRendimento += 0.001;
        }

        Console.WriteLine("Depois de 5 anos você terá R$ " + investimento);

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}


using System;

class Programa
{
    static void Main(string[] args)
    {
        Console.WriteLine("Executando projeto 13 - Encadeando For");

        //*
        //**
        //***
        //****
        //*****
        //******

        for (int contadorLinhas = 0; contadorLinhas < 10; contadorLinhas++)
        {
            for (int contadorColunas = 0; contadorColunas < 10; contadorColunas++)
            {
                Console.Write("*");
                if (contadorColunas >= contadorLinhas)
                    break;
            }
            Console.WriteLine();
        }

        Console.WriteLine("Tecle enter para fechar...");
        Console.ReadLine();
    }
}
