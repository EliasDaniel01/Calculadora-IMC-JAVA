# 🧮 Calculadora Básica em Java

Este é um projeto simples de uma **calculadora básica** desenvolvida em Java. O objetivo principal é servir como laboratório de testes e aprendizado, praticando conceitos fundamentais da linguagem.

## ✨ Funcionalidades

- Soma
- Subtração
- Multiplicação
- Divisão

## 📋 Exemplo de código

```java
import java.util.Scanner;

public class CalculadoraBasica {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("=== Calculadora Básica ===");
        System.out.print("Digite o primeiro número: ");
        double num1 = scanner.nextDouble();

        System.out.print("Digite o operador (+, -, *, /): ");
        char operador = scanner.next().charAt(0);

        System.out.print("Digite o segundo número: ");
        double num2 = scanner.nextDouble();

        double resultado;

        switch (operador) {
            case '+':
                resultado = num1 + num2;
                break;
            case '-':
                resultado = num1 - num2;
                break;
            case '*':
                resultado = num1 * num2;
                break;
            case '/':
                if (num2 != 0) {
                    resultado = num1 / num2;
                } else {
                    System.out.println("Erro: Divisão por zero!");
                    scanner.close();
                    return;
                }
                break;
            default:
                System.out.println("Operador inválido!");
                scanner.close();
                return;
        }

        System.out.println("Resultado: " + resultado);
        scanner.close();
    }
}
```

## 🚀 Como executar

1. Copie o código acima em um arquivo chamado `CalculadoraBasica.java`.
2. Compile o arquivo:
   ```
   javac CalculadoraBasica.java
   ```
3. Execute o programa:
   ```
   java CalculadoraBasica
   ```

## 🛠️ Requisitos

- Java 8 ou superior instalado na sua máquina.

## 📚 Objetivo

Este projeto foi criado apenas para fins de teste e aprendizado pessoal. Fique à vontade para modificar, estudar e experimentar!

---
