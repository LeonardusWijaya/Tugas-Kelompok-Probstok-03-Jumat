A STOCHASTIC PROCESS FOR WORD FREQUENCY

Tugas Kelompok Mata Kuliah Probabilitas dan Proses Stokastik 03
Hosea Yoarana (1706042913)
Leonardus Wijaya (1706042945)
Nathanael Tristan Bramantyo (1706042900)

================================================================================================================================

Markovian Process and Markov Chain
Various models for word frequency distributions have been developed since Zipf (1935) applied the zeta distribution to describe a wide range of lexical data. Mandelbrot (1953, 1962)extended Zipf's distribution 'law'

PROBLEM
There is a growing consensus in psycholinguistic research that word recognition depends not only on properties of the target word (e.g. its length and frequency), but also upon the number and nature of its lexical competitors or neighbors. Landauer and Streeter observed that (1) highfrequency words have more neighbors than lowfrequency words (the neighborhood density effect), and that (2) high-frequency words have higher-frequency neighbors than low-frequency words (the neighborhood frequency effect). 

MODELING
By themselves, models of the kind proposed by Zipf, Herdan and Muller or Sichel, even though they may yield reasonable fits to particular word frequency distributions, have no bearing on the similarity relations in the lexicon. The only model that is promising in this respect is that of Mandelbrot (1953, 1962). Mandelbrot derived his modification of Zipf's law (2) on the basis of a Markovlan model for generating words as strings of letters, in combination with some assumptions concerning the cost of transmitting the words generated in some optimal code, giving a precise interpretation to Zipf's 'law of abbreviation'.

Secara garis besar paper tersebut mengatakan bahwa penggunaan kata dan kalimat dalam kehidupan sehari – hari memiliki pattern yang sama tidak terikat pada Bahasa apa yang sedang digunakan. Teori Shannon and Weaver Model of communication. Dikatakan bahwa human communication is not mathematical in nature(1949). Komunikasi antar manusia pada hakikatnya adalah sebuah paduan antara randomness dan statistical dependencies. Sebagai contoh sebuah kata akan erat hubungannya dengan kata sebelumnya sampai batas tertentu.

Misalnya ada banyak huruf seperti ini :
A b a c a c a a b a c a b a b c a c a a
Dari huruf diatas terlihat bahwa a lebih sering untuk berkumpul menjadi a a daripada b atau c.
Menggunakan markov chain. Kemudian kita dapat membuat hal yang serupa dengan memasukkan huruf a b c dalam suatu gelas dan mengambilnya secara random satu per satu sampai membuat similar – looking string atau zero-order approximation. Akan tetapi dengan menggunakan Teknik ini akan sulit untuk mendapatkan hal yang mirip dengan string diatas. Oleh karena itu kita dapat menggunakan cara yang lebih baik dengan cara first-order approximation dimana huruf dipilih secara random akan tetapi sesuai dengan probabilitas setiap huruf, sehingga huruf a jumlahnya akan lebih banyak dibanding dengan b atau c. 

Setelah itu ada cara yang lebih baik lagi adalah dengan second-order approximation yaitu memasangkan antar huruf namun perlu kesesuaian dengan probabilitas setiap huruf. Sehingga dapat dibuat seperti berikut :
AA AB AA AA AC 
BC BA BB
CB CA CC
Hasil string dari second-order akan lebih mirip dengan string awal yang kita gunakan.
Dari sini kita dapat one step further dengan menggunakan third-order approximation yaitu dengan membuat grup dari 3 huruf atau trigrams dan disini kita akan membutuh kan 9 state.
AAA AAB AAC dst
BBA BBB BBC dst
CCA CCB CCC dst
Dan akan didapatkan string yang sama dengan yang digunakan di awal.
