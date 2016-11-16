Sistem Informasi Geografis – Create Shapefile

1. Latar Belakang

Shapefile adalah bagian dari vektor dalam Sistem Informasi Geografis. Vektor dibagi menjadi empat yaitu, .shp, .dbf, .shx, dan .prj.

1. Pembahasan

Berikut adalah langkah membuat shapefile

&gt;&gt;Import Shapefile

&gt;&gt;a=shapefile.writer()

&gt;&gt;a.point(x,y)

&gt;&gt;a.poly([x,y],[x,y])

&gt;&gt;a.field(&#39;namefolder&#39;,&#39;C&#39;,&#39;4&#39;)

&gt;&gt;a.record(&#39;JKT&#39;)

&gt;&gt;a.save(&#39;file.shp&#39;)

Menambahkan data:

- .Poin

&gt;&gt;a.poly([a,b],[c,d])

- .Polygon

&gt;&gt;a.field(&#39;kota&#39;,&#39;C&#39;,4&#39;)

 &gt;&gt;a.field(&#39;Kota&#39;,&#39;C&#39;,&#39;4&#39;)

 &gt;&gt;a.record(&#39;Jakarta&#39;)

 &gt;&gt;a.save(&#39;namefile&#39;)

1. Penutup

1. a)Kesimpulan

Jadi Shapefile adalah bagian dari vektor dalam Sistem Informasi Geografis. Vektor dibagi menjadi empat yaitu, .shp, .dbf, .shx, dan .prj.

1. b)Saran

Untuk memahami lebih jelasnya alangkah lebih baiknya jika kita mencarinya di buku-buku dengan sumber yang terpercaya atau melakukan praktikum mandiri.

