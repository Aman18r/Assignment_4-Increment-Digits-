# Assignment_4-Increment-Digits-

import java.util.Arrays;
public class Main {
    public static int[] plusOne(int[] digits) {

        int n = digits.length;
        for(int i=n-1; i>=0; i--) {
            if(digits[i] < 9) {
                digits[i]++; return digits;
            }
            digits[i] = 0;
        }

        int[] newNumber = new int [n+1];
        newNumber[0] = 1;
        return newNumber;
    }
    public static void main(String[] args) {
        System.out.println("Increment digits are: ");
        int [] arr = {4,3,2,1};
        int[]ans=plusOne(arr);
        System.out.println(Arrays.toString(ans));
    }
}
