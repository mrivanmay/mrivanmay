Class LinearFunction {
    
    Public Static main([] args) {
        
        Scanner x1Scan = new Scanner();
        System.out.println("Введите значение точки x1: ");
        int x1 = x1Scan.nextInt();

        Scanner y1Scan = new Scanner();
        System.out.println("Введите значение точки y1: ");
        int y1 = x2Scan.nextInt();

        Scanner x2Scan = new Scanner();
        System.out.println("Введите значение точки x2: ");
        int x2 = x2Scan.nextInt();

        Scanner y2Scan = new Scanner();
        System.out.println("Введите значение точки y2: ");
        int y2 = y2Scan.nextInt();

        // y = ax + b
        // a = (y2 - y1) / (x2 - x1)

        int a = (y2 - y1) / (x2 - x1);
        int b1 = y1 - a * x1;
        int b2 = y2 - a * x2;

        if (b1 == b2) {
            System.out.println("Уравнение прямой по заданным точкам: y = " + a + "x + " + b1);
        } else {
            System.out.println("Error: вычисления некорректны");
        }
    }
}
