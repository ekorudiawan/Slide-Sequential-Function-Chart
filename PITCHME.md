## Sequential Function Chart
##### Eko Rudiawan @ 2018
---

### Pendahuluan
* SFC merupakan bahasa pemrograman yang didefinisikan pada standar IEC 61131-3.
* SFC merupakan bahasa pemrograman berbasis graphic yang digunakan untuk merepresentasikan sequence/urutan proses dalam sebuah program.
* SFC disebut juga dengan Grafcet yang mengacu pada standar French National Standar.
* SFC didesain untuk membuat program terstruktur terutama untuk sistem yang beroperasi secara sequential dan paralel.
---

### Structure Utama SFC
1. **Steps** merupakan urutan dari sebuah proses yang akan dijalankan.
2. **Transitions** berisi sebuah kondisi/syarat yang harus terpenuhi agar sebuah step dapat diproses. 
3. **Actions** merupakan sebuah step yang berisi aksi yang akan dilakukan pada sebuah proses.
---

### Simbol Pada SFC

1. **Steps** 
    * Initial Step
    * Ordinary Step
2. **Transitions** 
3. **Alternative Sequences**
    * Alternative Convergence
    * Alternative Divergence
4. **Paralel Sequences**
    * Parallel Divergence
    * Parallel Convergence
5. **Jump**
---

#### Steps
1. Initial Step : Proses yang akan dieksekusi pertama kali ketika program dijalankan.

![Initial Step](assets/image/initial_step.png)

2. Ordinary Step : Proses lain yang akan dijalankan ketika sebuah kondisi transition telah terpenuhi.

![Ordinary Step](assets/image/ordinary_step.png)
---

#### Transitions
Transition merupakan sebuah syarat yang harus terpenuhi jika step ingin dieksekusi

![Transition](assets/image/transition.png)
---

#### Alternative Sequence
1. Alternative Divergence : Kondisi masuk ke dalam sebuah percabangan yang digunakan untuk memilih dua atau lebih step yang akan dieksekusi

![Alternative Divergence](assets/image/alternative_divergence.png)

2. Alternative Convergence : : Kondisi keluar dari sebuah percabangan yang telah dieksekusi

![Alternative Convergence](assets/image/alternative_convergence.png)
---

#### Parallel Sequence
1. Parallel Divergence : Kondisi masuk ke dalam sebuah percabangan untuk mengeksekusi dua atau lebih step secara bersamaan/parallel

![Parallel Divergence](assets/image/parallel_divergence.png)

2. Parallel Convergence : Kondisi keluar dari sebuah percabangan yang dieksekusi secara bersamaan/parallel

![Parallel Convergence](assets/image/parallel_convergence.png)
---

### Steps 
* Step Addresses
    * Step_Name.X
    * Step_name.T
---

### Transitions
* Covergence, keluar dari perbacangan
* Divergence, masuk dalam percabangan
---

### Actions
* Action Types
* Action Control
* Indicator Variable
---

#### SFC action types
|Qualifier|Type|
|---------|----|
|N|Non-stored|
|S|Set (Stored)|
|R|Reset|
|P|Pulse|
|L|Time Limited|
|D|Time Delayed|
|SD|Stored and time Delayed|
|DS|Time Delayed and Stored|
|SL|Stored and time Limited|
|P1|Pulse—rising edge|
|P0|Pulse—falling edge|
---