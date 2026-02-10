# Reflection 1

## Coding Standards

### 1. Clean Code
- <b>Meaningful Names</b>

    Mayoritas nama variabel dan fungsi sudah mengikuti standar ini. Contohnya `ProductRepository` untuk menyatakan repositori produk dan `ProductService` untuk menyatakan <i>service</i> yang digunakan untuk keperluan CRUD.

- <b>Functions</b>
    
    Dalam banyak kasus, terdapat fungsi-fungsi yang tersebar di <i>codebase</i>.

    Fungsi yang dibuat melaksanakan hanya satu pekerjaan. Contohnya `create` pada `ProductServiceImpl` hanya menjalankan fungsi membuat produk. 
    
    Command-query separation juga dilakukan dengan menerapkan <i>getter</i> dan <i>setter</i> pada model `Product`.

- <b>Comments</b>

    Penggunaan <i>comments</i> tidak diperlukan selama kode menjelaskan dirinya sendiri (<i>self-explanatory</i>). Hal ini mengurangi kemungkinan terjadinya redundansi.

- <b>Objects and Data Structure</b>

    Objek `Product` memiliki variabel-variabel yang bersifat <i>private</i> untuk alasan keamanan.

- <b>Error Handling</b>

    Error handling tidak secara eksplisit diimplementasikan di projek ini.

### 2. Git Flow

- <b>Feature Branch Workflow</b>

    Setiap fitur yang dikembangkan memiliki <i>branch</i> tersendiri. Hal ini menjadikan <i>workflow</i> menjadi lebih terstruktur dan membantu jika terjadi sebuah kesalahan.

### 3. Secure Coding

- Untuk saat ini, belum ada banyak <i>secure coding principles</i> yang diterapkan.

## Future Improvements

- `GetMapping` yang digunakan untuk POST dan DELETE. Padahal ada `PostMapping` dan `DeleteMapping` yang terdapat di Spring Boot.
