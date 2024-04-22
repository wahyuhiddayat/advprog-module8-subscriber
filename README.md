***1. what is amqp?***

AMQP, atau Advanced Message Queuing Protocol, adalah sebuah protokol open standard untuk message-oriented middleware yang memiliki tujuan untuk memastikan pesan dapat dikirimkan secara andal dan aman. Protokol ini mendukung sejumlah fitur penting seperti message orientation, queuing, routing (melalui direct exchange, topic exchange, dan lain-lain), reliability dan security. AMQP sangat berguna dalam kasus dimana aplikasi yang berjalan di lokasi atau platform yang berbeda perlu berkomunikasi satu sama lain secara efisien dan dapat diandalkan.

***2. what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?***

`guest:guest@localhost:5672` merupakan sebuah URI (Uniform Resource Identifier) yang digunakan untuk mengkoneksikan client ke server message broker yang mendukung AMQP. Di sini:
- `guest:guest` adalah username dan password yang digunakan untuk autentikasi dengan broker. Dalam hal ini, "guest" yang pertama adalah username dan "guest" yang kedua adalah password. Biasanya, ini adalah nilai default yang digunakan RabbitMQ, salah satu broker populer yang mendukung AMQP.
- `localhost` adalah hostname di mana broker AMQP berjalan. "localhost" secara spesifik merujuk ke mesin lokal dari pengguna, yang berarti server berjalan pada komputer yang sama dengan client.
- `5672` adalah port di mana broker AMQP mendengarkan koneksi. Ini adalah port default untuk koneksi klien ke RabbitMQ tanpa menggunakan enkripsi SSL/TLS.

Secara keseluruhan, string koneksi ini digunakan untuk menentukan bagaimana aplikasi harus terhubung ke broker AMQP untuk mengirim dan menerima pesan dalam cara yang efisien dan terkontrol.