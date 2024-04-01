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
