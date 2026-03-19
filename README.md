# Listas
Atividades
namespace ListasC#
    { 
class Program
{
    static void Main()
    {
        int X = int.Parse(Console.ReadLine());
        for (int i = 1; i <= X; i += 2)
            Console.WriteLine(i);
    }
}

//Soma de Inparconsecultivos


class Program
{ 
static void Main()
{
        int X = int.Parse(Console.ReadLine());
        int Y = int.Parse(Console.ReadLine());
        if (X > Y) { int tmp = X; X = Y; Y = tmp; }
        int soma = 0;
        for (int i = X + 1; i < Y; i++)
            if (i % 2 != 0) soma += i;
        Console.WriteLine(soma);
    }
}

//Intervalo

class Program
{
    static void Main()
    {
        int N = int.Parse(Console.ReadLine());
        int dentro = 0, fora = 0;
        for (int i = 0; i < N; i++)
        {
            int X = int.Parse(Console.ReadLine());
            if (X >= 10 && X <= 20) dentro++;
            else fora++;
        }
        Console.WriteLine($"{dentro} in\n{fora} out");
    }
}

//Quadrados de Pares

class Program
{
    static void Main()
    {
        int N = int.Parse(Console.ReadLine());
        for (int i = 2; i <= N; i += 2)
            Console.WriteLine($"{i}^2 = {i * i}");
    }
}

//Par ou Ínpar

class Program
{
    static void Main()
    {
        int N = int.Parse(Console.ReadLine());
        int a = 0, b = 1;
        for (int i = 0; i < N; i++)
        {
            Console.Write(i < N - 1 ? $"{a} " : $"{a}\n");
            int temp = a; a = b; b += temp;
        }
    }
}

//Fibonacci facil

class Program
{
    static void Main()
    {
        int N = int.Parse(Console.ReadLine());
        int a = 0, b = 1;
        for (int i = 0; i < N; i++)
        {
            Console.Write(i < N - 1 ? $"{a} " : $"{a}\n");
            int temp = a; a = b; b += temp;
        }
    }
}

//Fatorial Sinples


class Program
{
    static void Main()
    {
        int N = int.Parse(Console.ReadLine());
        int fat = 1;
        for (int i = 2; i <= N; i++) fat *= i;
        Console.WriteLine(fat);
    }
}

