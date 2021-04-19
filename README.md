# Web-Indexing-Project
# Web-Indexing-Project

Ana Sayfa

<img src= "https://user-images.githubusercontent.com/50086295/115256302-c5e00c00-a137-11eb-8df9-e097fdf9a82d.jpeg" width=300>

1-Frekans Hesaplama

Kullanıcının girdiği URL adresine gidilerek site içerisindeki kelimelerin frekansları bulunmuştur.

<img src= "https://user-images.githubusercontent.com/50086295/115256819-3c7d0980-a138-11eb-8c3e-25429a1f16d5.jpeg" width=300>

2-Anahtar Kelime Bulma

Kullanıcının girdiği URL adresine ulaşılarak bu adresteki en çok tekrar eden, bağlaç olmayan ve kelime uzunluğu ikiden fazla olan 10 anahtar kelime yazdırılmıştır.

<img src= "https://user-images.githubusercontent.com/50086295/115257078-71895c00-a138-11eb-86ae-4a1e2351307c.jpeg" width=300>

3- Benzerlik Skorlaması

Kullanıcından alınan 2 URL için ilk girilen URL içeriğine ulaşılarak anahtar kelimelerin çıkarılmasıyla ikinci girilen URL içerisinde bu anahtar kelimelerin frekansları bulunmuş ve buna göre bir skor hesaplanmıştır.Bu hesaplamada kullanılan formül ise ana url içerindeki anahtar kelimelerin frekans toplamları F1, ana url içerisindeki toplam kelime frekansları F2, ikinci girilen URL adresteki ana URL ile belirlediğimiz anahtar kelimelerin bu adresteki frekanslarının toplamı F3, ikinci URL adresinde bulunan toplam kelime frekansları F4 ise skor hesabı:
100*((100*F3)/F4))/((100*F1)/F2)  olarak hesaplanır. 

<img src= "https://user-images.githubusercontent.com/50086295/115257081-73531f80-a138-11eb-9d61-88e53b21dadb.jpeg" width=300>

4-Site İndeksleme ve Sıralama

Kullanıcıdan URL ve web kümesi alındıktan sonra girdiği URL adresinin içeriğine ulaşılarak anahtar kelimeler belirlenmiştir. Belirlenen anahtar kelimeler web kümesinde bulunan her bir adresin içeriğine erişilip arama işlemi yapılarak frekansları bulunmuştur.
Ardından bu web kümesindeki her bir link içerisinden max 5 link seçilmiş ve ana url içerisindeki anahtar kelime frekansları adres içerikleri içerisinde arama işlemiyle frekans sayılarına ulaşılmıştır.
Daha sonra  web kümesi içerisindeki her bir link için elde edilen max 5 URL’den max 5’er link seçilmiş ve toplamda web kümesindeki bir link için max 25 link olacak şekilde derinlik oluşturulmuş ve ana url anahtar kelimeleri bu linklerde de aranarak web kümesindeki bir link skorlama formülü ile hesaplaması yapılmıştır.

<img src= "https://user-images.githubusercontent.com/50086295/115257094-751ce300-a138-11eb-8f29-9347aa6f59a1.jpeg" width=300>

5-Sematik Analiz

Kullanıcıdan URL ve web kümesi alındıktan sonra girdiği URL adresinin içeriğine ulaşılarak anahtar kelimeler belirlenmiştir
Anahtar kelimeler eş anlamlara içeren synonyms.txt dosyasında arama işlemi yapılarak eş anlamlıları belirlendikten sonra bu kelimelerde anahtar kelime dizisine dahil edilmiş ve tüm katmanlarda bu eş anlamlı kelimelerde aratılarak  bir önceki aşamada yapılan işlemler tekrarlanmış ve skorlama işlemi yapılmıştır.


<img src= "https://user-images.githubusercontent.com/50086295/115257101-764e1000-a138-11eb-9dc3-592944c5306f.jpeg" width=300>


PROJE ÇALIŞTIRILMASI:

İlk olarak tarayıcınıza Moesif CORS uzantısı eklemeniz gerekmektedir.

Daha sonra proje dosyasını  indirip  zip içerisinden çıkararak kullanılacak IDE'ye import ediniz . Ardından uygulamanın giriş sayfasını içeren index0.html dosyası seçerek kullandığınız IDE'ye göre Open with  Browser işlemi yaparak tarayıcınızda çalıştırınız. Her aşama için oluşturulmuş butonlara tıklayarak istediğiniz sayfaya erişebilirsiniz.
