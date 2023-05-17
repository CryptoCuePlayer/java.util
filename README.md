# java.util
java.util
import java.util.Arrays;

public class BubbleSort {
    public static void bubbleSort(int[] array, int n) {
        if (n == 1) return;
        
        for (int i = 0; i < n - 1; i++) {
            if (array[i] > array[i + 1]) {
                int temp = array[i];
                array[i] = array[i + 1];
                array[i + 1] = temp;
            }
        }
        
        bubbleSort(array, n - 1);
    }

    public static void main(String[] args) {
        int[] numbers = {7, 2, 9, 1, 5};
        System.out.println("Before sorting: " + Arrays.toString(numbers));
        
        bubbleSort(numbers, numbers.length);
        
        System.out.println("After sorting: " + Arrays.toString(numbers));
    }
}
