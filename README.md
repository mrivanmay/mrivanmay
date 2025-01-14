public class LinearFunction {
    
    Public Static void main(String[] args) {
        
        Scanner x1Scan = new Scanner(System.in);
        System.out.println("Введите значение точки x1: ");
        BigDecimal x1 = new BigDecimal(x1Scan.nextLine());

        Scanner y1Scan = new Scanner(System.in);
        System.out.println("Введите значение точки y1: ");
        BigDecimal y1 = new BigDecimal(x2Scan.nextLine());

        Scanner x2Scan = new Scanner(System.in);
        System.out.println("Введите значение точки x2: ");
        BigDecimal x2 = new BigDecimal(x2Scan.nextLine());

        Scanner y2Scan = new Scanner(System.in);
        System.out.println("Введите значение точки y2: ");
        BigDecimal y2 = new BigDecimal(y2Scan.nextLine());

        if (x1.compareTo(x2) == 0) {
            System.out.println("Уравнение невозможно. Точки х имеют одинаковое значение");
        }

        // y = ax + b
        // a = (y2 - y1) / (x2 - x1)
        // add, subtract, multiply, divide

        BigDecimal a = (y2.subtract(y1)).divide(x2.subtract(x1));
        BigDecimal b1 = y1.subtract(a.multiply(x1));
        BigDecimal b2 = y2.subtract(a.multiply(x2));

        if (b1 == b2) {
            System.out.println("Уравнение прямой по заданным точкам: y = " + a + "x + " + b1);
        } else {
            System.out.println("Error: вычисления некорректны");
        }
    }
}
