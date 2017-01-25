# numbersToWord



public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner scan = new Scanner(System.in);
		System.out.print("Enter a = ");
		int a = scan.nextInt();
    scan.close();
            
		int firstNum = a/100;
		int secondNum = (a%100)/10;
		int lastNum = a%10;
		int lastTwo = a%100;
		
		if (a==0){
		System.out.print("Нула");
		}
        if (firstNum <= 9){
		switch (firstNum) {
			case 1: System.out.print("Сто ");break;
			case 2: System.out.print("Двеста ");break;
			case 3: System.out.print("Триста ");break;
			case 4: System.out.print("Четиристотин ");break;
			case 5: System.out.print("Петстотин ");break;
			case 6: System.out.print("Шестотин ");break;
			case 7: System.out.print("Седемстотин ");break;
			case 8: System.out.print("Осемстотин ");break;
			case 9: System.out.print("Деветстотин ");break;
			}
		if (secondNum == 1) {
		switch (lastTwo) { 
			case 10: System.out.print("и десет "); break;
			case 11: System.out.print("и единадесет "); break;
			case 12: System.out.print("и дванадесет "); break;
			case 13: System.out.print("и тринадесет "); break;
			case 14: System.out.print("и четиринадесет "); break;
			case 15: System.out.print("и петнадесет "); break;
			case 16: System.out.print("и шестнадесет "); break;
			case 17: System.out.print("и седемнадесет "); break;
			case 18: System.out.print("и осемнадесет "); break;
			case 19: System.out.print("и деветнадесет "); break;
		    }
		}else {
			if (lastNum == 0 && a != 0){
				System.out.print(" и ");
			}
        if (secondNum != 1){	
		switch(secondNum) {
		    case 0: System.out.print(""); break;
			case 2: System.out.print("двадесет"); break;
			case 3: System.out.print("тридесет"); break;
			case 4: System.out.print("четиресет"); break;
			case 5: System.out.print("петдесет"); break;
			case 6: System.out.print("шестдесет"); break;
			case 7: System.out.print("седемдесет"); break;
			case 8: System.out.print("осемдесет"); break;
			case 9: System.out.print("деветдесет"); break;
			}
		
		if (lastNum != 0 && (firstNum!=0 || secondNum != 0)){
			System.out.print(" и ");
		}
		if (lastNum !=0){	
		switch (lastNum) {
			
			case 1: System.out.print("едно "); break;
			case 2: System.out.print("две "); break;
			case 3: System.out.print("три "); break;
			case 4: System.out.print("четири "); break;
			case 5: System.out.print("пет "); break;
			case 6: System.out.print("шест "); break;
			case 7: System.out.print("седем "); break;
			case 8: System.out.print("осем "); break;
			case 9: System.out.print("девет "); break;
			}
		  }
        }
      }	
    }
