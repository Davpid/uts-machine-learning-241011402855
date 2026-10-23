# uts-machine-learning-241011402855
repositori ini dibuat untuk memenuhi tugas UTS mata kuliah Machine Learning

Nama : David Paskah
Kelas : 05TPLM001
NIM   : 241011402855


Pada bagian A - Linear Regression
Diperoleh persamaan regresi linear dengan koefisien sebesar 8,9558 dan intercept 29,5113, yang menunjukkan bahwa setiap kenaikan biaya iklan Rp1 juta diperkirakan meningkatkan penjualan sekitar Rp8,96 juta serta hubungan keduanya bersifat positif. Model memiliki performa yang baik dengan RMSE training 5,98 dan testing 6,26 serta nilai R² masing-masing 93,78% dan 94,25%, sehingga sebagian besar variasi penjualan dapat dijelaskan oleh biaya iklan dan model mampu melakukan prediksi secara akurat. 
Pada proses Gradient Descent, learning rate 0,001 berhasil konvergen namun lambat, learning rate 0,02 menjadi yang paling optimal karena menghasilkan MSE terendah dan konvergen secara stabil, sedangkan learning rate 0,1 gagal konvergen akibat pembaruan parameter yang terlalu besar hingga menghasilkan nilai NaN. Selain itu, prediksi penjualan untuk biaya iklan Rp12 juta sebesar 136,98 termasuk ekstrapolasi karena berada di luar rentang data pengamatan, sehingga meskipun model memiliki akurasi tinggi, hasil prediksi tersebut perlu diinterpretasikan dengan lebih hati-hati.

Pada bagian B - Logistic Regression
Model Logistic Regression berhasil konvergen dengan baik yang ditunjukkan oleh nilai log loss yang terus menurun hingga stabil pada iterasi akhir. Model mampu memisahkan sebagian besar data Spam dan Bukan Spam dengan akurat berdasarkan decision boundary, meskipun masih terdapat satu data yang salah diklasifikasikan karena berada sangat dekat dengan batas keputusan. Dalam konteks filter spam, false positive dianggap lebih merugikan dibanding false negative karena dapat menyebabkan email penting masuk ke folder spam dan tidak terbaca oleh pengguna. Selain itu, perubahan threshold memengaruhi keseimbangan antara precision dan recall, di mana threshold rendah cenderung meningkatkan recall tetapi menurunkan precision, sedangkan threshold tinggi meningkatkan precision tetapi menurunkan recall. Oleh karena itu, threshold 0,5 umumnya digunakan sebagai nilai yang seimbang, sementara pemilihan threshold terbaik perlu disesuaikan dengan tujuan sistem dan dampak kesalahan klasifikasi yang ingin diminimalkan.
