# File1
Atm code
public class LCMExample {

    // Method to get GCD of two numbers
    public static int getGCD(int a, int b) {
        while (b != 0) {
            int temp = b;
            b = a % b;
            a = temp;
        }
        return a;
    }

    // Method to get LCM of two numbers
    public static int getLCM(int a, int b) {
        return (a * b) / getGCD(a, b);
    }

    public static void main(String[] args) {
        int num1 = 12, num2 = 18;

        int lcm = getLCM(num1, num2);

        System.out.println("LCM of " + num1 + " and " + num2 + " is: " + lcm);
    }
}
