# Reversing-numbers
public class Main {

    public static void main(String[] args) {
        System.out.println(reverse(9876));
    }
    public static int reverse(int number) {
        int rev = 0;
        int lastdigit = 0;
        while ((number > 0) && (number <= 10000)) {
            lastdigit = number % 10;
            rev = (rev * 10) + lastdigit;
            number /= 10;
        }
        return rev;
    }
}
