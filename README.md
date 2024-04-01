public class Main{
    public static void main(String[] args) {
        double ticketPrice = 13676.00;
        int miles = calculateMiles(ticketPrice);
        System.out.println("Количество начисленных миль: " + miles);
    }

    public static int calculateMiles(double ticketPrice) {
        return (int) Math.ceil(ticketPrice / 20.0);
    }
}




2 код


public class Main {
    public static void main(String[] args) {
        double bonus = 0;
        double initialBalance = 100;
        double depositAmount = 300;

        if (depositAmount > 1000) {
            int hundredDepositAmount = (int) Math.floor(depositAmount / 100);
            bonus = hundredDepositAmount;
        }

        double finalBalance = initialBalance + depositAmount - (bonus * 100);

        System.out.println("Итоговый баланс: " + finalBalance + " Бонусные рубли: " + bonus);
    }
}
