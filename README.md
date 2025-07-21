# TersUcgenimport java.util.Scanner;

public class TersUcgen {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Kullanıcıdan satır sayısı alınır
        System.out.print("Ters üçgenin yüksekliğini girin: ");
        int satir = scanner.nextInt();

        for (int i = satir; i >= 1; i--) {
            // Boşluklar
            for (int j = 0; j < satir - i; j++) {
                System.out.print(" ");
            }
            // Yıldızlar
            for (int k = 1; k <= (2 * i - 1); k++) {
                System.out.print("*");
            }
            // Yeni satıra geç
            System.out.println();
        }

        scanner.close();
    }
}
