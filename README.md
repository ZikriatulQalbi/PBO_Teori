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

BAB 3
Mengenal Lingkup Pemrograman Anda
1. Hello World!
public class ZikriatulTgs_2201081013 {

    public static void main(String[] args) {
        System.out.println("Hello Word,Welcom to java Programing Zikriatul Qalbi");
    }
    
}

Fungsi dari setiap baris kode adalah sebagai berikut:
public static void main(String[] args): Ini adalah deklarasi metode utama yang akan dieksekusi ketika program dijalankan. Ini adalah titik awal eksekusi program.
System.out.println("Hello Word,Welcom to java Programing Zikriatul Qalbi");: Ini adalah perintah untuk mencetak teks ke konsol. Metode println() mengambil argumen teks yang ingin dicetak, dan mencetaknya ke konsol dengan baris baru di akhir.
Jadi, fungsi dari kode ini adalah mencetak pesan sambutan ke konsol ketika program dijalankan.

2. The Tree
public class theTree {
    
        public static void main(String[]args){
            System.out.println("I think that shall never see,");
            System.out.println("a poem as lovely as a tree.");
            System.out.println("A tree whose hungry mouth is pressed");
            System.out.println("Againts the Earth's sweet flowing breast.");
        }
    
}

Fungsi dari setiap baris kode adalah sebagai berikut:
public static void main(String[]args){: Ini adalah deklarasi metode utama yang akan dieksekusi ketika program dijalankan. Ini adalah titik awal eksekusi program.
System.out.println("I think that shall never see,");: Ini adalah perintah untuk mencetak teks "I think that shall never see," ke konsol, diikuti dengan baris baru.
System.out.println("a poem as lovely as a tree.");: Ini adalah perintah untuk mencetak teks "a poem as lovely as a tree." ke konsol, diikuti dengan baris baru.
System.out.println("A tree whose hungry mouth is pressed");: Ini adalah perintah untuk mencetak teks "A tree whose hungry mouth is pressed" ke konsol, diikuti dengan baris baru.
System.out.println("Againts the Earth's sweet flowing breast.");: Ini adalah perintah untuk mencetak teks "Againts the Earth's sweet flowing breast." ke konsol, diikuti dengan baris baru.
Jadi, fungsi dari kode ini adalah mencetak beberapa baris teks dari puisi ke konsol. Puisi ini adalah "Trees" karya Joyce Kilmer.

          BAB 4
Dasar-Dasar Pemrograman
Latihan
1.Mendeklarasikan dan Mencetak Variabel

public class DeklarasiDanCetakVariabel {

    public static void main(String[] args) {
        int number = 10;
        char letter = 'a';
        boolean result = true;
        String str = "hello";
        
        System.out.println("Number : "+number);
        System.out.println("Letter : "+letter);
        System.out.println("Result : "+result);
        System.out.println("Str :"+str);
        
        
    }
    
}

2.Mendapatkan Nilai Rata-rata Dari Tiga Angka

public class MenampilkanNilaiTerbesar {
    public static void main(String[] args){
        int number1=10;
        int number2=23;
        int number3=5;
        int nilai = 0;
        
        nilai = (number2 > number3)? (number2 > number1)? number2:number1:number3;
        
        System.out.println("Number1 : "+number1);
        System.out.println("Number2 : "+number2);
        System.out.println("Number3 : "+number3);
        System.out.println("Nilai Tertinggi : "+nilai);
        
    }
    
}

3.Menampilkan Nilai Terbesar

public class MendapatkanNilaiRata_rata_dariTigaAngka {
    public static void main(String[] args){
        int number1=10;
        int number2=20;
        int number3=45;
        int fathy=(number1+number2+number3)/3;
        
        System.out.println("Number1 : "+number1);
        System.out.println("Number2 : "+number2);
        System.out.println("Number3 : "+number3);
        System.out.println("Avarage is : "+fathy);
                
    }
    
}

4.Operator Precedence

public class OperatorPrecedence {
    public static void main(String[] args){
        System.out.println("1. a / b ^ c ^ d - e + f - g * h + i ");
        System.out.println("2. 3 * 10* 2 / 15 - 2 + 4 ^ 2 ^ 2 ");
        System.out.println("3. r ^ s * t / u - v + w ^ x - y++");
    }
    
}
