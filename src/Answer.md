Output:
Televisi dihidupkan
volume menjadi 10
volume di set ke 7
TV menjadi TRANS7
Televisi dimatikan

Pada baris tersebut, objek dibuat untuk mengimplementasikan antarmuka kontrolTv dengan menggunakan kelas televisi.
- kontrolTv adalah sebuah antarmuka (interface) yang menentukan kontrak metode yang harus diimplementasikan oleh kelas yang menggunakan antarmuka tersebut. Dalam kasus ini, antarmuka kontrolTv memiliki empat metode: hidupkan, pindahChannel, keraskanVolume, dan pelankanVolume.
- televisi adalah kelas yang mengimplementasikan antarmuka kontrolTv. Ini berarti bahwa kelas televisi harus menyediakan implementasi untuk keempat metode yang didefinisikan dalam antarmuka kontrolTv.
Pada baris kontrolTv tvku = new televisi("SHARP");, kita membuat objek tvku dari kelas televisi dan menginisialisasi objek dengan konstruktor televisi yang menerima satu parameter bertipe String (yaitu merek televisi). Dalam hal ini, merek televisi yang diberikan adalah "SHARP".
Objek tvku memiliki tipe data kontrolTv, yang berarti kita hanya dapat memanggil metode-metode yang didefinisikan dalam antarmuka kontrolTv pada objek tersebut. Meskipun demikian, karena kelas televisi mengimplementasikan antarmuka kontrolTv, metode-metode tersebut akan memiliki implementasi yang sesuai dalam kelas televisi.

Dalam kode di atas, objek tidak dapat langsung diinisialisasi dengan antarmuka (interface) karena antarmuka tidak dapat diinstansiasi secara langsung. Namun, kita dapat membuat objek dari kelas yang mengimplementasikan antarmuka tersebut.
Dalam contoh ini, antarmuka kontrolTv diimplementasikan oleh kelas televisi. Jadi, kita bisa membuat objek dari kelas televisi dan menginisialisasinya dengan menggunakan konstruktor kelas tersebut.
Berikut adalah contoh cara menginisialisasi objek tvku dengan antarmuka kontrolTv menggunakan kelas televisi:
kontrolTv tvku = new televisi("SHARP");
Dalam kode di atas, kita membuat objek tvku dengan tipe data kontrolTv dan menginisialisasinya dengan menggunakan konstruktor televisi. Parameter yang diberikan ke konstruktor adalah merek televisi, dalam contoh ini "SHARP".
Setelah objek tvku terbuat, kita dapat memanggil metode-metode yang didefinisikan dalam antarmuka kontrolTv pada objek tersebut. Misalnya:
tvku.hidupkan(true);
tvku.keraskanVolume(10);
tvku.pelankanVolume(3);
tvku.pindahChannel(5);
tvku.hidupkan(false);
Dalam contoh di atas, kita memanggil metode-metode hidupkan, keraskanVolume, pelankanVolume, dan pindahChannel pada objek tvku yang merupakan objek dari kelas televisi yang mengimplementasikan antarmuka kontrolTv.

===========================================================================

Output:
Televisi dihidupkan
TV terkoneksiInternet
volume menjadi 10
Televisi dimatikan

Baris "public class televisi2 implements kontrolTv, komputer" pada class televisi2 menunjukkan bahwa class tersebut mengimplementasikan dua buah interface, yaitu kontrolTv dan komputer. Dengan menggunakan kata kunci implements, class televisi2 menyatakan bahwa ia akan menyediakan implementasi dari semua metode yang didefinisikan dalam kedua interface tersebut.
Dalam konteks ini, class televisi2 akan mengimplementasikan metode-metode yang didefinisikan dalam interface kontrolTv dan komputer. Sebagai contoh, metode-metode seperti hidupkan, pindahChannel, keraskanVolume, pelankanVolume, dan konekInternet harus diimplementasikan dalam class televisi2.
Dengan menggunakan implementasi interface, class televisi2 dapat memberikan definisi konkret untuk setiap metode dalam interface, sehingga dapat digunakan untuk mengontrol televisi dan menghubungkannya ke internet.

Dalam class televisi2, terdapat beberapa behavior yang diimplementasikan dari interface kontrolTv dan komputer. Berikut adalah penjelasan tentang setiap behavior tersebut:
Dari interface kontrolTv:
- hidupkan(boolean hidup): Metode ini digunakan untuk menghidupkan atau mematikan televisi. Jika parameter hidup bernilai true, maka televisi akan dihidupkan. Jika bernilai false, maka televisi akan dimatikan.
- pindahChannel(int channel): Metode ini digunakan untuk mengubah saluran/channel pada televisi. Parameter channel digunakan untuk menentukan saluran yang akan dipilih. Saluran saluran yang tersedia ditentukan dalam array saluran.
- keraskanVolume(int tambah): Metode ini digunakan untuk meningkatkan volume televisi. Parameter tambah menentukan jumlah penambahan volume.
- pelankanVolume(int kurangi): Metode ini digunakan untuk mengurangi volume televisi. Parameter kurangi menentukan jumlah pengurangan volume.
Dari interface komputer:
- konekInternet(boolean konek): Metode ini digunakan untuk menghubungkan atau memutuskan koneksi internet pada televisi. Jika parameter konek bernilai true, maka televisi akan terkoneksi dengan internet. Jika bernilai false, maka koneksi internet pada televisi akan terputus.
Dengan mengimplementasikan kedua interface tersebut, class televisi2 dapat mengendalikan televisi seperti menghidupkan atau mematikannya, mengubah saluran/channel, meningkatkan atau mengurangi volume, serta menghubungkan atau memutuskan koneksi internet pada televisi.