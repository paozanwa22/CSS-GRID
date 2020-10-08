

CSS GRID - #1 Apa itu CSS GRID
CSS GRID - #2 Terminologi pada CSS GRID
CSS GRID - #3 Columns & Rows
CSS GRID - #4 Special Keywords & Functions
	ul.gallery>li*10>img[src="img/$.jpg"]	//ini adalah emmet
CSS GRID - #5 Grid Area & Grid Gap
CSS GRID - #6 Grid Alignment
CSS GRID - #7 Grid Item Properties
NGOBAR #24 - Membuat WEBSITE RESPONSIVE menggunakan CSS GRID


CSS Grid Terminology
• Grid container //elemen pembungkus grid
• Grid item	//Element-element yang berada (1level) di dalam grid container
• Grid line	//Garis horizontal (kolom) atau vertikal (baris) yang memisahkan grid menjadi beberapa bagian dan ditandai dengan angka.
• Grid cell	//Perpotongan / pertemuan antara baris dan kolom di dalam grid.
• Grid area	//Kumpulan lebih dari satu grid cell yang membentuk kotak
• Grid track	//(seperti cellpadding pada HTML)Ukuran / jarak antara 2 grid line, bisa horizontal (kolom) atau vertikal (baris).
• Grid gap	//(seperti cellspacing pada HTML)Jarak antar grid track / cell.


//CSS Grid Properties CONTAINER		clolumn (ke samping)
• grid-template-rows
• grid-template-columns
	//untuk apa explicit dan implicit? karna data itu dinames (tidak diketahui pasti)
	explicit grid	//ketika kita menentukan secara jelas memberi nilai pada grid	//garis lurus
	implicit grid	//ketika grid menentukan secara otomatis sisanya	//garis putus-putus
• grid-auto-rows	//digunakan saat data implicit ke bawah(mengatur yang row yang implicit)
• grid-auto-columns	//digunakan saat data implicit ke kanan(mengatur yang column yang explicit)
• grid-auto-flow	//Mengatur penempatan item/cell pada grid track(kebawah, kesamping dll..), termasuk yang ditulis secara implicit

		Special Function & Keywords
		• repeat()			//Menentukan ukuran grid track secara berulang
		• min-content & max-content	//Menentukan seberapa besar ukuran grid track berdasarkan content pada sebuah item
		• minmax()			//Menentukan ukuran minimal dan maksimal dari grid track
		• auto-fill & auto-fit		//Menentukan jumlah item untuk berada pada grid track

• grid-template-areas	//Mendefinisikan grid template menggunakan nama dari area yang ditulis pada property grid-area pada item
• grid-template		//Shorthand untuk mendefinisikan grid-template-rows, grid-template-columns, dan grid-template-areas dalam satu deklarasi.






• grid-row-gap		//row-gap	//penulisan baru	//same
• grid-column-gap	//column-gap	//penulisan baru	//Mendefinisikan ukuran grid-line / jarak antara baris atau kolom
• grid-gap		//gap	//penulisan baru	//Shorthand untuk mendefinisikan row-gap, column-gap dalam satu deklarasi.
• grid			//Shorthand untuk mendefinisikan properti-properti berikut dalam satu deklarasi : 
				grid-template-rows, grid-template-columns,
				grid-template-areas, grid-auto-rows, 
				grid-auto-colums dan grid-auto-flow


• align-items		//Mensejajarkan grid-items pada sumbu vertikal
• justify-items		//Mensejajarkan grid-items pada sumbu horizontal
• place-items		//shorthand untuk menulis align-items dan justify-items dalam satu deklarasi.

• justify-content	//Mengatur posisi seluruh grid container pada sumbu horizontal.
				Ini bisa dilakukan ketika ukuran total grid lebih kecil dari
				ukuran containernya, biasanya ketika grid items nya
				menggunakan ukuran yang fixed (px)
• align-content		//sama seperti justify-content, tapi untuk sumbu vertical
• place-content		//shorthand untuk menulis justify-content dan align-content dalam satu deklarasi.


//CSS Grid Properties ITEM
• grid-column-start	//
• grid-column-end	//
• grid-row-start	//
• grid-row-end		//


• grid-column		// Shorthand untuk start dan end pada grid-column & grid-row
• grid-row		// grid-column: 2 / 4;
			   grid-row: 2 / 4;

			grid-column: 1 / span 2;
			grid-row: 1 / span 2;	//span disini artinya menambah dua


• grid-area		//Menentukan nama area pada item sesuai dengan template yang sudah dibuat sebelumnya melalui properti grid-template-areas.
			Bisa digunakan sebagai shorthand untuk grid-row-start, grid-column-start, grid-row-end, grid-columnend-end
			//grid-area: 2 / 1 / 4 / 3

//MENGATUR POSISI PADA SEBUAH ITEM
• align-self		//Mengatur posisi item pada sebuah cell terhadap sumbu vertikal
• justify-self		//Mengatur posisi item pada sebuah cell terhadap sumbu horizontal
• place-self		//Shorthand posisi item pada sebuah cell terhadap sumbu vertikal dan
			sumbu horizontal dalam satu deklarasi