# SOMA-DE-DUAS-MATRIZES-PREENCHIDA-PELO-USUARIO-COD-JAVA

public class Exercicio {
	public static void main(String[] args) {
		int[][] m1 = new int[3][8];
		int[][] m2 = new int[3][8];
		int[][] result = new int[3][8];
		
		System.out.println("--------------- MATRIZ 1 ---------------");
		for(int lin = 0; lin < m1.length; lin++) { 
			for(int col = 0; col < m1[lin].length; col++) {
				System.out.printf("m1[%d][%d]: ", lin, col);
				m1[lin][col] = Integer.parseInt(System.console().readLine());
			}
		}
		
		System.out.println("--------------- MATRIZ 2 ---------------");
		for(int lin = 0; lin < m2.length; lin++) { 
			for(int col = 0; col < m2[lin].length; col++) {
				System.out.printf("m2[%d][%d]: ", lin, col);
				m2[lin][col] = Integer.parseInt(System.console().readLine());
			}
		}
		
		for(int lin = 0; lin < result.length; lin++) { 
			for(int col = 0; col < result[lin].length; col++) {
				result[lin][col] = m1[lin][col] + m2[lin][col];
			}
		}
		
		System.out.println("--------------- RESULTADO ---------------");
		for(int lin = 0; lin < result.length; lin++) { 
			for(int col = 0; col < result[lin].length; col++) {
				System.out.printf("result[%d][%d] = %d\n", lin, col, result[lin][col]);
			}
		}
	}
}
