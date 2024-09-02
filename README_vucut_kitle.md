// vucut kitle indeksi icin update
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        float a; // Kilo
        float b; // Boy
        double indeks;
        Scanner input = new Scanner(System.in);
        System.out.print("Boyunuzu girin (metre cinsinden, örn: 1,75): ");
        b = input.nextFloat();
        System.out.print("Kilonuzu girin: ");
        a = input.nextFloat();
        indeks = a / (b * b);
        System.out.println("Vücut kitle indeksiniz: " + indeks);
        // durum ve yorum
        if (indeks < 18.5) {
            System.out.println("durum : cok zayıfsın öl");
        } else if (indeks >= 18.5 && indeks <= 24.9) {
            System.out.println("durum : iyisin iyi");
        } else if (indeks >= 25 && indeks <= 29.9) {
            System.out.println("durum : ekmegi kes ");
        } else if (indeks >= 30 && indeks <= 39.9) {
            System.out.println("(durum : obez)");
        } else if (indeks >= 40) {
            System.out.println("durum : agir yasamlar)");
        }
    }
}
