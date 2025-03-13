# Performance Testing and Profiling

## Before Optimization

/all-students before profiling.
![/all-students 1 - Before](./images/before-1-1.jpg)

![/all-students 2 - Before](./images/before-1-2.jpg)

![/all-students 3 - Before](./images/before-1-3.jpg)

![/all-students 4 - Before](./images/before-1-4.jpg)

/all-student-name before profiling.
![/all-student-name 1  -  Before](./images/before2-1.jpg)

![/all-student-name 2  -  Before](./images/before2-2.jpg)

![/all-student-name 3  -  Before](./images/before2-3.jpg)

![/all-student-name 4  -  Before](./images/before2-4.jpg)

/highest-gpa before profiling.
![/highest-gpa 1 - Before](./images/before-3-1.jpg)

![/highest-gpa 2 - Before](./images/before-3-2.jpg)

![/highest-gpa 3 - Before](./images/before-3-3.jpg)

![/highest-gpa 4 - Before](./images/before-3-4.jpg)

Using Command Line:

/all-students before profiling.
![/all-students CLI  -  Before](./images/beforecli-1.jpg)

/all-student-name before profiling.
![/all-student-name CLI  -  Before](./images/beforecli-2.jpg)

/highest-gpa before profiling.
![/highest-gpa CLI  -  Before](./images/beforecli-3.jpg)

## After Optimization

/all-students after profiling.
![/all-students 1 - After](./images/after-1-1.jpg)

![/all-students 2 - After](./images/after-1-2.jpg)

![/all-students 3 - After](./images/after-1-3.jpg)

![/all-students 4 - After](./images/after-1-4.jpg)

/all-student-name after profiling.
![/all-student-name 1 - After](./images/after-2-1.jpg)

![/all-student-name 2 - After](./images/after-2-2.jpg)

![/all-student-name 3 - After](./images/after-2-3.jpg)

![/all-student-name 4 - After](./images/after-2-4.jpg)

/highest-gpa after profiling.
![/highset-gpa 1 - After](./images/after-3-1.jpg)

![/highset-gpa 2 - After](./images/after-3-2.jpg)

![/highset-gpa 3 - After](./images/after-3-3.jpg)

![/highset-gpa 4 - After](./images/after-3-4.jpg)

Using Command Line:

/all-students after profiling.
![/all-students CLI - After](./images/after-cli-1.jpg)

/all-student-name after profiling.
![/all-student-name CLI - After](./images/after-cli-2.jpg)

/highest-gpa after profiling.
![/highest-gpa CLI - After](./images/after-cli-3.jpg)

## Conclusion

Berdasarkan perbandingan hasil JMeter sebelum dan sesudah melakukan profiling, kita menemukan bahwa kecepatan eksekusi request dari kedua implementasi sangatlah berbeda. Hal ini terutama dapat dilihat pada implementasi function getAllStudentCourses (endpoint all-student), di mana sebelum melakukan profiling waktu yang dibutuhkan berkisar pada angka 72.000 ms, tetapi setelah dilakukan profiling angka ini turun secara signifikan ke kisaran 3.500-4.000 ms. Hal ini menunjukkan penurunan waktu eksekusi sebesar 94-95% yang tentunya akan sangat berpengaruh terhadap suatu aplikasi. Kemudian, hal yang sama juga terjadi pada dua function lainnya yaitu findStudentWithHighestGpa (highest-gpa) yang berubah dari rata-rata 220 ms menjadi 88 ms, menunjukkan penurunan waktu eksekusi sebesar 60%. Terakhir, terdapat fungsi joinStudentNames (endpoint all-student-name), di mana terjadi penurunan dari rata-rata 1688 ms menjadi 193 ms, menunjukkan penurunan sebesar 88%. Dengan demikian, kita dapat menyimpulkan bahwa proses optimasi dengan memanfaatkan profiling terbukti efektif dalam meningkatkan performa dari sistem secara keseluruhan tanpa mengubah fungsionalitas yang ada. 