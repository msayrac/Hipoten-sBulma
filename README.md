# Hipotenus Cevre Alan Bulma
Dik Üçgende Hipotenüs Bulan Program
Java ile kullanıcıdan dik kenarlarının uzunluğunu alan ve hipotenüsü hesaplayan programı yazın.

Ödev
Üç kenar uzunluğunu kullanıcıdan aldığınız üçgenin alanını hesaplayan programı yazınız.

Formül
Üç𝑔𝑒𝑛𝑖𝑛 ç𝑒𝑣𝑟𝑒𝑠𝑖 = 2𝑢

𝑢 = (a+b+c) / 2

Alan * Alan = 𝑢 * (𝑢 − 𝑎)* (𝑢 − 𝑏) * (𝑢 − 𝑐)

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        int a, b;
        double c;

        Scanner input = new Scanner(System.in);
        System.out.println("1. Kenari giriniz : ");

        a = input.nextInt();

        System.out.println("2. Kenari giriniz : ");

        b = input.nextInt();
        c= Math.sqrt(Math.pow(a,2) +Math.pow(b,2));


        System.out.println("Dik Ucgenin Hipotenus degeri : " + c);

        double u = (a+b+c)/2;
        System.out.println("Dik Ucgenin Cevresi : " + u*2);

        double alan = u*(u-a)*(u-b)*(u-c);

        System.out.println("Dik Ucgenin Alani : " + alan);

   }
}

