# 26PR
# 26 Практика
# Задание 1
```
import java.util.Stack;

public class ArrayInverter {
    
    public static void invertArray(int[] array) {
        Stack<Integer> stack = new Stack<>();

        for (int num : array) {
            stack.push(num);
        }

        for (int i = 0; i < array.length; i++) {
            array[i] = stack.pop();
        }
    }

    public static void main(String[] args) {
        int[] myArray = {1, 2, 3, 4, 5};
        
        System.out.println("Исходный массив:");
        for (int num : myArray) {
            System.out.print(num + " ");
        }

        invertArray(myArray);
        
        System.out.println("nИнвертированный массив:");
        for (int num : myArray) {
            System.out.print(num + " ");
        }
    }
}
```
