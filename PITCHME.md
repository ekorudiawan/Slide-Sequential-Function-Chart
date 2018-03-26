## Sequential Function Chart
##### Eko Rudiawan @ 2018
---

### Sequential Function Chart
* <span style="font-size:0.8em; ">SFC merupakan bahasa pemrograman yang didefinisikan pada standar IEC 61131-3.</span>
* <span style="font-size:0.8em; ">SFC merupakan bahasa pemrograman berbasis graphic yang digunakan untuk merepresentasikan sequence/urutan proses dalam sebuah program. </span>
* <span style="font-size:0.8em; ">SFC disebut juga dengan Grafcet yang mengacu pada standar French National Standar. </span>
* <span style="font-size:0.8em; ">SFC didesain untuk membuat program terstruktur </span>
* <span style="font-size:0.8em; ">SFC didesain untuk membuat program terstruktur terutama untuk sistem yang beroperasi secara sequential dan paralel. </span>
---

### Struktur Utama SFC
* <span style="font-size:0.8em; ">**Steps** merupakan urutan dari sebuah proses yang akan dijalankan. </span>
* <span style="font-size:0.8em; ">**Transitions** berisi sebuah kondisi/syarat yang harus terpenuhi agar sebuah step dapat diproses. </span>
* <span style="font-size:0.8em; ">**Actions** merupakan sebuah step yang berisi aksi yang akan dilakukan pada sebuah proses. </span>
---

### Contoh Program SFC
![Program SFC](assets/image/program_sfc.png)
---

### Simbol Pada SFC

* <span style="font-size:0.8em; ">**Steps** </span>
    * <span style="font-size:0.5em; ">Initial Step </span>
    * <span style="font-size:0.5em; ">Ordinary Step </span>
* <span style="font-size:0.8em; ">**Transitions** </span>
* <span style="font-size:0.8em; ">**Alternative Sequences** </span>
    * <span style="font-size:0.5em; ">Alternative Convergence </span>
    * <span style="font-size:0.5em; ">Alternative Divergence </span>
* <span style="font-size:0.8em; ">**Paralel Sequences** </span>
    * <span style="font-size:0.5em; ">Parallel Divergence </span>
    * <span style="font-size:0.5em; ">Parallel Convergence </span>
* <span style="font-size:0.8em; ">**Jump** </span>

---

### Steps
* <span style="font-size:0.8em; ">**Initial Step** : Proses yang akan dieksekusi pertama kali ketika program dijalankan. </span>

![Initial Step](assets/image/initial_step.png)

* <span style="font-size:0.8em; ">**Ordinary Step** : Proses lain yang akan dijalankan ketika sebuah kondisi transition telah terpenuhi. </span>

![Ordinary Step](assets/image/ordinary_step.png)
---

### Transitions
<span style="font-size:0.8em; ">**Transition** merupakan sebuah syarat yang harus terpenuhi jika step ingin dieksekusi </span>

![Transition](assets/image/transition.png)
---

### Alternative Branch
* <span style="font-size:0.8em; ">**Alternative Divergence** : Kondisi masuk ke percabangan. </span>

![Alternative Divergence](assets/image/alternative_divergence.png)

* <span style="font-size:0.8em; ">**Alternative Convergence** : Kondisi keluar dari percabangan. </span>

![Alternative Convergence](assets/image/alternative_convergence.png)
---

### Alternative Branch
![Program Alternative Brach](assets/image/program_alternative_branch.png)
---

### Parallel Branch
* <span style="font-size:0.8em; ">**Parallel Divergence** : Masuk ke percabangan secara parallel. </span>

![Parallel Divergence](assets/image/parallel_divergence.png)

* <span style="font-size:0.8em; ">**Parallel Convergence** : Keluar dari percabangan parallel. </span>

![Parallel Convergence](assets/image/parallel_convergence.png)
---

### Parallel Branch
![Program Parallel Brach](assets/image/program_parallel_branch.png)
---

### Steps 

<span style="font-size:0.8em; ">Setiap step secara otomatis akan meng-*generate* sebuah variabel yang disebut dengan **Step Address** </span>

* <span style="font-size:0.7em; ">**Step Addresses**</span>
    * <span style="font-size:0.5em; ">**Step_Name.X** : Kondisi aktif atau tidaknya sebuah Step.</span>
    * <span style="font-size:0.5em; ">**Step_Name.T** : Bernilai waktu berapa lama Step telah aktif</span>
---

### Transitions
<span style="font-size:0.8em; ">**Transition** selalu bernilai akhir **TRUE/FALSE**</span>
* <span style="font-size:0.5em; ">**Divergence** : masuk ke dalam sebuah percabangan</span>
* <span style="font-size:0.5em; ">**Covergence** : keluar dari sebuah percabangan</span>
---

### Actions
![Action](assets/image/program_action.png)
* <span style="font-size:0.5em; ">**Action Types** : Bagaimana dan kapan aksi tersebut dieksekusi. </span>
* <span style="font-size:0.5em; ">**Action Control** : Berisi variabel yang akan dikontrol</span>
* <span style="font-size:0.5em; ">**Indicator Variable** : Variabel sebagai indikator bahwa action step telah dieksekusi</span>
---

#### SFC action types
![Table Action Types](assets/image/table_action_types.png)
---