# Ex15 Value Existence Check in a TreeMap
## DATE: 12-10-2025
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Read n and insert n key–value pairs into the TreeMap.
2. Read the value to be searched in the TreeMap.
3. In checkValue, use containsValue to check whether the given value exists.
4. If it exists, print that the value is present in the TreeMap.
5. Otherwise, print that the value does not exist.

## Program:
```JAVA
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: Ashwin Akash M
RegisterNumber: 212223230024
*/
import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        // Type Your Code Here.
        if(map.containsValue(searchValue))
        System.out.println("Value \""+searchValue+"\" exists in the TreeMap.");
        else
        System.out.println("Value \""+searchValue+"\" does not exist in the TreeMap.");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

```

## Output:
<img width="1249" height="735" alt="image" src="https://github.com/user-attachments/assets/82f781eb-b564-4694-b48f-88d103dae84e" />



## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
