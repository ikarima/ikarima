/*NIM   : 13020210283
Nama    : Ikarima
Hari/Tgl: jumat, 10 Maret 2023
Waktu   : 03:08 PM*/

import java.util.Scanner;

public class ConvertSecondsToTime {
    public static void main(String[] args) {
        // Meminta input total detik dari pengguna
        Scanner input = new Scanner(System.in);
        System.out.print("Masukkan total detik: ");
        int totalDetik = input.nextInt();

        // Menghitung detik saat ini
        int detikSekarang = totalDetik % 60;

        // Menghitung total menit
        int totalMenit = totalDetik / 60;

        // Menghitung menit saat ini
        int menitSekarang = totalMenit % 60;

        // Menghitung total jam
        int totalJam = totalMenit / 60;

        // Menghitung jam saat ini
        int jamSekarang = totalJam % 24;

        // Menampilkan waktu dalam format jam:menit:detik
        System.out.println("Waktu saat ini adalah " + jamSekarang + ":" + menitSekarang + ":" + detikSekarang);
    }
}
