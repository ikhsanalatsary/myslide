+++

title = "JQUERY"
weight = 3
type="slide"

theme = "league"
[revealOptions]
transition= 'convex'
controls= true
progress= true
history= true
center= true
+++


## Apa itu JQuery?

<p class="fragment fade-up">
  Kumpulan `functions` JavaScript (Library), yang memudahkan dan dapat digunakan berulang-ulang.
</p>

---

## Apa yang bisa dilakukan JQuery?

<ul>
  <li class="fragment fade-up"> Akses element pada dokumen HTML
  <li class="fragment fade-up"> Mengubah Document HTML pada Halaman web
  <li class="fragment fade-up"> Menanggapi Tindakan Yang dilakukan oleh pengguna
  <li class="fragment fade-up"> Animasi
  <li class="fragment fade-up"> Bisa berkomunikasi dengan server
</ul>

---

## Kenapa Harus JQUERY?

<h3 class="fragment fade-up">
  "Write Less, Do More"
</h3>

---

## Browser Compatibility
- Chrome
- Safari
- Firefox Mozila
- IE

---

## More...

- Dari pemula menjadi pro
  * Mudah digunakan dan dipahami
  * walaupun pemula, bisa membuat website dinamis level profesional
- Serba cepat
  * 5 baris kode `jQuery` vs 30 baris kode vanilla `JavaScript`
  * Tidak ada masalah dengan kompatibel browser yang berbeda
  * Banyak Plugin bertebaran (Open Source)

---

## Using JQUERY

- Akses element (di jquery disebut Selectors)
  * dengan cara akses elemen html
  * dengan cara akses elemen dengan ID(Unique)
  * dengan cara akses elemen dengan nama kelas

___

### CSS

```css
  /* paragraph element*/
  p { ... }

  /* ID */
  #container { ... }

  /* class name */
  .nama-kelas { ... }

```

### jQuery

```javascript
/* paragraph element*/
$('p');

/* ID */
$('#container');

/* class name */
$('.nama-kelas');
```

---

## Conceptual Aside

- The DOM
- traversing the DOM
- Working with the DOM
- Listening to DOM events
- Styling
- Introduction to Ajax Basic
- Ajax with form
- Utility methods
- JQuery plugin
- Working with promises

---

## Apa itu DOM

---

## Document Object Model:
### The DOM model represents a document with a logical tree.

<p class="fragment fade-up">
  is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.
</p>

---

___

## HTML Document

```html

<html>
<head>
  <title>the title</title>
</head>
<body>
  <div>
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>
    <p>This is yet another paragraph.</p>
  </div>
</body>
</html>

```
___

## DOM tree

![Dom tree](/myslide/intro-to/dom-tree.jpg)

___

### modelling HTML, SVG, or XML documents as objects is not part of the JavaScript language

---

## Traversing The DOM

---

## Searching The DOM

- Descendant:
  * mengakses turunan selektor(parent selektor)
  * mengakses turunan langsung dari selektor (hirarki)
  * mengakses lebih dari satu selector
  * Pseudo classes CSS (filter)

___

### Descendant

#### HTLML

```html
  <article>
    <h1>Cara menggunakan Jquery</h1>
    <ul id="parent">
      <li>cari selektor</li>
      <li>tambahkan kecap</li>
      <li class="ketiga">sajikan</li>
    </ul>
  </article>
```

#### Jquery

```javascript
  $('#parent li')
```

___

### Descendant (direct children)

#### HTLML

```html
  <article>
    <h1>Cara menggunakan Jquery</h1>
    <ul id="parent">
      <li>cari selektor</li>
      <li>
        <ul id="other">
          <li>tambahkan kecap</li>
        </ul>
      </li>
      <li class="ketiga">sajikan</li>
    </ul>
  </article>
```

#### Jquery

```javascript
  $('#parent > li')
```

___

### Descendant (select multiple selector)

#### HTLML

```html
  <article>
    <h1>Cara menggunakan Jquery</h1>
    <ul id="parent">
      <!-- list ke #0 -->
      <li>cari selektor</li>
      <!-- list ke #1 -->
      <li>tambahkan kecap</li>
      <!-- list ke #2 -->
      <li class="ketiga">sajikan</li>
    </ul>
  </article>
```

#### Jquery

```javascript
  $('.ketiga, #other')
```

___

### Descendant (pseudo classes CSS)

#### HTLML

```html
  <article>
    <h1>Cara menggunakan Jquery</h1>
    <ul id="parent">
      <li>cari selektor</li>
      <li>
        <ul id="other">
          <li>tambahkan kecap</li>
        </ul>
      </li>
      <li class="ketiga">sajikan</li>
    </ul>
  </article>
```

#### Jquery

```javascript
  $('#parent li:first') // list pertama
  $('#parent li:last') // list terakhir
  $('#parent li:odd') // list ganjil
  $('#parent li:even') // list genap
```

---

## Traversing It

---

#### HTLML

```html
  <article>
    <h1>Cara menggunakan Jquery</h1>
    <ul id="parent">
      <li>cari selektor</li>
      <li>tambahkan kecap</li>
      <li class="ketiga">sajikan</li>
    </ul>
  </article>
```

#### Jquery

```javascript
  $('#parent').find('li') // ini disebut traversal
```

---

#### pertama

```javascript
  $('li:first')
```

#### kedua

```javascript
  $('li').first();
```

Hasil tetap sama

---

## lebih cepat dibanding cara pertama!!

---

## Walking the DOM

Bagaimana jika kita mencoba mendapatkan list yang ditengah (antara list pertama dan terakhir)?

### Traversing

```javascript
  $('li').first().next();
```

ini di sebut **method chaining**

```javascript
  $('li').first().next().prev(); // contoh more chaining
```

hasilnya kembali lagi ke sebelumnya

---

## Walking up the DOM

Bagaimana jika kita mencoba mendapatkan parent selectornya?

```javascript
  $('li').first().parent();
```

```javascript
  $('li').first().parent();
```

---

## Walking down the DOM

### Traversing down

```javascript
  $('#parent').children('li');
```

same as

```javascript
  $('#parent > li');
```

---

## Jquery Cheat Sheet

[Jquery Cheat Sheet](https://oscarotero.com/jquery/)
