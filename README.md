
public class PrimeNumbers {
    public static void main(String[] args) {

        int count = 0;
        int number = 2;

        System.out.println("First 100 Prime Numbers:");

        while (count < 100) {

            boolean isPrime = true;

            for (int i = 2; i <= Math.sqrt(number); i++) {

                if (number % i == 0) {
                    isPrime = false;
                    break;
                }
            }

            if (isPrime) {
                System.out.print(number + " ");
                count++;
            }

            number++;
        }
    }
}
