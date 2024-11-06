import java.util.Scanner;

public class DataTypeInfo {

    public static void main(String[] args) {
        // Displaying information about primitive data types
        System.out.println("Information about primitive data types:");

        System.out.printf("byte: Size = %d bits, Min = %d, Max = %d%n", Byte.SIZE, Byte.MIN_VALUE, Byte.MAX_VALUE);
        System.out.printf("short: Size = %d bits, Min = %d, Max = %d%n", Short.SIZE, Short.MIN_VALUE, Short.MAX_VALUE);
        System.out.printf("int: Size = %d bits, Min = %d, Max = %d%n", Integer.SIZE, Integer.MIN_VALUE, Integer.MAX_VALUE);
        System.out.printf("long: Size = %d bits, Min = %d, Max = %d%n", Long.SIZE, Long.MIN_VALUE, Long.MAX_VALUE);
        System.out.printf("float: Size = %d bits, Min = %e, Max = %e%n", Float.SIZE, Float.MIN_VALUE, Float.MAX_VALUE);
        System.out.printf("double: Size = %d bits, Min = %e, Max = %e%n", Double.SIZE, Double.MIN_VALUE, Double.MAX_VALUE);
        System.out.printf("char: Size = %d bits, Min = %d, Max = %d%n", Character.SIZE, (int) Character.MIN_VALUE, (int) Character.MAX_VALUE);
        System.out.println("boolean: Size = 1 bit, Values = true or false");

        // Creating a Scanner object to read user input from the console
        Scanner scanner = new Scanner(System.in);

        try {
            // Reading a value of type byte
            System.out.print("Enter a value of type byte: ");
            byte byteValue = Byte.parseByte(scanner.nextLine());
            System.out.println("You entered byte: " + byteValue);

            // Reading a value of type short
            System.out.print("Enter a value of type short: ");
            short shortValue = Short.parseShort(scanner.nextLine());
            System.out.println("You entered short: " + shortValue);

            // Reading a value of type int
            System.out.print("Enter a value of type int: ");
            int intValue = Integer.parseInt(scanner.nextLine());
            System.out.println("You entered int: " + intValue);

            // Reading a value of type long
            System.out.print("Enter a value of type long: ");
            long longValue = Long.parseLong(scanner.nextLine());
            System.out.println("You entered long: " + longValue);

            // Reading a value of type float
            System.out.print("Enter a value of type float: ");
            float floatValue = Float.parseFloat(scanner.nextLine());
            System.out.println("You entered float: " + floatValue);

            // Reading a value of type double
            System.out.print("Enter a value of type double: ");
            double doubleValue = Double.parseDouble(scanner.nextLine());
            System.out.println("You entered double: " + doubleValue);

            // Reading a value of type char
            System.out.print("Enter a character of type char: ");
            char charValue = scanner.nextLine().charAt(0);
            System.out.println("You entered char: " + charValue);

            // Reading a value of type boolean
            System.out.print("Enter a value of type boolean (true or false): ");
            boolean booleanValue = Boolean.parseBoolean(scanner.nextLine());
            System.out.println("You entered boolean: " + booleanValue);

        } catch (NumberFormatException e) {
            System.out.println("Error: Invalid input.");
        } finally {
            scanner.close();
        }
    }
}
