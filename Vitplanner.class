import java.util.ArrayList;
import java.util.Scanner;

public class Vitplanner {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<String> tasks = new ArrayList<>();

        System.out.println("================= VitPlanner ====================");

        while (true) {
            System.out.println("\nMenu");
            System.out.println("1. Tambah Tugas Sehat");
            System.out.println("2. Lihat Semua Tugas");
            System.out.println("3. Hapus Tugas");
            System.out.println("4. Keluar");
            System.out.print("Pilih Opsi: ");

            int choice = scanner.nextInt();
            scanner.nextLine(); // untuk membersihkan newline dari nextInt()

            switch (choice) {
                case 1 -> {
                    System.out.print("Masukkan Nama Tugas: ");
                    String task = scanner.nextLine();
                    tasks.add(task);
                    System.out.println("Tugas berhasil ditambahkan!");
                }

                case 2 -> {
                    System.out.println("\nDaftar Tugas:");
                    if (tasks.isEmpty()) {
                        System.out.println("Tidak ada tugas.");
                    } else {
                        for (int i = 0; i < tasks.size(); i++) {
                            System.out.println((i + 1) + ". " + tasks.get(i));
                        }
                    }
                }

                case 3 -> {
                    System.out.print("Masukkan nomor tugas yang akan dihapus: ");
                    int taskNumber = scanner.nextInt();
                    scanner.nextLine(); // bersihkan newline
                    if (taskNumber > 0 && taskNumber <= tasks.size()) {
                        tasks.remove(taskNumber - 1);
                        System.out.println("Tugas berhasil dihapus!");
                    } else {
                        System.out.println("Nomor tugas tidak valid.");
                    }
                }

                case 4 -> {
                    System.out.println("Terima kasih telah menggunakan VitPlanner!");
                    scanner.close();
                    return;
                }

                default -> System.out.println("Opsi tidak valid, silakan coba lagi.");
            }
        }
    }
}
