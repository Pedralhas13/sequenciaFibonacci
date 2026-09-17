# sequenciaFibonacci
Exibe N termos de Fibonacci de acordo com o que o usuário pedir

import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a quantidade de termos (N): ");
        int n = scanner.nextInt();

        long primeiro = 0;
        long segundo = 1;

        System.out.println("Sequência de Fibonacci:");

        for (int i = 0; i < n; i++) {
            System.out.print(primeiro + " ");

            long proximo = primeiro + segundo;
            primeiro = segundo;
            segundo = proximo;
        }

        scanner.close();
    }
}
