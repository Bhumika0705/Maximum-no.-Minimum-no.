# Maximum-no.-Minimum-no.
This code is for finding maximum and minimum number in any particular given array
import java.util.Scanner;

public class maxmin {
    public maxmin() {
    }

    public static void main(String[] args) {
        System.out.println("Enter the size of array:");
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the elements in array:");

        int max;
        for(max = 0; max < n; ++max) {
            arr[max] = sc.nextInt();
        }

        max = Integer.MAX_VALUE;
        int min = Integer.MIN_VALUE;

        int i;
        for(i = 0; i < n; ++i) {
            if (arr[i] < min) {
                min = arr[i];
            }
        }

        for(i = 0; i < n; ++i) {
            if (arr[i] > max) {
                max = arr[i];
            }
        }

        System.out.println("Largest no.: " + max);
        System.out.println("Smallest no.: " + min);
    }
}
