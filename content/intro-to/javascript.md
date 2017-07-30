+++

title = "JavaScript"
weight = 2
date = "2017-04-24T18:36:24+02:00"
type="slide"

theme = "league"
[revealOptions]
transition= 'convex'
controls= true
progress= true
history= true
center= true
+++

## Introduction and The Goal of This Section

---

### Pengenalan & Tujuan

- Mengenal JavaScript
- Memahami karakteristik dan konsep
- Memahami sintaks

---

## Setup

- Text Editor menggunakan Atom
- Browser menggunakan Chrome
- Developer tools Chrome

---

#  Apa itu JavaScript

___

## JavaScript

JavaScript is a cross-platform, object-oriented scripting language. It is a small and lightweight language. Inside a host environment (for example, a web browser), JavaScript can be connected to the objects of its environment to provide programmatic control over them. (MDN-Mozilla)

___

## Penjelasan

JavaScript adalah cross-platform, bahasa scripting berorientasi objek. Ini adalah bahasa yang kecil dan ringan. Di dalam environment host (misalnya, browser web), JavaScript dapat dihubungkan ke objek dari environment tersebut untuk memberikan kontrol program terhadapnya.

---

# JavaScript Dan Java

___

JavaScript Bukan Java. namun sintaks javascipt mirip java dalam beberapa case tertentu.

---

## First Conceptual Aside

<ul>
  <li class="fragment fade-up">Syntax Parsers</li>
  <li class="fragment fade-up">Execution Contexts</li>
  <li class="fragment fade-up">Lexical Environments</li>
</ul>

---

## Syntax Parsers:

### A PROGRAM THAT READS YOUR CODE AND DETERMINES WHAT IT DOES AND IF ITS GRAMMAR IS VALID

<p class="fragment fade-up">Your code isn't magic. Someone else wrote a program to translate it for the computer.</p>


___

### SEBUAH PROGRAM YANG MEMBACA KODE KALIAN DAN TAHU BAHWA KODE KALIAN BENAR ATAU SALAH

<p class="fragment fade-up">Kode kalian bukanlah sihir/sulap. Orang lain yang membuat program tersebut diterjemahkan untuk berkomunikasi ke komputer.</p>

---

![Syntax Parser](/intro-to/syntaxparser.jpeg)

---

## Lexical Environment:

### WHERE SOMETHING SITS PHYSICALLY IN THE CODE YOU WRITE

<p class="fragment fade-up">'Lexical' means 'having to do with words or grammar'. A lexical environment exists in programming languages in which where you write something is important.</p>

---

## Execution Contexts:

### A WRAPPER TO HELP MANAGE THE CODE THAT IS RUNNING

<p class="fragment fade-up">There are a lots of lexical environments. Which one is currently running is managed via execution contexts. it can contain things beyond what you've written in your code.</p>

---

# It's Important!

---

## Second Conceptual Aside:

### Name / Value Pairs And Objects

___

## Name / Value Pair:

### A NAME WHICH MAPS TO A UNIQUE VALUE

<p class="fragment fade-up">The name may be defined more than once, but only can have one value in any given context.<br />
That value may be more name/value pairs.</p>

___

## For Example

`Alamat = 'Jl. Margonda no. 7'`

---

## Object:

### A COLLECTION OF NAME VALUE PAIRS

<p class="fragment fade-up">The simplest definition when talking about JavaScript.</p>

___

## Ilustration

![Syntax Parser](/intro-to/name-value-pairs.jpeg)

___

## Example Object

```javascript
{
  Alamat:
    {
      Jalan: 'Margonda',
      Nomor: 7,
      Apartemen:
      {
        Lantai: 3,
        Nomor: 007
      }
    }
}

```

---

## The Global Environment And The Global Object

___

### Execution Context (Global)

#### Provide us

* Global Object
* `this`

---

# Let's start code!
