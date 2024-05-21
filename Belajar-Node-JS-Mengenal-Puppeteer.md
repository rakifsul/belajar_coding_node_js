# Belajar Node JS Mengenal Puppeteer

## Source Code Project Ini

https://github.com/rakifsul/belajar_coding_node_js/tree/main/contoh_nodejs_puppeteer

## Pendahuluan

Setelah Anda belajar tentang Axios pada "[Belajar Node JS Mengenal Axios](https://github.com/rakifsul/belajar_coding_node_js/blob/main/Belajar-Node-JS-Mengenal-Axios.md)", mungkin Anda akan menyadari sesuatu.

Yakni, isi HTML yang diperoleh melalui Axios tadi masih bisa diolah.

Dengan library tertentu, mengekstrak data berharga dari HTML yang dikembalikan bisa dilakukan dengan mudah.

TAPI... itu dengan asumsi bahwa data berharga tersebut ada di HTML nya, bukan tersembunyi dalam JavaScript.

Lalu, bagaimana dengan halaman web yang kontennya dinamis, dalam artian hanya tampil setelah diolah dengan JavaScript?

Jawabannya ada pada Puppeteer.

Puppeteer itu sendiri mengandalkan web browser untuk melakukan perolehan data.

Analoginya:

-   Data yang dikembalikan dari Axios menyerupai browser view source.
-   Data yang dikembalikan dari Puppeteer menyerupai browser inspect element.

Di artikel ini, saya akan memberikan contoh sederhana untuk menggunakan Puppeteer.

## Lebih Lanjut tentang Puppeteer

Puppeteer adalah sebuah library Node.js yang dikembangkan oleh tim Google Chrome.

Ini memungkinkan otomatisasi browser headless (tanpa UI) melalui antarmuka yang ramah pengembang.

Berikut adalah beberapa poin penting tentang Puppeteer:

-   Automasi Browser: Puppeteer memungkinkan Anda mengendalikan browser Chrome atau Chromium secara programatik melalui JavaScript. Anda dapat mengotomatiskan interaksi seperti klik, isi formulir, navigasi, dan lainnya.
-   Headless Mode: Salah satu fitur utama dari Puppeteer adalah kemampuannya untuk menjalankan browser dalam mode tanpa kepala (headless). Ini berarti browser tidak akan memiliki antarmuka pengguna grafis (GUI), yang membuatnya lebih efisien untuk menjalankan skrip otomatisasi di latar belakang.
-   Testing Otomatis: Puppeteer sangat berguna untuk pengujian otomatis di situs web. Anda dapat mengotomatiskan serangkaian aksi pengguna untuk menguji fungsi dan kinerja situs web Anda.
-   Web Scraping: Dengan menggunakan Puppeteer, Anda dapat melakukan web scraping, yaitu mengekstrak data dari halaman web secara otomatis. Ini dapat berguna untuk mengumpulkan informasi dari situs web yang tidak menyediakan API.
-   Rendering dan Screenshot: Puppeteer dapat digunakan untuk merender halaman web dan mengambil tangkapan layar (screenshot). Ini berguna jika Anda perlu membuat laporan visual atau melakukan pemantauan visual terhadap perubahan pada situs web.
-   Deteksi dan Bypass CAPTCHA: Dengan menggunakan Puppeteer, Anda dapat memprogram agar melakukan navigasi ke halaman web yang membutuhkan CAPTCHA, dan dalam beberapa kasus, Anda bahkan dapat membuat skrip yang secara otomatis memecahkan CAPTCHA.
-   Dukungan untuk Chrome DevTools Protocol: Puppeteer dibangun di atas protokol DevTools Chrome, yang memberikan kontrol penuh terhadap perilaku browser. Ini memungkinkan Anda untuk melakukan debugging, analisis, dan optimisasi performa.

Keseluruhan, Puppeteer adalah alat yang sangat kuat dan fleksibel untuk mengotomatisasi interaksi dengan browser, baik untuk pengujian otomatis, web scraping, atau tujuan lainnya.

## Tujuan

Tujuan dari artikel ini adalah:

-   Pembaca mengenal Puppeteer.
-   Pembaca mampu mencoba menggunakan Puppeteer.

## Prasyarat

Berikut ini adalah prasyarat dari tutorial ini:

-   Menggunakan sistem operasi Windows 10 ke atas.
-   Men-download dan meng-install Node.js dan NPM.
-   Bisa mengakses Node.js dan NPM dari PowerShell di folder manapun.
