# hesapMakine
import java.util.Scanner;
public class HesapMakinesi {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);
        
        int secim;
        double sayi1, sayi2;
        
        System.out.println("Hesap Makinesi");
        System.out.println("1- Toplama");
        System.out.println("2- Çıkarma");
        System.out.println("3- Çarpma");
        System.out.println("4- Bölme");
        
        System.out.print("Seçiminiz (1-4): ");
        secim = scanner.nextInt();
        
        System.out.print("1. Sayı: ");
        sayi1 = scanner.nextDouble();
        
        System.out.print("2. Sayı: ");
        sayi2 = scanner.nextDouble();
        
        switch(secim) {
            case 1:
                System.out.println("Sonuç: " + (sayi1 + sayi2));
                break;
            case 2:
                System.out.println("Sonuç: " + (sayi1 - sayi2));
                break;
            case 3:
                System.out.println("Sonuç: " + (sayi1 * sayi2));
                break;
            case 4:
                System.out.println("Sonuç: " + (sayi1 / sayi2));
                break;
            default:
                System.out.println("Geçersiz seçim!");
                break;
        }
        
        scanner.close();
    }
}
