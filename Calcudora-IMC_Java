import java.util.InputMismatchException;
import java.util.Scanner;

public class imc {
   public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.println("Digite o peso: ");
            float peso;
            try {
                peso = scanner.nextFloat();
            } catch (InputMismatchException e) {
                System.out.println("Entrada inválida.");
                return;
            }
            System.out.println("Digite a altura: ");
            float altura;
            try {
                altura = scanner.nextFloat();
            } catch (InputMismatchException e) {
                System.out.println("Entrada inválida.");
                return;
            }
            double imc = peso / (altura * altura);
            System.out.println("IMC: " + imc);
            System.out.print("Classificação: ");
            if (imc < 18.5) {
                System.out.println("Abaixo do peso");
            } else if (imc < 24.9) {
                System.out.println("Peso normal");
            } else if (imc < 29.9) {
                System.out.println("Sobrepeso");
            } else if (imc < 34.9) {
                System.out.println("Obesidade grau 1");
            } else if (imc < 39.9) {
                System.out.println("Obesidade grau 2");
            } else {
                System.out.println("Obesidade grau 3");
            }
        }
    }
}
