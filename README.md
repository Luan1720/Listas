using System.Diagnostics;

int[] vetor = new int;
int soma = 0;

for (int i = 0; i < 10; i++)
{
    Console.Write($"Digite o valor {i + 1}: ");
    vetor[i] = int.Parse(Console.ReadLine());
    soma += vetor[i];
}
Console.WriteLine($"O somatório é: {soma}");
//==========================================
.
int[] vetor = new int;
for (int i = 0; i < 15; i++)
{
    vetor[i] = int.Parse(Console.ReadLine());
}

Console.WriteLine("Números positivos:");
foreach (int num in vetor)
{
    if (num > 0) Console.WriteLine(num);
}
//=========================================

int[] vetor = new int;
for (int i = 0; i < 8; i++) vetor[i] = int.Parse(Console.ReadLine());

Console.Write("Digite o valor para busca: ");
int busca = int.Parse(Console.ReadLine());
bool encontrado = false;

for (int i = 0; i < 8; i++)
{
    if (vetor[i] == busca)
    {
        Console.WriteLine($"O número está na posição: {i}");
        encontrado = true;
        break;
    }
}
if (!encontrado) Console.WriteLine("O número não se encontra no vetor");
//=======================================

int[] v1 = new int;
int[] v2 = new int;
int[] v3 = new int;

for (int i = 0; i < 10; i++)
{
    v3[i] = v1[i] + v2[i];
    Console.Write(v3[i] + " ");
}
//=====================================
int[] vetor = new int;
int pares = 0, impares = 0, maiores50 = 0, menores7 = 0;

for (int i = 0; i < 20; i++)
{
    vetor[i] = int.Parse(Console.ReadLine());
    if (vetor[i] % 2 == 0) pares++; else impares++;
    if (vetor[i] > 50) maiores50++;
    if (vetor[i] < 7) menores7++;
}
Console.WriteLine($"Pares: {pares}, Ímpares: {impares}, >50: {maiores50}, <7: {menores7}");
//====================================
double[] salarios = new double;
for (int i = 0; i < 10; i++)
{
    Console.Write("Salário: ");
    salarios[i] = double.Parse(Console.ReadLine());
    salarios[i] *= 1.05; 
}

//=====================================
int[] vetor = new int;
for (int i = 0; i < 5; i++)
{ 
    int temp = vetor[i];
    vetor[i] = vetor[9 - i];
    vetor[9 - i] = temp;
}
