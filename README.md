# PBO_Teori
          BAB 1
Pengenalan Pemrograman Komputer
    Kata komputer berasal dari bahasa Latin yaitu Computare yang artinya menghitung.
Dalam bahasa Inggris disebut to compute. Secara definisi komputer diterjemahkan
sebagai sekumpulan alat elektronik yang saling bekerja sama, dapat menerima data
(input), mengolah data (proses) dan memberikan informasi (output) serta terkoordinasi
dibawah kontrol program yang tersimpan di memorinya.
    Flowchart adalah representasi grafis dari langkah – langkah yang harus diikuti dalam
menyelesaikan suatu permasalahan yang terdiri atas sekumpulan simbol, dimana
masing – masing simbol merepresentasikan kegiatan tertentu. Flowchart diawali dengan
penerimaan input dan diakhiri dengan penampilan output.
  >Simbol proses
  >simbol I/O
  >simbol Garis
  >simbol garis alir
  >simbol anotasi
  >simbol percabgan
  >simbol terminator
  >simbol konektor
  simbol prosedur
  
        Bilangan dapat disajikan dalam beberapa cara. Cara penyajiannya tergantung pada Basis
(BASE) bilangan tersebut. Terdapat 4 cara utama dalam penyajian bilangan. 
  >sistem bilangan desimal
    Bilangan desimal adalah sistem bilangan yang berbasis 10. Hal ini berarti bilangan – bilangan pada sistem ini terdiri dari 0 sampai dengan 9.
  >sistem bilangan oktal
    Bilangan yang berbasis 8.Bilangan-bilangan yang diperoleh hanya berkisar antara 0-7
  >sistem bilangan heksadesimal
    Bilangan yang berbasis 16.Sistem hanya memperbolehkan pengunaan bilangan dalam skala 0-9 dan mengunakan huruf A- F atau a - f karena perbedaan kapital huruf tidak     memiliki efek apapun.
  >sistem bilangan biner  
    Bilangan yang berbasis 2.Ini menyatakan bilangan yang terdapat dalam sistem ini hanya 0 dan 1
    
    >Konversi Bilangan Desimal ke Biner (mengunakan Metode pembagian dengan angka 2)
    >Konversi Bilangan Desimal ke oktal (mengunakan Metode pembagian dengan angka 2 untuk biner,angka 8 untuk oktal)
    >Konversi Bilangan Biner ke oktal (Untuk mengubah bilangan biner ke oktal, kita pila bilangan tersebut menjadi 3 bit bilangan biner dari kanan ke kiri.)
    >Konversi Bilangan Biner ke Heksadesimal (Pengubahan bilangan Biner ke Heksadesimal dilakukan dengan pengelompokan setiap empat bit Biner dimulai dari bit paling  kanan.Kemudian konversikan setiap kelompok menjadi satu digit Heksadesimal.)
  Begitu Sebaliknya
  
  Latihan Modul 1
  1. 198010  ke sistem bilangan Biner, Heksadesimal dan Oktal 
  public class KonversiBilangan {
            
    public static void main(String[] args) {
        int bilanganDesimal = 1980;

        // Konversi ke biner
        String bilanganBiner = Integer.toBinaryString(bilanganDesimal);
        System.out.println("Biner: " + bilanganBiner);

        // Konversi ke heksadesimal
        String bilanganHeksadesimal = Integer.toHexString(bilanganDesimal);
        System.out.println("Heksadesimal: " + bilanganHeksadesimal);

        // Konversi ke oktal
        String bilanganOktal = Integer.toOctalString(bilanganDesimal);
        System.out.println("Oktal: " + bilanganOktal);
    }
}

    2. 100100110 2  ke sistem bilangan Desimal, Heksadesimal dan Oktal
    public class KonversiBilangan2 {
    
    public static void main(String[] args) {
        String bilanganBiner = "1001001101";

        // Konversi ke desimal
        int bilanganDesimal = Integer.parseInt(bilanganBiner, 2);
        System.out.println("Desimal: " + bilanganDesimal);

        // Konversi ke heksadesimal
        String bilanganHeksadesimal = Integer.toHexString(bilanganDesimal);
        System.out.println("Heksadesimal: " + bilanganHeksadesimal);

        // Konversi ke oktal
        String bilanganOktal = Integer.toOctalString(bilanganDesimal);
        System.out.println("Oktal: " + bilanganOktal);
    }
}

    3.768 ke sistem bilangan Biner, Heksadesimal dan Desimal
    public class KonversiBilangan3 {
    
    public static void main(String[] args) {
        String bilanganOktal = "76";

        // Konversi ke desimal
        int bilanganDesimal = Integer.parseInt(bilanganOktal, 8);
        System.out.println("Desimal: " + bilanganDesimal);

        // Konversi ke biner
        String bilanganBiner = Integer.toBinaryString(bilanganDesimal);
        System.out.println("Biner: " + bilanganBiner);

        // Konversi ke heksadesimal
        String bilanganHeksadesimal = Integer.toHexString(bilanganDesimal);
        System.out.println("Heksadesimal: " + bilanganHeksadesimal);
    }
}

    4. 43F16 ke sistem bilangan Biner, Desimal dan Oktal
  public class KonversiBilangan4 {
   
    public static void main(String[] args) {
        String bilanganHeksadesimal = "43F";

        // Konversi ke desimal
        int bilanganDesimal = Integer.parseInt(bilanganHeksadesimal, 16);
        System.out.println("Desimal: " + bilanganDesimal);

        // Konversi ke biner
        String bilanganBiner = Integer.toBinaryString(bilanganDesimal);
        System.out.println("Biner: " + bilanganBiner);

        // Konversi ke oktal
        String bilanganOktal = Integer.toOctalString(bilanganDesimal);
        System.out.println("Oktal: " + bilanganOktal);
    }
}
