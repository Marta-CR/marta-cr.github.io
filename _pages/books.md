---
layout: page
title: Books & reading
description: My personal bookshelf — finished books, current reads, and stories to return to.
permalink: /books/
nav: false

# To add a book, copy an entry into the appropriate list below.
# Keep a series as one entry unless you want to list individual volumes.
currently_reading:
  - title: Harry Potter
    author: J. K. Rowling
    language: en
  - title: Verity
    author: Colleen Hoover
    language: en

books_read:
  - title: Los hornos de Hitler
    author: Olga Lengyel
    language: es
  - title: Três irmãs
    language: pt
    note: Read in Portuguese.
  - title: As filhas do capitão
    author: María Dueñas
    language: pt
  - title: Non penses nun elefante rosa
    author: Antía Yáñez
    language: gl
  - title: Valeria
    author: Elísabet Benavent
    language: es
    note: Book series.
  - title: Por siempre tú
    author: Moruena Estríngana
    language: es
  - title: Happy as a Dane
    author: Malene Rydahl
    language: en
  - title: Mujeres que compran flores
    author: Vanessa Montfort
    language: es
  - title: Lean In
    author: Sheryl Sandberg
    language: en
  - title: El mentalista
    author: Camilla Läckberg & Henrik Fexeus
    language: es
  - title: La princesa de hielo
    author: Camilla Läckberg
    language: es
  - title: El espejismo
    author: Camilla Läckberg & Henrik Fexeus
    language: es
  - title: La secta
    author: Camilla Läckberg & Henrik Fexeus
    language: es
  - title: El jurado
    author: John Grisham
    language: es
  - title: La verdad sobre el caso Savolta
    author: Eduardo Mendoza
    language: es
  - title: La fundación
    author: Antonio Buero Vallejo
    language: es
  - title: The Black Art of Killing
    author: Matthew Hall
    language: en
  - title: "1984"
    author: George Orwell
    language: es
  - title: Un mundo feliz
    author: Aldous Huxley
    language: es
  - title: Rebelión en la granja
    author: George Orwell
    language: es

to_finish:
  - title: Anna Karénina
    author: Lev Tolstói
    language: es
  - title: Guerra y paz
    author: Lev Tolstói
    language: es

_styles: |
  .reading-section {
    margin: 2rem 0 2.5rem;
  }
  .reading-list {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    list-style: none;
    padding: 0;
    margin: 1.25rem 0;
  }
  .reading-list > li {
    min-width: 0;
    padding: 1rem 1.15rem;
    border: 1px solid var(--section-border, #d3cadc);
    border-radius: 5px;
    color: var(--global-text-color);
    overflow-wrap: anywhere;
  }
  .reading-list .book-title {
    display: block;
    margin-bottom: 0.3rem;
    font-size: 1.08rem;
    font-weight: 600;
    line-height: 1.4;
  }
  .reading-list .book-author,
  .reading-list .book-note {
    display: block;
    font-size: 0.95rem;
    line-height: 1.5;
  }
  .reading-list .book-note {
    margin-top: 0.35rem;
    font-style: italic;
  }
  @media (max-width: 575px) {
    .reading-list {
      grid-template-columns: 1fr;
    }
  }
---

A little space for reading beyond research: the books I have finished, the ones keeping me company now, and a couple of classics I still want to finish.

<section class="reading-section" aria-labelledby="currently-reading">
  <h2 id="currently-reading">Currently reading</h2>
  <ul class="reading-list">
    {% for book in page.currently_reading %}
    <li>
      <span class="book-title" lang="{{ book.language | escape }}">{{ book.title | escape }}</span>
      {% if book.author %}<span class="book-author">{{ book.author | escape }}</span>{% endif %}
      {% if book.note %}<span class="book-note">{{ book.note | escape }}</span>{% endif %}
    </li>
    {% endfor %}
  </ul>
</section>

<section class="reading-section" aria-labelledby="books-read">
  <h2 id="books-read">Books I have read</h2>
  <ul class="reading-list">
    {% for book in page.books_read %}
    <li>
      <span class="book-title" lang="{{ book.language | escape }}">{{ book.title | escape }}</span>
      {% if book.author %}<span class="book-author">{{ book.author | escape }}</span>{% endif %}
      {% if book.note %}<span class="book-note">{{ book.note | escape }}</span>{% endif %}
    </li>
    {% endfor %}
  </ul>
</section>

<section class="reading-section" aria-labelledby="to-finish">
  <h2 id="to-finish">To pick up again</h2>
  <p>Two classics I want to finish — they are making me work for it!</p>
  <ul class="reading-list">
    {% for book in page.to_finish %}
    <li>
      <span class="book-title" lang="{{ book.language | escape }}">{{ book.title | escape }}</span>
      {% if book.author %}<span class="book-author">{{ book.author | escape }}</span>{% endif %}
      {% if book.note %}<span class="book-note">{{ book.note | escape }}</span>{% endif %}
    </li>
    {% endfor %}
  </ul>
</section>
