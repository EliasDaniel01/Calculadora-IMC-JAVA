# 🧮 Calculadora de IMC em Java

Este projeto é uma calculadora simples de IMC (**Índice de Massa Corporal**) desenvolvida em Java, ideal para testes e aprendizado.

## ✨ Funcionalidades

- Calcula o IMC a partir do peso e altura informados pelo usuário.
- Informa a faixa de classificação do IMC (baixo peso, normal, sobrepeso, obesidade).

## 📋 Exemplo de código

```java
import java.util.Scanner;

public class CalculadoraIMC {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("=== Calculadora de IMC ===");
        System.out.print("Digite seu peso (kg): ");
        double peso = scanner.nextDouble();

        System.out.print("Digite sua altura (m): ");
        double altura = scanner.nextDouble();

        double imc = peso / (altura * altura);

        System.out.printf("Seu IMC é: %.2f\n", imc);

        if (imc < 18.5) {
            System.out.println("Classificação: Baixo peso");
        } else if (imc < 25) {
            System.out.println("Classificação: Peso normal");
        } else if (imc < 30) {
            System.out.println("Classificação: Sobrepeso");
        } else {
            System.out.println("Classificação: Obesidade");
        }

        scanner.close();
    }
}
```

## 🚀 Como executar

1. Copie o código acima em um arquivo chamado `CalculadoraIMC.java`.
2. Compile o arquivo:
   ```
   javac CalculadoraIMC.java
   ```
3. Execute o programa:
   ```
   java CalculadoraIMC
   ```

## 🛠️ Requisitos

- Java 8 ou superior instalado na sua máquina.

## 📚 Objetivo

Este projeto foi criado apenas para fins de teste e aprendizado pessoal. Fique à vontade para modificar, estudar e experimentar!

---
