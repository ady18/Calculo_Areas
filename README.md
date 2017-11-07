# Calculo_Areas
package com.adirane;
import java.util.*;
import javax.swing.*;

public class Areas {

	public static void main(String[] args) {
		
		Scanner teclado = new Scanner(System.in);
		
		System.out.println("Elige una opción: \n1. Cuadrado \n2. Rectángulo \n3. Triángulo \n4.Círculo");
		
		int figura = teclado.nextInt();
		
		switch (figura){
			
		case 1:
			
			int lado = Integer.parseInt(JOptionPane.showInputDialog("Introduce el lado:"));
			
			System.out.println("El área del Cuadrado es " + Math.pow(lado, 2));
			
			break;
			
		case 2:
			
			int base = Integer.parseInt(JOptionPane.showInputDialog("Introduce la base:"));
			
			int altura = Integer.parseInt(JOptionPane.showInputDialog("Introduce la altura:"));
			
			System.out.println("El área del Rectángulo es " + base*altura);
			
			break;
			
		case 3:
			
			base = Integer.parseInt(JOptionPane.showInputDialog("Introduce la base:"));
			
			altura = Integer.parseInt(JOptionPane.showInputDialog("Introduce la altura:"));
			
			System.out.println("El área del Triángulo es " + (base*altura)/2);
			
			break;
			
		case 4:
			
			int radio = Integer.parseInt(JOptionPane.showInputDialog("Introduce el radio:"));
			
			System.out.print("El área del Círculo es ");
			
			System.out.printf("%1.2f", Math.PI*(Math.pow(radio, 2))); //La instrucción aquí sería PI*radio^2, 
																		//el %1.2f redondea el formato de salida
			
			break;
			
		default:
			
			System.out.println("La opción es incorrecta");
		} 

	}

}
