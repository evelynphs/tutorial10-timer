# Tutorial 10

### 1.2. Understanding how it works

![1.2](images/experiment_1.2.png)
Pada program kali ini, "Epel's computer: hey hey" di-print sebelum "Epel's computer: howdy!" dan "Epel's computer: done!". Ini terjadi karena `println!("Epel's computer: hey hey");` berada di luar `spawner.spawn` dan dijalankan sebelum `executor.run();`. Teks "Epel's computer: howdy!" dan "Epel's computer: done!" berada di dalam `spawner.spawn` dan baru akan di-print ketika `executor.run();` dijalankan, sehingga teks tersebut di-print setelah "Epel's computer: hey hey".
