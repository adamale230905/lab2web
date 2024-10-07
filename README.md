Buatlah dokumen HTML seperti berikut
![Screenshot (35)](https://github.com/user-attachments/assets/8ca90a5b-c590-4849-8751-a946922953ba)

Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen
![Screenshot (36)](https://github.com/user-attachments/assets/31ac7e82-1fa1-4e1c-a19b-88c8f945a3f1)

Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
![Screenshot (37)](https://github.com/user-attachments/assets/a9c3ac1a-912e-4bc9-bb1d-51cf33cff02d)

Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>
![Screenshot (39)](https://github.com/user-attachments/assets/bae046e0-63d6-41d3-a8c7-500fbccfffff)

Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.
![Screenshot (38)](https://github.com/user-attachments/assets/8f6f62d7-078e-483b-bb7e-8a315f53cd77)

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )

jawaban:
1.	Perbedaan antara h1 {...} dan #intro h1 {...}
      •	h1 {...} adalah selector elemen yang akan mempengaruhi SEMUA elemen h1 di halaman web
      •	#intro h1 {...} adalah selector yang lebih spesifik, hanya mempengaruhi elemen h1 yang berada di dalam elemen dengan id "intro"
2.	Prioritas antara Internal CSS, External CSS, dan Inline CSS
      prioritas CSS dari tertinggi ke terendah:
      1.	Inline CSS
      2.	Internal CSS
      3.	External CSS
      Dalam contoh di atas, teks akan berwarna MERAH karena inline CSS memiliki prioritas tertinggi, meskipun ada deklarasi warna berbeda di internal dan external CSS.
3.	Prioritas antara ID dan Class Selector
      •	ID selector (#paragraf-1) memiliki prioritas lebih tinggi dibandingkan Class selector (.text-paragraf)
      •	Dalam contoh di atas, teks akan berwarna MERAH dan ukuran font 14px, mengikuti style dari ID selector
      •	Ini karena ID bersifat unik dan lebih spesifik dibandingkan Class
  	.Secara umum, urutan prioritas CSS (specificity) dari tinggi ke rendah adalah:
      .	Inline styles
      .	ID selectors
      .	Class selectors, attributes selectors, dan pseudo-classes
      .	Element selectors dan pseudo-elements
