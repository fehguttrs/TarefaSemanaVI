package atividade.nova.pre.prova;

import java.util.Scanner;

public class ProgramaPrincipal {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Insira a medida da largura do retângulo: ");
            double largura = scanner.nextDouble();

            System.out.print("Insira a medida da altura do retângulo: ");
            double altura = scanner.nextDouble();

            Retangulo retanguloCriado = new Retangulo(largura, altura);
            System.out.printf("A Área do retângulo é: %.2f%n", retanguloCriado.calculaArea());
            System.out.printf("O perímetro do retângulo é: %.2f%n%n", retanguloCriado.calculaPerimetro());

            Retangulo retanguloExemplo = new Retangulo(12, 7);
            retanguloExemplo.descricao();
            System.out.printf("A Área do retângulo exemplo: %.2f%n", retanguloExemplo.calculaArea());
            System.out.printf("O perímetro do retângulo exemplo: %.2f%n%n", retanguloExemplo.calculaPerimetro());

            System.out.print("Insira a medida do raio da circunferência: ");
            double raio = scanner.nextDouble();

            Circunferencia circunferenciaCriada = new Circunferencia(raio);
            System.out.printf("A área da circunferência é: %.2f%n", circunferenciaCriada.calculaArea());
            System.out.printf("O perímetro da circunferência é: %.2f%n", circunferenciaCriada.calculaPerimetro());
        }
    }
}
