# DiziTekrar
www.patika.dev
--------------


public class DiziTekrar {
	
	public static void main(String[] args) {
		
		int[] array = {9,8,19,20,18,2,15,1,6,11,19,18,4,11,16,5,13,9,6,11,7,15,11,8,18,12,7,9,2,9,9,8,19,20,11,15,8,16,15,11,7,5,14,12};
		
		for (int i = 0; i < array.length; i++) {
		    for (int j = i + 1; j < array.length; j++) {
		        if (array[i] == array[j] && array[i] % 2 == 0) {
		            boolean isDuplicate = false;
		            for (int k = 0; k < i; k++) {
		                if (array[k] == array[i]) {
		                    isDuplicate = true;
		                    break;
		                }
		            }
		            if (!isDuplicate) {
		                System.out.print(array[i] + " ");
		            }
		            break;
		        }
		    }
		}
	}
}
