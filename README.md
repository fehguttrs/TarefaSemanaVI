package atividade.nova.pre.prova;

import java.util.Scanner;

public class ProgramaPrincipal {

	public static void main(String[] args) {
		
		Scanner entrada = new Scanner(System.in);
		System.out.println("Insira a medida da largura do retângulo: ");
		double largura = entrada.nextDouble();
		System.out.println("Insira a medida da altura do retângulo: ");
		double altura = entrada.nextDouble();
		Retangulo A = new Retangulo (largura, altura);
		
		System.out.println("A area do retângulo é : "+ A.calculaArea());
		System.out.println("O perímetro do retângulo é : "+A.calculaPerimetro());
		
		Retangulo retang = new Retangulo(12,7);
		retang.descricao();
		System.out.println("A area do retângulo é : "+ retang.calculaArea());
		System.out.println("O perímetro do retângulo é : "+retang.calculaPerimetro());
			
		System.out.println("Insira a medida do raio da circunferência: ");
		double raio = entrada.nextDouble();
		Circunferencia X = new Circunferencia (raio);
		System.out.println("A area da circunferencia é : "+X.calculaArea());
		System.out.println("O perímetro da circunferencia é : "+X.calculaPerimetro());
		entrada.close();
	}

}

