# Nama : Muhammad Rafai (tim : FE-8)

# Penjelasan

# Berdasarkan Artikel, Buatlah code yang mencakup :

## Jawaban Nomor 1
###  :
1. Section 2-4 : Masing masing minimal 3 contoh dengan 1 usecase

### Jawaban :
jawaban tertera pada file [Section2-4.html](https://github.com/rafai123/Tugas-DOM-kak-Tata/blob/main/section2-4.html "Github Rafai")

**Penjelasan ada pada comment pada kode berikut : **

```html
<body>
    <ul id="unorder-list">
      <li>Rafai</li>
      <li>Home</li>
      <li>About</li>
      <li>Contact</li>
      <ol class="order-list">
        <li>Whangsaf</li>
        <li>LinkedIn</li>
        <li>Github</li>
      </ol>
      <li>Logout</li>
    </ul>
    <p class="text-paragraf"></p>
    <br />
    <br />

    <script>
      // section 2 (selecting Element)
      // minimal 3 contoh
      // getElementById()
      let ul = document.getElementById("unorder-list");
      // getElementByClassName()
      let ol = document.getElementsByClassName("order-list")[0];
      // querySelector()
      let paragraph = document.querySelector(".text-paragraf");

      // Section 3 (Traversing Elements)
      // Minimal 3 contoh
      // Get the parent element
      let parentElementOl = ol.parentNode;
      // Get Child Elements
      let childElement = ol.firstChild;
      // Get Next Siblings
      let nextSibling = childElement.nextSibling;

      // Section 4 (Manipulating Element)
      // Minimal 3 contoh
      // innerHTML
      nextSibling.innerHTML = "Dibuat Oleh Rafai";
      // textContent
      paragraph.textContent = "Ini paragraf Text Content";
      // after()
      paragraph.after("ini memasukkan paragraf dengan after()");
    </script>
  </body>
```

## Jawaban Nomor 2
### Soal :
2. Section 4-6 : Masing masing minimal 2 contoh dengan 1 usecase


### Jawaban :
jawaban tertera pada file [Section4-6.html](https://github.com/rafai123/Tugas-DOM-kak-Tata/blob/main/section4-6.html "Github Rafai")

**Penjelasan ada pada comment pada kode berikut : **

``` html
 <body>
    <div id="container"></div>
    <script>
      // Menangkap div#container
      let container = document.getElementById("container");

      // Section 4 (Manipulating Elements)
      // Minimal 3 contoh

      // createElement()
      let paragraph = document.createElement("p");
      let input = document.createElement("input");

      // InnerHTML
      paragraph.innerHTML = "Ini inner HTML di dalam element yang dibuat dengan createElement";

      // appentChild()
      container.appendChild(paragraph);
      container.appendChild(input);

      // Section 5 (Working with Attributes)
      // setAttribute
      input.setAttribute("name", "test");
      input.setAttribute("value", "Ini adalah value yang dibuat degan setAtribute()");

      // getAttribute
      let atributGet = input.getAttribute("value");
      // Menampilkan isi value dari getAttribute()
      console.log(atributGet);
      // hasAttribute
      // Melakukan pengecekan apabila memiliki atribut "value", maka true. jika tidak maka false
      input.hasAttribute("value") ? console.log(true) : console.log(false);

      
      // Section 6 (Manipulating Element's Style)
      // style property
      paragraph.style.color = "tomato"; //Mengubah warna huruf jadi warna Tomato

      //   getComputedStyle()
      let computedStyle = getComputedStyle(paragraph);
      console.log(computedStyle.color); //Menampilkan computed style warna huruf dari paragraph ke console

      // Classlist Property
      console.log(input.classList); //menampilkan classlist input ke console.log
    </script>
  </body>
```


## Jawaban Nomor 3
### Soal :
3.  Section 7-8 : Masing masing minimal 2 contoh dengan 2 usecase

### Jawaban :
jawaban tertera pada file [Section7-8.html](https://github.com/rafai123/Tugas-DOM-kak-Tata/blob/main/section7-8.html "Github Rafai")

**Penjelasan ada pada comment pada kode berikut : **

#### Usecase 1 :

``` html
 <body>
    <!-- Section 7 (Working with Events) -->
    <!-- HTML Event Handles attributes -->
    <!-- Usecase Menampilkan allert ketika tombol di klik -->
    <button onclick="alert('Tombol ini Telah di klik')">Alert</button> <!--Menampilkan alert() melalui html hamdles secara langsung -->
    <button onclick="tombolAlert()">Alert dengan Function</button> <!-- Ketika tombol di klik, memunculkan function tombolAlert()-->


    <script>
        // Section 7, Ini adalah function alert yang di panggil melalui atribut onclick
        const tombolAlert = () => {
            alert("Tombol dengan function tombolAlert() ini telah di klik")
        }
    </script>
```


