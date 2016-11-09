Sistem Informasi Geografis

1. Latar Belakang

Di dalam Sistem Informasi Geografis, data geospasial mempunyai beberapa fungsi atau jenis salah satunya adalah retrieve data geospasial yang akan kita bahas secara singkat.

1. Pembahasan

Retrieve data spasial bisa disebut juga sebagai manipulasi untuk melihat isi data pada data vektor. Shapefile yaitu format data geospasial yang umum untuk perangkat lunak sistem informasi geografis, diantaranya:

- .Bbox
- .Shape Type

Jumlah data Geometri

&gt;&gt; import shapefile

&gt;&gt;sf=shapefile.Reader(&quot;namefile.shp&quot;)

&gt;&gt;sf.shapes()

&gt;&gt;a=sf.shapes()

&gt;&gt;len(a)

Data DBF

&gt;&gt;import shapefile

&gt;&gt;sf.records()

&gt;&gt;sf.records(n)



1. Penutup

1. a)Kesimpulan

Retrieve data geospasial yaitu sebagai manipulasi untuk melihat isi data pada data vektor.

1. b)Saran

Untuk memahami lebih lanjut tentang Keamanan Jaringan Vulnerability alangkah lebih baiknya anda mempelajarinya di buku-buku yang terpercaya.



