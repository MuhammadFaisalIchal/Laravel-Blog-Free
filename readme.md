Ini adalah link source code dari tutorial https://www.youtube.com/playlist?list=PLx4zY98IACXhYdrurFvLT1fhTvaEysoSt

Clone Project ini setelah selesai pada terminal masuk kedalam directory project

Ketikkan:
1. Composer Install
2. cp .env.example .env
3. php artisan key:generate
4. php artisan migrate (Jangan lupa set up database)
5. php artisan db:seed

Jika ada masalah ketika menjalankan project ini (Note project ini tidak bisa dijanlankan menggunakan php artisan serve krn bakalan kacau linknya) (Silahkan cek video part 1 dan 2 kenapa hal ini bisa terjadi)
1. Project ini sengaja merubah server.php menjadi index.php agar project dapat dijalankan langsung tanpa perlu pergi ke folder public
2. Karena hal itu maka url pada asset yang sebelumnya asset('/gambar') menjadi asset('/public/gambar')
3. Jika ingin mengembalikan ke normal ubah index.php menjadi server.php kemudian ubah semua url asset menjadi kebalikan dari nomor 2. Lalu jalankan php artisan serve (cek part 2)

Bagi yang ingin kembangkan menjadi lebih baik maka saya akan kasih beberapa clue
1. Integrasikan semua page menggunakan meta
2. Integrasikan text editor menggunakan Laravel File Manager (Silahkan cek video terbaru saya untuk tutorialnya)
3. Belajar menggunakan ajax dan datatables (Cek video terbaru saya soal ajax datatables)
4. Tambahkan captcha jika ingin hosting untuk menghindari bot pada halaman login
5. Gunakan package laravel sluggable dan integarsikan menggunakan ajax agar slug tergenerate otomatis dan menjadi unik meski judul postingan sama
6. Tambahkan opsi publish dan unpublish
7. Belajar menggunakan package laravel intevention image untuk membagi ukuran gambar sesuai dengan dimensi yang dibutuhkan ketika ditampikan pada halaman depan / halam details blog / sidebar (Gunakan berbagai macam ukuran untuk meningkatkan perfoma)
8. Belajar menggunakan lazyload
9. Belajar menggunakan webpack untuk mengecilkan ukuran css
10. Belajar menggunakan laravel query cache agar perfoma meningkat meski diakses oleh trafik yang tinggi
11. Belajarlah mengintegrasikan blog ini dengan google analystic dan buat admin panelnya (banyak package soal ini di github)
12. Belajar untuk menambahkan archieve post berdasarkan tahun
13. Belajar menambahkan iklan pada blog
14. Belajar mengembangkan landing page atau halaman home agar lebih menarik. Tampilkanlah featured Post. Postingan per kategori. Postingan terpanas dll pada sectionnya masing2 (Cluenya tinggal select where id_category == 'id_kategori' lalu lempar ke blade home trus tampikan)
15. Remove semua modules js dan css pada folder public yang tidak terpakai (Tapi terload karena pas tutorial saya mau cepet)
16. Jika udah Percaya Diri silahkan upload projectnya ke hosting masing-masing (Jangan lupa gunakan let's encript untuk https dan menghilangkan semua iklan atau hal yang gak perlu yg diinjek pada website kita)
17. Test Score website kalian menggunakan tool ini https://gtmetrix.com/
18. Semoga berhasil

Btw saya mungkin gak bisa cover semua hal diatas pada chanel saya.. tapi gak ada salahnya kan belajar mandiri?
