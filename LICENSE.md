 public static void main(String[] args) {
        int[] numbers = {7, 2, 9, 1, 5};
        System.out.println("Before sorting: " + Arrays.toString(numbers));
        
        bubbleSort(numbers, numbers.length);
        
        System.out.println("After sorting: " + Arrays.toString(numbers));
    }
}
