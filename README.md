# Perfect-Number

public class PerfectNumber {

        public static void main(String[] args) {
            System.out.println(isPerfectNumber(6));
        }
        public static boolean isPerfectNumber(int number) {
            if (number < 1) {
                return false;
            }
            int i = 0;
            int sumNumbers = 0;
            while(i < number) {
                i = i + 1;
                if(number % i == 0 && i != number){
                    System.out.println(i);
                    sumNumbers += i;
                }
            }
            return sumNumbers == number;
        }
}

