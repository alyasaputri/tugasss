# Jawaban Pertanyaan Tugas Reinforcement Learning

## 1. Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?

* **State** adalah kondisi atau posisi agent pada suatu lingkungan. Pada FrozenLake, state menunjukkan posisi agent pada kotak tertentu di peta.
* **Action** adalah tindakan yang dapat dilakukan agent untuk berpindah state. Pada FrozenLake terdapat 4 action yaitu Up, Down, Left, dan Right.
* **Reward** adalah nilai umpan balik yang diterima agent setelah melakukan action. Reward digunakan sebagai indikator apakah tindakan yang dilakukan sudah benar atau belum.

## 2. Apa fungsi dari Learning Rate (α)?

Learning Rate (α) berfungsi untuk mengatur seberapa besar informasi baru digunakan untuk memperbarui nilai pada Q-Table. Nilai α yang besar membuat agent belajar lebih cepat, sedangkan nilai α yang kecil membuat pembelajaran lebih stabil namun lebih lambat.

## 3. Apa fungsi dari Discount Factor (γ)?

Discount Factor (γ) berfungsi untuk menentukan seberapa penting reward di masa depan dibandingkan reward saat ini. Semakin besar nilai γ, maka agent akan lebih mempertimbangkan keuntungan jangka panjang dalam menentukan tindakan terbaik.

## 4. Mengapa digunakan metode Exploration dan Exploitation?

* **Exploration** digunakan agar agent mencoba berbagai kemungkinan tindakan sehingga dapat menemukan jalur atau strategi yang lebih baik.
* **Exploitation** digunakan agar agent memanfaatkan pengalaman yang sudah dipelajari dengan memilih action yang memiliki nilai Q paling tinggi.

Kombinasi keduanya penting agar agent tidak hanya mencoba-coba terus menerus, tetapi juga dapat memanfaatkan pengetahuan yang telah diperoleh selama training.

## 5. Bagaimana perubahan nilai reward setelah training 2000 episode?

Pada awal training, reward yang diperoleh agent masih rendah karena agent belum memahami jalur menuju goal. Setelah training sebanyak 2000 episode, nilai reward cenderung meningkat dan lebih stabil. Hal ini menunjukkan bahwa agent telah berhasil mempelajari jalur terbaik menuju tujuan (Goal). Dari hasil testing diperoleh Total Reward = 1 yang menandakan agent berhasil mencapai goal pada FrozenLake.

Modifikasi program sehingga:

Menggunakan environment Taxi-v3 Menampilkan rata-rata reward setiap 100 episode Membandingkan hasil training 1000, 2000, dan 5000 episode
Pada tugas lanjutan ini, program Q-Learning dimodifikasi dengan menggunakan environment Taxi-v3, yaitu simulasi taksi yang bertugas menjemput dan mengantarkan penumpang ke tujuan yang benar. Selama proses training, ditampilkan rata-rata reward setiap 100 episode untuk melihat perkembangan kemampuan agent dalam belajar. Selain itu, dilakukan perbandingan hasil training pada 1000, 2000, dan 5000 episode untuk mengetahui pengaruh jumlah latihan terhadap performa agent. Semakin banyak episode yang digunakan, biasanya nilai reward akan semakin baik dan stabil karena agent memiliki lebih banyak pengalaman dalam menentukan tindakan terbaik. Dengan demikian, agent dapat menemukan strategi yang lebih optimal untuk menyelesaikan tugas pada environment Taxi-v3.
<img width="1202" height="1406" alt="image" src="https://github.com/user-attachments/assets/be7b5be2-8bb9-4fcb-9582-61c83d475a61" />
<img width="920" height="1368" alt="image" src="https://github.com/user-attachments/assets/f3f05e84-2823-4fe8-a932-90376fec8c9c" />
<img width="1144" height="1386" alt="image" src="https://github.com/user-attachments/assets/bf111c65-d9a1-4e58-9b7d-a66fd698dd20" />


