# Panduan Belajar Python Lengkap: Dari Nol hingga Mahir

[![Python Version](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Selamat Datang di Panduan Beljar Python Terlengkap!**

Panduan ini dirancang untuk menjadi sumber belajar Python yang komprehensif, mulai dari konsep paling dasar hingga topik-topik yang lebih lanjut. Ditujukan bagi siapa saja yang ingin mempelajari Python, baik Anda seorang pemula tanpa pengalaman pemrograman sama sekali, maupun programmer dari bahasa lain yang ingin beralih ke Python.

Dokumen ini sengaja dibuat sangat panjang dan detail untuk memberikan pemahaman yang mendalam pada setiap topik. Gunakan Daftar Isi di bawah ini untuk menavigasi bagian-bagian yang Anda minati.

**Mengapa Belajar Python?**

*   **Mudah Dipelajari:** Sintaks Python dirancang agar mudah dibaca dan ditulis, mirip dengan bahasa Inggris. Ini menjadikannya bahasa yang bagus untuk pemula.
*   **Serbaguna (Versatile):** Python digunakan di berbagai bidang, termasuk:
    *   Pengembangan Web (Backend)
    *   Ilmu Data (Data Science), Pembelajaran Mesin (Machine Learning), dan Kecerdasan Buatan (AI)
    *   Otomatisasi Tugas (Scripting)
    *   Pengembangan Game
    *   Komputasi Ilmiah dan Numerik
    *   Pengembangan Aplikasi Desktop (GUI)
    *   Dan masih banyak lagi!
*   **Komunitas Besar dan Aktif:** Ada banyak sekali dokumentasi, tutorial, forum, dan pustaka (library) yang tersedia. Jika Anda mengalami kesulitan, kemungkinan besar orang lain pernah mengalaminya dan solusinya sudah ada.
*   **Banyak Pustaka (Libraries) dan Kerangka Kerja (Frameworks):** Python memiliki ekosistem pustaka pihak ketiga yang kaya (seperti NumPy, Pandas, Django, Flask, TensorFlow, PyTorch) yang mempercepat pengembangan.
*   **Permintaan Tinggi di Industri:** Keahlian Python sangat dicari di pasar kerja saat ini.

---

## Daftar Isi

1.  [Pendahuluan](#1-pendahuluan)
    *   [Apa itu Python?](#apa-itu-python)
    *   [Sejarah Singkat Python](#sejarah-singkat-python)
    *   [Filosofi Python (The Zen of Python)](#filosofi-python-the-zen-of-python)
    *   [Bagaimana Menggunakan Panduan Ini](#bagaimana-menggunakan-panduan-ini)
2.  [Persiapan Lingkungan Pengembangan](#2-persiapan-lingkungan-pengembangan)
    *   [Instalasi Python](#instalasi-python)
        *   [Windows](#windows)
        *   [macOS](#macos)
        *   [Linux](#linux)
    *   [Memverifikasi Instalasi](#memverifikasi-instalasi)
    *   [Editor Teks dan Integrated Development Environment (IDE)](#editor-teks-dan-integrated-development-environment-ide)
        *   [Rekomendasi (VS Code, PyCharm, Sublime Text, dll)](#rekomendasi-vs-code-pycharm-sublime-text-dll)
        *   [Menjalankan Kode Python](#menjalankan-kode-python)
    *   [Lingkungan Virtual (Virtual Environments)](#lingkungan-virtual-virtual-environments)
        *   [Mengapa Menggunakan Lingkungan Virtual?](#mengapa-menggunakan-lingkungan-virtual)
        *   [Membuat dan Mengaktifkan Lingkungan Virtual (`venv`)](#membuat-dan-mengaktifkan-lingkungan-virtual-venv)
    *   [Manajer Paket `pip`](#manajer-paket-pip)
        *   [Instalasi Paket](#instalasi-paket)
        *   [Melihat Paket Terinstal](#melihat-paket-terinstal)
        *   [`requirements.txt`](#requirementstxt)
3.  [Dasar-Dasar Python](#3-dasar-dasar-python)
    *   [Sintaks Dasar dan Komentar](#sintaks-dasar-dan-komentar)
    *   [Variabel dan Tipe Data](#variabel-dan-tipe-data)
        *   [Aturan Penamaan Variabel](#aturan-penamaan-variabel)
        *   [Tipe Data Dasar](#tipe-data-dasar)
            *   [`int` (Integer / Bilangan Bulat)](#int-integer--bilangan-bulat)
            *   [`float` (Floating-Point / Bilangan Desimal)](#float-floating-point--bilangan-desimal)
            *   [`str` (String / Teks)](#str-string--teks)
            *   [`bool` (Boolean / Logika True/False)](#bool-boolean--logika-truefalse)
            *   [`NoneType` (Nilai Kosong `None`)](#nonetype-nilai-kosong-none)
        *   [Pengecekan Tipe (`type()`)](#pengecekan-tipe-type)
        *   [Konversi Tipe Data (Type Casting)](#konversi-tipe-data-type-casting)
    *   [Operator](#operator)
        *   [Operator Aritmatika (`+`, `-`, `*`, `/`, `%`, `**`, `//`)](#operator-aritmatika-------)
        *   [Operator Perbandingan (`==`, `!=`, `>`, `<`, `>=`, `<=`)](#operator-perbandingan----)
        *   [Operator Logika (`and`, `or`, `not`)](#operator-logika-and-or-not)
        *   [Operator Penugasan (`=`, `+=`, `-=`, `*=`, `/=`, dll)](#operator-penugasan----dll)
        *   [Operator Keanggotaan (`in`, `not in`)](#operator-keanggotaan-in-not-in)
        *   [Operator Identitas (`is`, `is not`)](#operator-identitas-is-is-not)
        *   [Operator Bitwise (Opsional Lanjutan)](#operator-bitwise-opsional-lanjutan)
    *   [Input dan Output Dasar](#input-dan-output-dasar)
        *   [Fungsi `print()`](#fungsi-print)
        *   [Fungsi `input()`](#fungsi-input)
    *   [String Lanjutan](#string-lanjutan)
        *   [Indexing dan Slicing](#indexing-dan-slicing)
        *   [Metode String Umum (`upper()`, `lower()`, `strip()`, `split()`, `join()`, `replace()`, `find()`, `startswith()`, `endswith()`, dll)](#metode-string-umum-upper-lower-strip-split-join-replace-find-startswith-endswith-dll)
        *   [F-Strings (Formatted String Literals)](#f-strings-formatted-string-literals)
4.  [Struktur Kontrol Alur (Control Flow)](#4-struktur-kontrol-alur-control-flow)
    *   [Pernyataan Kondisional (`if`, `elif`, `else`)](#pernyataan-kondisional-if-elif-else)
        *   [Logika Bersarang (Nested Conditions)](#logika-bersarang-nested-conditions)
        *   [Ekspresi Kondisional (Operator Ternary)](#ekspresi-kondisional-operator-ternary)
    *   [Perulangan (`for` loop)](#perulangan-for-loop)
        *   [Iterasi Melalui Urutan (List, Tuple, String, dll)](#iterasi-melalui-urutan-list-tuple-string-dll)
        *   [Fungsi `range()`](#fungsi-range)
        *   [Perulangan Bersarang (Nested Loops)](#perulangan-bersarang-nested-loops)
    *   [Perulangan (`while` loop)](#perulangan-while-loop)
        *   [Loop Tak Terbatas (Infinite Loop) dan Cara Menghentikannya](#loop-tak-terbatas-infinite-loop-dan-cara-menghentikannya)
    *   [Kontrol Perulangan (`break`, `continue`, `pass`)](#kontrol-perulangan-break-continue-pass)
        *   [`break`: Menghentikan Loop](#break-menghentikan-loop)
        *   [`continue`: Melanjutkan ke Iterasi Berikutnya](#continue-melanjutkan-ke-iterasi-berikutnya)
        *   [`pass`: Pernyataan Kosong (Placeholder)](#pass-pernyataan-kosong-placeholder)
    *   [Klausa `else` pada Loop](#klausa-else-pada-loop)
5.  [Struktur Data](#5-struktur-data)
    *   [List](#list)
        *   [Membuat List](#membuat-list)
        *   [Mengakses Elemen (Indexing dan Slicing)](#mengakses-elemen-indexing-dan-slicing)
        *   [Memodifikasi List (Mutable)](#memodifikasi-list-mutable)
        *   [Metode List (`append()`, `insert()`, `extend()`, `remove()`, `pop()`, `clear()`, `index()`, `count()`, `sort()`, `reverse()`)](#metode-list-append-insert-extend-remove-pop-clear-index-count-sort-reverse)
        *   [List Comprehensions (Cara Cepat Membuat List)](#list-comprehensions-cara-cepat-membuat-list)
        *   [List Bersarang (Nested Lists)](#list-bersarang-nested-lists)
    *   [Tuple](#tuple)
        *   [Membuat Tuple](#membuat-tuple)
        *   [Mengakses Elemen (Immutable)](#mengakses-elemen-immutable)
        *   [Kapan Menggunakan Tuple?](#kapan-menggunakan-tuple)
        *   [Tuple Unpacking](#tuple-unpacking)
    *   [Set](#set)
        *   [Membuat Set](#membuat-set)
        *   [Karakteristik (Tidak Terurut, Unik)](#karakteristik-tidak-terurut-unik)
        *   [Operasi Set (Union, Intersection, Difference, Symmetric Difference)](#operasi-set-union-intersection-difference-symmetric-difference)
        *   [Metode Set (`add()`, `update()`, `remove()`, `discard()`, `pop()`, `clear()`)](#metode-set-add-update-remove-discard-pop-clear)
        *   [Kapan Menggunakan Set?](#kapan-menggunakan-set)
    *   [Dictionary](#dictionary)
        *   [Membuat Dictionary (Key-Value Pairs)](#membuat-dictionary-key-value-pairs)
        *   [Mengakses Nilai (Menggunakan Key)](#mengakses-nilai-menggunakan-key)
        *   [Memodifikasi Dictionary (Mutable)](#memodifikasi-dictionary-mutable)
        *   [Metode Dictionary (`keys()`, `values()`, `items()`, `get()`, `pop()`, `popitem()`, `update()`, `clear()`)](#metode-dictionary-keys-values-items-get-pop-popitem-update-clear)
        *   [Iterasi Melalui Dictionary](#iterasi-melalui-dictionary)
        *   [Dictionary Comprehensions](#dictionary-comprehensions)
        *   [Dictionary Bersarang (Nested Dictionaries)](#dictionary-bersarang-nested-dictionaries)
6.  [Fungsi](#6-fungsi)
    *   [Mendefinisikan Fungsi (`def`)](#mendefinisikan-fungsi-def)
    *   [Memanggil Fungsi](#memanggil-fungsi)
    *   [Parameter dan Argumen](#parameter-dan-argumen)
        *   [Argumen Positional](#argumen-positional)
        *   [Argumen Keyword](#argumen-keyword)
        *   [Parameter Default](#parameter-default)
        *   [Argumen Arbitrer (`*args`)](#argumen-arbitrer-args)
        *   [Argumen Keyword Arbitrer (`**kwargs`)](#argumen-keyword-arbitrer-kwargs)
    *   [Nilai Kembali (`return`)](#nilai-kembali-return)
        *   [Mengembalikan Beberapa Nilai (sebagai Tuple)](#mengembalikan-beberapa-nilai-sebagai-tuple)
    *   [Scope Variabel (LEGB Rule: Local, Enclosing, Global, Built-in)](#scope-variabel-legb-rule-local-enclosing-global-built-in)
        *   [Keyword `global`](#keyword-global)
        *   [Keyword `nonlocal`](#keyword-nonlocal)
    *   [Docstrings (Dokumentasi Fungsi)](#docstrings-dokumentasi-fungsi)
    *   [Fungsi Lambda (Fungsi Anonim)](#fungsi-lambda-fungsi-anonim)
    *   [Rekursi](#rekursi)
7.  [Modul dan Paket](#7-modul-dan-paket)
    *   [Apa itu Modul?](#apa-itu-modul)
    *   [Mengimpor Modul (`import`, `from ... import ...`, `import ... as ...`)](#mengimpor-modul-import-from--import--import--as-)
    *   [Python Standard Library](#python-standard-library)
    *   [Membuat Modul Sendiri](#membuat-modul-sendiri)
    *   [Blok `if __name__ == "__main__":`](#blok-if-__name__--__main__)
    *   [Paket (Packages)](#paket-packages)
    *   [Mengimpor dari Paket](#mengimpor-dari-paket)
    *   [File `__init__.py`](#file-__init__py)
    *   [Menginstal Paket Eksternal dengan `pip`](#menginstal-paket-eksternal-dengan-pip)
    *   [Lingkungan Virtual (`venv`)](#lingkungan-virtual-venv)
8.  [Input/Output File (File I/O)](#8-inputoutput-file-file-io)
    *   [Membuka dan Menutup File (`open()`, `close()`)](#membuka-dan-menutup-file-open-close)
    *   [Mode Akses File](#mode-akses-file)
    *   [Menggunakan `with` untuk File Handling](#menggunakan-with-untuk-file-handling)
    *   [Membaca File](#membaca-file)
        *   [`read(size=-1)`](#readsize-1)
        *   [`readline(size=-1)`](#readlinetsize-1)
        *   [`readlines()`](#readlines)
        *   [Iterasi Langsung atas Objek File](#iterasi-langsung-atas-objek-file)
    *   [Menulis ke File](#menulis-ke-file)
        *   [`write(string)`](#writestring)
        *   [`writelines(list_of_strings)`](#writelineslist_of_strings)
    *   [Bekerja dengan Path File (`os.path`, `pathlib`)](#bekerja-dengan-path-file-ospath-pathlib)
    *   [Bekerja dengan Format File Umum](#bekerja-dengan-format-file-umum)
        *   [CSV (`csv` module)](#csv-csv-module)
        *   [JSON (`json` module)](#json-json-module)
    *   [Penanganan Error pada Operasi File](#penanganan-error-pada-operasi-file)
9.  [Penanganan Error dan Exceptions](#9-penanganan-error-dan-exceptions)
    *   [Syntax Errors vs Exceptions](#syntax-errors-vs-exceptions)
    *   [Exceptions Umum](#exceptions-umum)
    *   [Blok `try...except`](#blok-tryexcept)
    *   [Menangkap Exceptions Spesifik](#menangkap-exceptions-spesifik)
    *   [Menangkap Multiple Exceptions](#menangkap-multiple-exceptions)
    *   [Klausa `else`](#klausa-else-1)
    *   [Klausa `finally`](#klausa-finally)
    *   [Membangkitkan Exceptions (`raise`)](#membangkitkan-exceptions-raise)
    *   [Membuat Custom Exceptions](#membuat-custom-exceptions)
    *   [Assertion (`assert`)](#assertion-assert)
10. [Pemrograman Berorientasi Objek (Object-Oriented Programming - OOP)](#10-pemrograman-berorientasi-objek-object-oriented-programming---oop)
    *   [Pendahuluan OOP](#pendahuluan-oop)
    *   [Kelas dan Objek](#kelas-dan-objek)
        *   [Mendefinisikan Kelas di Python](#mendefinisikan-kelas-di-python)
    *   [Atribut (Instance vs Class Attributes)](#atribut-instance-vs-class-attributes)
    *   [Metode](#metode)
        *   [Metode `__init__` (Konstruktor)](#metode-__init__-konstruktor)
        *   [Parameter `self`](#parameter-self)
        *   [Metode Instance](#metode-instance)
        *   [Metode Kelas (`@classmethod`)](#metode-kelas-classmethod)
        *   [Metode Statis (`@staticmethod`)](#metode-statis-staticmethod)
    *   [Prinsip Utama OOP](#prinsip-utama-oop)
        *   [Enkapsulasi (Encapsulation)](#enkapsulasi-encapsulation)
            *   [Kontrol Akses (Public, Protected, Private)](#kontrol-akses-public-protected-private)
            *   [Properti (`@property`)](#properti-property)
        *   [Pewarisan (Inheritance)](#pewarisan-inheritance)
            *   [Membuat Subclass](#membuat-subclass)
            *   [Meng-override Metode](#meng-override-metode)
            *   [Fungsi `super()`](#fungsi-super)
            *   [Pewarisan Ganda (Multiple Inheritance)](#pewarisan-ganda-multiple-inheritance)
        *   [Polimorfisme (Polymorphism)](#polimorfisme-polymorphism)
            *   [Duck Typing](#duck-typing)
            *   [Polimorfisme dengan Inheritance (Method Overriding)](#polimorfisme-dengan-inheritance-method-overriding)
        *   [Abstraksi (Abstraction)](#abstraksi-abstraction)
            *   [Kelas Abstrak (Abstract Base Classes - ABCs)](#kelas-abstrak-abstract-base-classes---abcs)
    *   [Metode Khusus (Dunder/Magic Methods)](#metode-khusus-dundermagic-methods)
        *   [`__str__` dan `__repr__`](#__str__-dan-__repr__)
        *   [`__len__`](#__len__)
        *   [`__eq__`](#__eq__)
        *   [Metode Operator (`__add__`, `__lt__`, dll)](#metode-operator-__add__-__lt__-dll)
    *   [Data Classes (`@dataclass`) - Python 3.7+](#data-classes-dataclass---python-37)
11. [Topik Menengah](#11-topik-menengah)
    *   [List/Set/Dictionary Comprehensions (Lebih Dalam)](#listsetdictionary-comprehensions-lebih-dalam)
    *   [Generator Expressions](#generator-expressions)
    *   [Fungsi Generator (`yield`)](#fungsi-generator-yield)
        *   [Keuntungan Menggunakan Generator](#keuntungan-menggunakan-generator)
    *   [Decorators (`@`)](#decorators-)
        *   [Memahami Decorator](#memahami-decorator)
        *   [Membuat Decorator Sederhana](#membuat-decorator-sederhana)
        *   [Decorator dengan Argumen](#decorator-dengan-argumen)
        *   [`functools.wraps`](#functoolswraps)
    *   [Context Managers (`with` statement dan `contextlib`)](#context-managers-with-statement-dan-contextlib)
        *   [Membuat Context Manager Sendiri (dengan kelas atau `contextlib.contextmanager`)](#membuat-context-manager-sendiri-dengan-kelas-atau-contextlibcontextmanager)
    *   [Regular Expressions (`re` modul)](#regular-expressions-re-modul)
        *   [Pola Dasar](#pola-dasar)
        *   [Fungsi Utama (`match()`, `search()`, `findall()`, `sub()`)](#fungsi-utama-match-search-findall-sub)
        *   [Grup dan Penangkapan](#grup-dan-penangkapan)
    *   [Type Hinting (PEP 484)](#type-hinting-pep-484)
        *   [Mengapa Menggunakan Type Hinting?](#mengapa-menggunakan-type-hinting)
        *   [Sintaks Dasar](#sintaks-dasar-1)
        *   [Modul `typing`](#modul-typing)
    *   [Partial Functions (`functools.partial`)](#partial-functions-functoolspartial)
    *   [Enumerations (`enum` modul)](#enumerations-enum-modul)
12. [Pengenalan Pustaka Populer](#12-pengenalan-pustaka-populer)
    *   [Ilmu Data dan Analisis:](#ilmu-data-dan-analisis)
        *   [NumPy: Komputasi Numerik](#numpy-komputasi-numerik)
        *   [Pandas: Manipulasi dan Analisis Data](#pandas-manipulasi-dan-analisis-data)
        *   [Matplotlib: Visualisasi Data Dasar](#matplotlib-visualisasi-data-dasar)
        *   [Seaborn: Visualisasi Data Statistik](#seaborn-visualisasi-data-statistik)
    *   [Pengembangan Web (Backend):](#pengembangan-web-backend)
        *   [Flask: Kerangka Kerja Mikro](#flask-kerangka-kerja-mikro)
        *   [Django: Kerangka Kerja Tingkat Tinggi](#django-kerangka-kerja-tingkat-tinggi)
    *   [Permintaan HTTP:](#permintaan-http)
        *   [Requests: HTTP untuk Manusia](#requests-http-untuk-manusia)
    *   [Web Scraping:](#web-scraping)
        *   [Beautiful Soup 4: Parsing HTML/XML](#beautiful-soup-4-parsing-htmlxml)
        *   [Scrapy: Kerangka Kerja Scraping](#scrapy-kerangka-kerja-scraping)
    *   [Pengujian (Testing):](#pengujian-testing)
        *   [unittest: Kerangka Kerja Pengujian Bawaan](#unittest-kerangka-kerja-pengujian-bawaan)
        *   [pytest: Kerangka Kerja Pengujian Populer](#pytest-kerangka-kerja-pengujian-populer)
    *   [*Catatan: Ini hanya pengenalan singkat, setiap pustaka memerlukan pembelajaran lebih lanjut*](#catatan-ini-hanya-pengenalan-singkat-setiap-pustaka-memerlukan-pembelajaran-lebih-lanjut)
13. [Praktik Terbaik dan Gaya Kode](#13-praktik-terbaik-dan-gaya-kode)
    *   [PEP 8 - Panduan Gaya Kode Python](#pep-8---panduan-gaya-kode-python)
        *   [Penamaan Variabel, Fungsi, Kelas, Modul](#penamaan-variabel-fungsi-kelas-modul)
        *   [Indentasi (4 spasi)](#indentasi-4-spasi)
        *   [Panjang Baris Maksimum](#panjang-baris-maksimum)
        *   [Komentar yang Efektif](#komentar-yang-efektif)
        *   [Whitespace](#whitespace)
    *   [Menulis Kode yang Pythonic](#menulis-kode-yang-pythonic)
        *   [Memanfaatkan Struktur Data Bawaan](#memanfaatkan-struktur-data-bawaan)
        *   [Menggunakan Comprehensions dan Generator](#menggunakan-comprehensions-dan-generator)
        *   [Menghindari Pengulangan Kode (DRY - Dont Repeat Yourself)](#menghindari-pengulangan-kode-dry---dont-repeat-yourself)
        *   [Menulis Kode yang Mudah Dibaca dan Dipelihara](#menulis-kode-yang-mudah-dibaca-dan-dipelihara)
    *   [Alat Bantu (Linters dan Formatters)](#alat-bantu-linters-dan-formatters)
        *   [Flake8 / Pylint (Linting)](#flake8--pylint-linting)
        *   [Black / YAPF (Formatting Otomatis)](#black--yapf-formatting-otomatis)
    *   [Manajemen Ketergantungan (Dependency Management)](#manajemen-ketergantungan-dependency-management)
        *   [`requirements.txt`](#requirementstxt-1)
        *   [Alat seperti Poetry atau Pipenv (Opsional Lanjutan)](#alat-seperti-poetry-atau-pipenv-opsional-lanjutan)
    *   [Kontrol Versi dengan Git](#kontrol-versi-dengan-git)
        *   [Mengapa Git Penting?](#mengapa-git-penting)
        *   [Perintah Dasar (`init`, `add`, `commit`, `status`, `log`, `branch`, `checkout`, `merge`, `push`, `pull`)](#perintah-dasar-init-add-commit-status-log-branch-checkout-merge-push-pull)
14. [Ide Proyek untuk Latihan](#14-ide-proyek-untuk-latihan)
    *   [Tingkat Pemula:](#tingkat-pemula)
        *   Kalkulator Sederhana
        *   Game Tebak Angka
        *   Konverter Satuan (Suhu, Panjang, dll)
        *   Generator Kata Sandi Sederhana
        *   Batu-Gunting-Kertas
    *   [Tingkat Menengah:](#tingkat-menengah)
        *   Aplikasi Todo List (Simpan ke file)
        *   Web Scraper Sederhana (misalnya, judul berita)
        *   Pengelola Kontak Sederhana
        *   Jam Pomodoro di Terminal
        *   Penganalisis Teks Sederhana (hitung kata, frekuensi huruf)
    *   [Tingkat Lanjut:](#tingkat-lanjut)
        *   Aplikasi Web Sederhana dengan Flask/Django (misalnya, Blog)
        *   Bot Otomatisasi (misalnya, bot Twitter/Discord sederhana)
        *   Alat Visualisasi Data Kecil
        *   Game Sederhana dengan Pygame
        *   API Sederhana
15. [Topik Lanjutan (Sekilas Pandang)](#15-topik-lanjutan-sekilas-pandang)
    *   [Asynchronous I/O (`asyncio`)](#asynchronous-io-asyncio)
    *   [Multithreading dan Multiprocessing](#multithreading-dan-multiprocessing)
    *   [Metaprogramming (Metaclasses)](#metaprogramming-metaclasses)
    *   [Descriptors](#descriptors)
    *   [Interaksi dengan C/C++ (ctypes, Cython)](#interaksi-dengan-cc-ctypes-cython)
    *   [Packaging dan Distribusi Kode](#packaging-dan-distribusi-kode)
16. [Sumber Belajar Lebih Lanjut](#16-sumber-belajar-lebih-lanjut)
    *   [Dokumentasi Python Resmi](#dokumentasi-python-resmi)
    *   [Buku Rekomendasi (misalnya, "Python Crash Course", "Fluent Python", "Automate the Boring Stuff with Python")](#buku-rekomendasi-misalnya-python-crash-course-fluent-python-automate-the-boring-stuff-with-python)
    *   [Kursus Online (Coursera, edX, Udemy, Codecademy, DataCamp, dll)](#kursus-online-coursera-edx-udemy-codecademy-datacamp-dll)
    *   [Platform Latihan Koding (HackerRank, LeetCode, Codewars)](#platform-latihan-koding-hackerrank-leetcode-codewars)
    *   [Komunitas (Stack Overflow, Reddit r/learnpython, Forum Diskusi Lokal/Online)](#komunitas-stack-overflow-reddit-rlearnpython-forum-diskusi-lokalonline)
17. [Kesimpulan dan Langkah Selanjutnya](#17-kesimpulan-dan-langkah-selanjutnya)
    *   [Terus Berlatih!](#terus-berlatih)
    *   [Berkontribusi pada Proyek Open Source](#berkontribusi-pada-proyek-open-source)
    *   [Bangun Portofolio Anda](#bangun-portofolio-anda)
    *   [Jangan Pernah Berhenti Belajar](#jangan-pernah-berhenti-belajar)

---

## 1. Pendahuluan

### Apa itu Python?

Python adalah bahasa pemrograman interpretatif tingkat tinggi yang serbaguna dan dinamis. Disebut "interpretatif" karena kode Python dieksekusi baris per baris oleh interpreter, bukan dikompilasi menjadi kode mesin sebelumnya (meskipun ada tahap kompilasi ke bytecode). "Tingkat tinggi" berarti sintaksnya lebih dekat ke bahasa manusia daripada bahasa mesin, menyembunyikan banyak detail kompleks dari perangkat keras. "Dinamis" mengacu pada fitur seperti pengetikan dinamis (tipe variabel ditentukan saat runtime).

### Sejarah Singkat Python

Python diciptakan oleh Guido van Rossum dan pertama kali dirilis pada tahun 1991. Nama "Python" terinspirasi dari acara komedi Inggris "Monty Python's Flying Circus". Python terus berkembang melalui kontribusi komunitas global di bawah naungan Python Software Foundation (PSF). Versi utama yang digunakan saat ini adalah Python 3.

### Filosofi Python (The Zen of Python)

Prinsip-prinsip desain Python dirangkum dalam "The Zen of Python" oleh Tim Peters. Anda bisa melihatnya dengan mengetik `import this` di interpreter Python. Beberapa prinsip utamanya adalah:

*   Beautiful is better than ugly. (Indah lebih baik daripada jelek)
*   Explicit is better than implicit. (Eksplisit lebih baik daripada implisit)
*   Simple is better than complex. (Sederhana lebih baik daripada kompleks)
*   Readability counts. (Keterbacaan itu penting)

### Bagaimana Menggunakan Panduan Ini

Panduan ini disusun secara berurutan, mulai dari dasar. Jika Anda pemula, sangat disarankan untuk mengikuti urutan dari awal. Jika Anda sudah memiliki pengalaman, gunakan Daftar Isi untuk melompat ke topik yang spesifik.

Setiap bagian akan berisi penjelasan konsep, contoh kode, dan terkadang latihan kecil atau poin penting yang perlu diperhatikan. Jangan ragu untuk mencoba menjalankan semua contoh kode di mesin Anda sendiri. **Praktik adalah kunci utama dalam belajar pemrograman.**

---

## 2. Persiapan Lingkungan Pengembangan

Sebelum mulai menulis kode Python, Anda perlu memastikan Python terinstal di komputer Anda dan menyiapkan lingkungan kerja yang nyaman.

### Instalasi Python

Kunjungi situs web resmi Python: [https://www.python.org/downloads/](https://www.python.org/downloads/)

#### Windows

1.  Unduh installer Windows terbaru (versi 3.x).
2.  Jalankan installer.
3.  **Penting:** Centang kotak "Add Python X.Y to PATH" atau "Add python.exe to PATH" di bagian bawah layar instalasi pertama. Ini akan memudahkan Anda menjalankan Python dari Command Prompt.
4.  Pilih "Install Now" (atau "Customize installation" jika Anda ingin mengubah lokasi atau fitur).
5.  Ikuti petunjuk hingga selesai.

#### macOS

macOS biasanya sudah terinstal Python 2.x versi lama atau Python 3.x yang mungkin bukan versi terbaru.

1.  Unduh installer macOS terbaru dari situs web Python.
2.  Jalankan installer `.pkg` yang diunduh.
3.  Ikuti petunjuk instalasi. Python 3 akan diinstal di `/Library/Frameworks/Python.framework/Versions/X.Y/` dan sebuah symlink biasanya akan dibuat di `/usr/local/bin/python3`.

Anda juga bisa menginstal Python menggunakan manajer paket seperti Homebrew (direkomendasikan jika Anda sudah menggunakan Homebrew):
```bash
brew update
brew install python
```

#### Linux

Sebagian besar distribusi Linux modern sudah menyertakan Python 3. Jika belum atau Anda ingin versi terbaru:

*   **Debian/Ubuntu:**
    ```bash
    sudo apt update
    sudo apt install python3 python3-pip python3-venv
    ```
*   **Fedora:**
    ```bash
    sudo dnf update
    sudo dnf install python3 python3-pip python3-venv # Nama paket venv mungkin berbeda
    ```
*   **Distro Lain:** Periksa manajer paket spesifik distro Anda (misalnya `pacman` untuk Arch, `zypper` untuk openSUSE). Cari paket `python3`, `python3-pip`, dan `python3-venv` (atau nama serupa).

### Memverifikasi Instalasi

Buka terminal atau Command Prompt Anda dan ketik perintah berikut:

```bash
python3 --version
# atau di Windows, jika 'Add to PATH' dicentang dan tidak bentrok dengan Python 2:
python --version
```

Anda juga perlu memeriksa `pip` (manajer paket Python):

```bash
pip3 --version
# atau di Windows:
pip --version
```

Jika perintah ini menampilkan nomor versi (misalnya, `Python 3.10.4`), instalasi Anda berhasil. Jika Anda mendapatkan error "command not found", periksa kembali langkah instalasi, terutama bagian "Add to PATH" di Windows atau pastikan symlink `python3` ada di PATH Anda di macOS/Linux.

### Editor Teks dan Integrated Development Environment (IDE)

Anda bisa menulis kode Python di editor teks sederhana seperti Notepad (Windows), TextEdit (Mac), atau Nano/Vim (Linux), tetapi menggunakan editor kode atau IDE khusus akan jauh lebih efisien.

#### Rekomendasi (VS Code, PyCharm, Sublime Text, dll)

*   **Visual Studio Code (VS Code):** Gratis, sangat populer, ringan, ekstensibel. Sangat direkomendasikan untuk pemula hingga profesional. Instal ekstensi "Python" dari Microsoft.
*   **PyCharm:** IDE khusus Python yang sangat kuat. Memiliki edisi "Community" (gratis) dan "Professional" (berbayar). Sangat baik untuk proyek besar dan pengembangan web/data science. Mungkin sedikit *overkill* untuk pemula absolut, tetapi fiturnya sangat lengkap.
*   **Sublime Text:** Editor teks cepat dan dapat disesuaikan. Memerlukan beberapa konfigurasi dan instalasi paket untuk pengalaman pengembangan Python yang optimal.
*   **Jupyter Notebook/Lab:** Populer di kalangan ilmuwan data. Memungkinkan Anda menjalankan kode dalam sel interaktif dan menggabungkannya dengan teks, gambar, dan visualisasi. Sangat baik untuk eksplorasi data dan prototyping.

Pilih yang paling nyaman bagi Anda. VS Code adalah titik awal yang bagus.

#### Menjalankan Kode Python

Ada beberapa cara:

1.  **Interpreter Interaktif:** Buka terminal/Command Prompt, ketik `python3` (atau `python`), dan tekan Enter. Anda akan masuk ke *shell* Python (`>>>`), di mana Anda bisa mengetik dan mengeksekusi perintah Python satu per satu. Ketik `exit()` atau tekan `Ctrl+D` (Linux/macOS) atau `Ctrl+Z` lalu `Enter` (Windows) untuk keluar.
2.  **Menjalankan File:**
    *   Tulis kode Anda dalam file teks dengan ekstensi `.py` (misalnya, `hello.py`).
    *   Simpan file tersebut.
    *   Buka terminal/Command Prompt, navigasikan ke direktori tempat Anda menyimpan file menggunakan perintah `cd` (change directory).
    *   Jalankan dengan perintah: `python3 hello.py` (atau `python hello.py`).

```python
# Contoh isi file hello.py
print("Halo, Dunia Python!")
nama = input("Masukkan nama Anda: ")
print(f"Senang bertemu denganmu, {nama}!")
```

### Lingkungan Virtual (Virtual Environments)

Sangat penting untuk menggunakan lingkungan virtual untuk setiap proyek Python yang berbeda.

#### Mengapa Menggunakan Lingkungan Virtual?

*   **Isolasi Ketergantungan:** Setiap proyek mungkin memerlukan versi pustaka (library) yang berbeda. Lingkungan virtual memungkinkan Anda menginstal pustaka spesifik untuk satu proyek tanpa memengaruhi proyek lain atau instalasi Python global Anda.
*   **Menghindari Konflik:** Mencegah konflik versi antar pustaka yang mungkin dibutuhkan oleh proyek yang berbeda.
*   **Reproduktifitas:** Memudahkan orang lain (atau Anda di masa depan/di komputer lain) untuk menyiapkan proyek dengan dependensi yang sama persis menggunakan file `requirements.txt`.

#### Membuat dan Mengaktifkan Lingkungan Virtual (`venv`)

`venv` adalah modul bawaan Python (sejak 3.3) untuk membuat lingkungan virtual.

1.  **Navigasi ke Direktori Proyek Anda:**
    ```bash
    mkdir proyek_python_saya
    cd proyek_python_saya
    ```
2.  **Buat Lingkungan Virtual:** (Ganti `env` dengan nama yang Anda inginkan, `env` atau `.venv` adalah konvensi umum)
    ```bash
    python3 -m venv env
    # atau di Windows:
    python -m venv env
    ```
    Ini akan membuat direktori `env` (atau nama yang Anda pilih) yang berisi salinan interpreter Python dan struktur direktori lainnya. *Catatan: Disarankan menambahkan nama direktori venv Anda (misal `env/` atau `.venv/`) ke file `.gitignore` agar tidak ter-commit ke Git.*
3.  **Aktifkan Lingkungan Virtual:**
    *   **macOS/Linux (bash/zsh):**
        ```bash
        source env/bin/activate
        ```
        Anda akan melihat nama lingkungan (misalnya `(env)`) muncul di awal prompt terminal Anda.
    *   **Windows (Command Prompt):**
        ```cmd
        .\env\Scripts\activate.bat
        ```
    *   **Windows (PowerShell):**
        ```powershell
        .\env\Scripts\Activate.ps1
        ```
        (Anda mungkin perlu mengubah Execution Policy jika ini pertama kalinya: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser` atau `-Scope Process`)
    *   **Windows (Git Bash):**
        ```bash
        source env/Scripts/activate
        ```
4.  **Bekerja di Lingkungan Virtual:** Sekarang, `python` dan `pip` akan merujuk ke versi yang ada di dalam lingkungan virtual `env`. Instalasi paket hanya akan terjadi di dalam lingkungan ini.
5.  **Nonaktifkan Lingkungan Virtual:** Cukup ketik `deactivate` di terminal Anda.

**Selalu aktifkan lingkungan virtual Anda sebelum mulai bekerja pada sebuah proyek Python.**

### Manajer Paket `pip`

`pip` adalah manajer paket standar untuk Python. Anda menggunakannya untuk menginstal dan mengelola pustaka (paket) pihak ketiga yang tidak termasuk dalam instalasi Python standar (yaitu dari Python Package Index - PyPI).

#### Instalasi Paket

Pastikan lingkungan virtual Anda aktif.

```bash
pip install nama_paket
# Contoh: Instal pustaka 'requests' untuk membuat permintaan HTTP
pip install requests
# Contoh: Instal pustaka 'pandas' untuk analisis data
pip install pandas
# Instal versi spesifik
pip install requests==2.27.1
# Instal dari file requirements.txt
pip install -r requirements.txt
```

#### Melihat Paket Terinstal

```bash
pip list       # Menampilkan semua paket di lingkungan saat ini (termasuk pip, setuptools)
pip freeze     # Menampilkan paket terinstal dalam format requirements.txt (lebih bersih untuk dibagikan)
```

#### `requirements.txt`

Ini adalah file teks standar yang mencantumkan semua dependensi (pustaka pihak ketiga) yang dibutuhkan oleh proyek Anda, biasanya beserta versinya. Ini memungkinkan orang lain (atau Anda) untuk dengan mudah menginstal semua dependensi yang diperlukan untuk menjalankan proyek.

1.  **Membuat `requirements.txt`:** Setelah menginstal semua dependensi yang dibutuhkan proyek Anda di lingkungan virtual aktif:
    ```bash
    pip freeze > requirements.txt
    ```
2.  **Menginstal dari `requirements.txt`:** Di lingkungan virtual baru atau di komputer lain (pastikan venv sudah aktif):
    ```bash
    pip install -r requirements.txt
    ```

Sangat disarankan untuk menyertakan file `requirements.txt` dalam repositori Git Anda (dan *tidak* menyertakan direktori `env` atau `.venv` itu sendiri).

---

## 3. Dasar-Dasar Python

Sekarang mari kita mulai mempelajari bahasa Python itu sendiri.

### Sintaks Dasar dan Komentar

*   **Indentasi Penting:** Tidak seperti banyak bahasa lain yang menggunakan kurung kurawal `{}` untuk menandai blok kode, Python menggunakan **indentasi** (konvensi umum adalah **4 spasi** per level indentasi). Konsistensi indentasi sangat krusial. Blok kode di bawah `if`, `for`, `def`, `class`, dll., harus diindentasi. Kesalahan indentasi akan menyebabkan `IndentationError`.
*   **Akhir Baris:** Umumnya, satu pernyataan per baris. Titik koma (`;`) tidak diperlukan untuk mengakhiri pernyataan, meskipun bisa digunakan untuk menempatkan beberapa pernyataan pendek di satu baris (tidak disarankan karena mengurangi keterbacaan).
*   **Sensitif Huruf (Case-Sensitive):** `variabel`, `Variabel`, dan `VARIABEL` dianggap sebagai tiga nama yang berbeda.
*   **Komentar:** Digunakan untuk menjelaskan kode. Interpreter Python akan mengabaikannya.
    *   Komentar satu baris dimulai dengan tanda pagar (`#`).
    *   Komentar multi-baris secara teknis tidak ada, tetapi string multi-baris (menggunakan tiga tanda kutip `"""..."""` atau `'''...'''`) yang tidak ditugaskan ke variabel sering digunakan sebagai gantinya, terutama untuk *docstrings*.

    ```python
    # Ini adalah komentar satu baris
    print("Halo!") # Ini komentar di akhir baris

    # Komentar
    # multi-baris
    # dibuat dengan beberapa tanda # di awal setiap baris

    """
    Ini adalah docstring multi-baris.
    Bisa juga digunakan sebagai blok komentar, meskipun secara teknis
    ini adalah string literal yang tidak disimpan ke mana pun.
    Sering digunakan untuk dokumentasi fungsi atau kelas.
    """
    x = 10 # Contoh kode setelah komentar
    ```

### Variabel dan Tipe Data

Variabel adalah wadah bernama untuk menyimpan nilai data. Di Python, Anda tidak perlu mendeklarasikan tipe variabel secara eksplisit sebelum menggunakannya. Tipe ditentukan secara otomatis saat Anda memberikan nilai pertama kali (ini disebut *dynamic typing*).

#### Aturan Penamaan Variabel

*   Harus dimulai dengan huruf (a-z, A-Z) atau garis bawah (`_`).
*   Dapat diikuti oleh huruf, angka (0-9), atau garis bawah.
*   **Tidak boleh** berupa kata kunci Python (reserved keywords) seperti `if`, `else`, `for`, `while`, `def`, `class`, `import`, `try`, `except`, dll. (Anda bisa melihat daftar lengkapnya dengan `import keyword; print(keyword.kwlist)`).
*   Bersifat case-sensitive (`nama` berbeda dari `Nama`).
*   **Konvensi (PEP 8):** Gunakan `snake_case` (huruf kecil semua dengan kata-kata dipisahkan oleh garis bawah) untuk nama variabel dan fungsi (misalnya, `nama_pengguna`, `hitung_total_harga`). Gunakan `CamelCase` untuk nama kelas (misalnya, `NamaKelasSaya`).

```python
# Contoh penamaan variabel yang valid
nama_depan = "Budi"
umur = 25
_nilai_sementara = 100
TOTAL_HARGA = 5000 # Konvensi untuk konstanta (meskipun Python tidak punya konstanta sejati)

# Contoh penamaan variabel yang TIDAK valid
# 1angka = 10      # Tidak boleh diawali angka
# nama-belakang = "S" # Tidak boleh ada tanda hubung
# class = "Python" # Tidak boleh menggunakan keyword
```

#### Tipe Data Dasar

Python memiliki beberapa tipe data bawaan yang fundamental:

*   **`int` (Integer):** Bilangan bulat positif atau negatif, tanpa bagian desimal, dengan presisi tak terbatas (hanya dibatasi oleh memori). Contoh: `10`, `-5`, `0`, `999999999999999999999`.
    ```python
    jumlah_siswa = 30
    suhu_beku = -5
    tahun = 2024
    ```
*   **`float` (Floating-Point):** Bilangan yang memiliki bagian desimal, atau ditulis dengan notasi ilmiah. Menggunakan titik (`.`) sebagai pemisah desimal. Contoh: `3.14`, `-0.5`, `2.71828`, `10.0`, `2.5e2` (artinya 2.5 * 10^2 = 250.0). Float memiliki presisi terbatas.
    ```python
    harga_barang = 99.99
    phi = 3.14159
    jarak = 15.5
    saldo = 100.0 # Ini juga float
    ```
*   **`str` (String):** Urutan karakter (teks). Didefinisikan menggunakan tanda kutip tunggal (`'...'`), tanda kutip ganda (`"..."`), atau tiga tanda kutip (`'''...'''` atau `"""..."""` untuk string yang bisa mencakup beberapa baris). String bersifat *immutable* (tidak bisa diubah isinya setelah dibuat).
    ```python
    nama = "Alice"
    pesan = 'Selamat Pagi!'
    kalimat_panjang = """Ini adalah contoh string
    yang terdiri dari beberapa baris.
    Indentasi dan newline dipertahankan."""
    string_kosong = ""
    ```
*   **`bool` (Boolean):** Mewakili nilai kebenaran logis, hanya bisa `True` atau `False` (perhatikan huruf kapital di awal). Sangat penting dalam struktur kontrol alur (if, while).
    ```python
    sedang_belajar = True
    sudah_lulus = False
    ```
*   **`NoneType`:** Tipe data khusus yang hanya memiliki satu nilai: `None`. Digunakan untuk merepresentasikan ketiadaan nilai, nilai null, atau kondisi kosong/tidak terdefinisi. Berbeda dari `0`, `False`, atau string kosong `""`.
    ```python
    hasil_pencarian = None # Belum ada hasil ditemukan
    nilai_default = None
    ```

#### Pengecekan Tipe (`type()`)

Anda bisa menggunakan fungsi bawaan `type()` untuk mengetahui tipe data dari suatu variabel atau nilai.

```python
x = 10
y = 3.14
z = "Halo"
a = True
b = None
c = [1, 2] # Ini adalah tipe list (akan dibahas nanti)

print(f"Tipe data x ({x}): {type(x)}")  # Output: <class 'int'>
print(f"Tipe data y ({y}): {type(y)}")  # Output: <class 'float'>
print(f"Tipe data z ('{z}'): {type(z)}")  # Output: <class 'str'>
print(f"Tipe data a ({a}): {type(a)}")  # Output: <class 'bool'>
print(f"Tipe data b ({b}): {type(b)}")  # Output: <class 'NoneType'>
print(f"Tipe data c ({c}): {type(c)}")  # Output: <class 'list'>
```

#### Konversi Tipe Data (Type Casting)

Terkadang Anda perlu mengonversi nilai dari satu tipe ke tipe lain. Gunakan fungsi bawaan dengan nama tipe yang diinginkan: `int()`, `float()`, `str()`, `bool()`.

```python
angka_str = "123"
angka_int = int(angka_str) # Konversi string ke integer
print(f"'{angka_str}' sebagai int: {angka_int}, tipenya: {type(angka_int)}")

angka_float = float(angka_int) # Konversi integer ke float
print(f"{angka_int} sebagai float: {angka_float}, tipenya: {type(angka_float)}")

angka_desimal_str = "99.5"
angka_desimal_float = float(angka_desimal_str) # String desimal ke float
print(f"'{angka_desimal_str}' sebagai float: {angka_desimal_float}, tipenya: {type(angka_desimal_float)}")
# angka_desimal_int = int(angka_desimal_str) # Ini akan error (ValueError)! int() tidak bisa langsung dari string float.
angka_desimal_int = int(angka_desimal_float) # Konversi float ke int (bagian desimal dihilangkan/truncated)
print(f"{angka_desimal_float} sebagai int: {angka_desimal_int}, tipenya: {type(angka_desimal_int)}") # Output: 99

nilai_int = 0
nilai_bool_dari_int = bool(nilai_int) # Konversi int ke boolean (0 -> False, selain 0 -> True)
print(f"{nilai_int} sebagai bool: {nilai_bool_dari_int}") # Output: False

string_kosong = ""
nilai_bool_dari_str = bool(string_kosong) # String kosong -> False, string isi -> True
print(f"String kosong '' sebagai bool: {nilai_bool_dari_str}") # Output: False

nilai_str_dari_bool = str(True) # Konversi boolean ke string
print(f"True sebagai str: '{nilai_str_dari_bool}', tipenya: {type(nilai_str_dari_bool)}") # Output: 'True'

# Konversi ke int dari string non-angka akan error
# coba_int = int("halo") # ValueError: invalid literal for int() with base 10: 'halo'
```

### Operator

Operator adalah simbol khusus yang melakukan operasi pada nilai (operand).

#### Operator Aritmatika (`+`, `-`, `*`, `/`, `%`, `**`, `//`)

Digunakan untuk operasi matematika dasar.

*   `+`: Penjumlahan (juga untuk menggabungkan string/list)
*   `-`: Pengurangan
*   `*`: Perkalian (juga untuk mengulang string/list)
*   `/`: Pembagian (hasilnya **selalu float**, bahkan jika pembagiannya habis)
*   `%`: Modulo (sisa hasil bagi)
*   `**`: Eksponensial (pangkat)
*   `//`: Pembagian Bulat (floor division - membulatkan hasil pembagian ke bawah ke bilangan bulat terdekat)

```python
a = 17
b = 5

print(f"{a} + {b} = {a + b}")  # Output: 22
print(f"{a} - {b} = {a - b}")  # Output: 12
print(f"{a} * {b} = {a * b}")  # Output: 85
print(f"{a} / {b} = {a / b}")  # Output: 3.4 (float!)
print(f"{a} % {b} = {a % b}")  # Output: 2 (17 dibagi 5 adalah 3 sisa 2)
print(f"{a} ** {b} = {a ** b}") # Output: 1419857 (17 pangkat 5)
print(f"{a} // {b} = {a // b}") # Output: 3 (hasil 3.4 dibulatkan ke bawah)

print(f"18 / 6 = {18 / 6}")   # Output: 3.0 (tetap float!)
print(f"18 // 6 = {18 // 6}")  # Output: 3 (int)

print("Halo" + " " + "Dunia") # Output: Halo Dunia
print("ha" * 5)              # Output: hahahahaha
```

#### Operator Perbandingan (`==`, `!=`, `>`, `<`, `>=`, `<=`)

Membandingkan dua nilai dan menghasilkan nilai Boolean (`True` atau `False`).

*   `==`: Sama dengan
*   `!=`: Tidak sama dengan
*   `>`: Lebih besar dari
*   `<`: Lebih kecil dari
*   `>=`: Lebih besar dari atau sama dengan
*   `<=`: Lebih kecil dari atau sama dengan

```python
x = 10
y = 5
z = 10

print(f"{x} == {y} : {x == y}") # Output: False
print(f"{x} != {y} : {x != y}") # Output: True
print(f"{x} > {y} : {x > y}")   # Output: True
print(f"{x} < {y} : {x < y}")   # Output: False
print(f"{x} >= {z} : {x >= z}") # Output: True
print(f"{x} <= {z} : {x <= z}") # Output: True

print(f"'apel' == 'jeruk' : {'apel' == 'jeruk'}") # Output: False
print(f"'apel' < 'jeruk' : {'apel' < 'jeruk'}")   # Output: True (perbandingan leksikografis/urutan alfabet)
```

#### Operator Logika (`and`, `or`, `not`)

Menggabungkan atau membalikkan ekspresi Boolean.

*   `and`: Menghasilkan `True` jika *kedua* operand `True`.
*   `or`: Menghasilkan `True` jika *salah satu* atau kedua operand `True`.
*   `not`: Membalikkan nilai Boolean (`True` menjadi `False`, `False` menjadi `True`).

```python
usia = 20
punya_sim = True
nilai_cukup = False

# Cek syarat kelulusan: usia >= 17 DAN punya SIM
bisa_mengemudi = usia >= 17 and punya_sim
print(f"Bisa mengemudi? {bisa_mengemudi}") # Output: True

# Cek kondisi: punya SIM ATAU nilai cukup
memenuhi_syarat_lain = punya_sim or nilai_cukup
print(f"Memenuhi syarat lain? {memenuhi_syarat_lain}") # Output: True

# Cek kebalikan dari nilai_cukup
tidak_cukup = not nilai_cukup
print(f"Nilai tidak cukup? {tidak_cukup}") # Output: True

# Urutan evaluasi: not dievaluasi dulu, lalu and, lalu or
# Gunakan kurung () untuk kejelasan atau mengubah urutan
print(not punya_sim or nilai_cukup and usia > 18) # Sulit dibaca
print((not punya_sim) or (nilai_cukup and (usia > 18))) # Lebih jelas
```

**Short-circuit Evaluation:** Python menggunakan evaluasi sirkuit pendek untuk `and` dan `or`.
*   Untuk `A and B`: Jika `A` dievaluasi `False`, `B` *tidak akan* dievaluasi sama sekali (karena hasilnya pasti `False`).
*   Untuk `A or B`: Jika `A` dievaluasi `True`, `B` *tidak akan* dievaluasi sama sekali (karena hasilnya pasti `True`).
Ini penting jika operand kedua adalah pemanggilan fungsi yang mahal atau memiliki efek samping.

#### Operator Penugasan (`=`, `+=`, `-=`, `*=`, `/=`, `%=`, `**=`, `//=`)

Digunakan untuk memberikan nilai ke variabel.

*   `=`: Penugasan dasar.
*   `+=`, `-=`, `*=`, `/=`, `%=`, `**=`, `//=`: Operator penugasan gabungan. Melakukan operasi aritmatika lalu menugaskan hasilnya kembali ke variabel di sebelah kiri. `x += 5` adalah singkatan dari `x = x + 5`.

```python
total = 100

# Penugasan dasar
diskon = 10
total = total - diskon # total menjadi 90
print(f"Total setelah diskon: {total}")

# Penugasan gabungan
pajak = 5
total += pajak # total = total + pajak (90 + 5 = 95)
print(f"Total setelah pajak (+): {total}")

jumlah_barang = 3
total *= jumlah_barang # total = total * jumlah_barang (95 * 3 = 285)
print(f"Total setelah dikali jumlah (*): {total}")

# Contoh lain
sisa = 17
sisa %= 5 # sisa = sisa % 5 (17 % 5 = 2)
print(f"Sisa setelah modulo (%=): {sisa}")

pangkat = 2
pangkat **= 3 # pangkat = pangkat ** 3 (2 ** 3 = 8)
print(f"Pangkat setelah eksponen (**=): {pangkat}")
```

#### Operator Keanggotaan (`in`, `not in`)

Memeriksa apakah suatu nilai ada di dalam sebuah urutan (seperti string, list, tuple, set, dictionary (cek kunci)). Menghasilkan `True` atau `False`.

```python
nama = "Python Programming"
daftar_angka = [1, 2, 3, 4, 5]
data_dict = {'a': 1, 'b': 2}

print(f"'P' in nama? {'P' in nama}")                 # Output: True
print(f"'Java' in nama? {'Java' in nama}")           # Output: False
print(f"'gram' in nama? {'gram' in nama}")         # Output: True

print(f"3 in daftar_angka? {3 in daftar_angka}")       # Output: True
print(f"10 not in daftar_angka? {10 not in daftar_angka}") # Output: True

print(f"'a' in data_dict? {'a' in data_dict}")       # Output: True (cek kunci)
print(f"1 in data_dict? {1 in data_dict}")         # Output: False (tidak cek nilai secara default)
print(f"1 in data_dict.values()? {1 in data_dict.values()}") # Output: True (cek nilai jika eksplisit)
```

#### Operator Identitas (`is`, `is not`)

Memeriksa apakah dua variabel merujuk ke **objek yang sama persis** di memori, bukan hanya apakah nilainya sama. Menghasilkan `True` atau `False`.

```python
list_a = [1, 2, 3]
list_b = [1, 2, 3]
list_c = list_a

print(f"list_a == list_b : {list_a == list_b}") # Output: True (Nilainya sama)
print(f"list_a is list_b : {list_a is list_b}") # Output: False (Objek berbeda di memori)

print(f"list_a == list_c : {list_a == list_c}") # Output: True (Nilainya sama)
print(f"list_a is list_c : {list_a is list_c}") # Output: True (Merujuk ke objek yang sama)

print(f"list_a is not list_b : {list_a is not list_b}") # Output: True

# Perhatian dengan immutable kecil (angka kecil, string pendek)
# Python sering mengoptimalkannya (interning), jadi 'is' bisa True
x = 256
y = 256
print(f"\nx={x}, y={y}")
print(f"x == y : {x == y}") # Output: True
print(f"x is y : {x is y}") # Output: True (karena interning angka kecil)

a = 257
b = 257
print(f"\na={a}, b={b}")
print(f"a == b : {a == b}") # Output: True
print(f"a is b : {a is b}") # Output: False (biasanya, di luar rentang interning)

s1 = "python"
s2 = "python"
print(f"\ns1='{s1}', s2='{s2}'")
print(f"s1 == s2 : {s1 == s2}") # Output: True
print(f"s1 is s2 : {s1 is s2}") # Output: True (seringkali karena interning string)

# Kesimpulan: Gunakan '==' untuk membandingkan nilai,
# gunakan 'is' hanya jika Anda benar-benar perlu memeriksa identitas objek.
# Sering digunakan untuk mengecek dengan None: if my_var is None: ...
```

#### Operator Bitwise (Opsional Lanjutan)

Operator ini bekerja pada representasi biner (bit) dari bilangan bulat: `&` (AND), `|` (OR), `^` (XOR), `~` (NOT/Complement), `<<` (Left Shift), `>>` (Right Shift). Biasanya digunakan dalam pemrograman tingkat rendah, manipulasi data biner, atau optimasi spesifik. Tidak akan dibahas mendalam di sini.

### Input dan Output Dasar

#### Fungsi `print()`

Digunakan untuk menampilkan output (mencetak) ke konsol/terminal.

```python
print("Halo, ini pesan sederhana.")

nama = "Budi"
umur = 30
print("Nama:", nama, "Umur:", umur) # Otomatis menambahkan spasi antar argumen

# Mengontrol pemisah (sep) dan akhir baris (end)
print("Apel", "Jeruk", "Mangga", sep=", ") # Output: Apel, Jeruk, Mangga
print("Baris pertama.", end=" ") # Tidak pindah baris
print("Masih di baris pertama.")

# Menggunakan f-string (cara modern dan paling direkomendasikan)
print(f"\nNama saya {nama} dan umur saya {umur} tahun.")
print(f"Tahun depan umur saya {umur + 1}.")
nilai = 95.678
print(f"Nilai ujian: {nilai:.2f}") # Format float 2 angka desimal
```

#### Fungsi `input()`

Digunakan untuk menerima input dari pengguna melalui konsol. Selalu mengembalikan input sebagai **string**, bahkan jika pengguna mengetik angka. Anda perlu melakukan konversi tipe jika memerlukan tipe lain (misalnya `int` atau `float`).

```python
nama_pengguna = input("Siapa nama Anda? ")
print(f"Halo, {nama_pengguna}!")

# Meminta input angka (ingat untuk konversi)
usia_str = input(f"Berapa usia Anda, {nama_pengguna}? ")
try:
    usia_int = int(usia_str) # Konversi ke integer
    tahun_lahir = 2024 - usia_int
    print(f"Wow, Anda lahir sekitar tahun {tahun_lahir}.")
except ValueError:
    print(f"Maaf, '{usia_str}' sepertinya bukan angka usia yang valid.")

# Meminta input float
tinggi_str = input("Berapa tinggi badan Anda (dalam meter)? ")
try:
    tinggi_float = float(tinggi_str)
    print(f"Tinggi Anda adalah {tinggi_float} meter.")
except ValueError:
    print(f"Input tinggi '{tinggi_str}' tidak valid.")
```

### String Lanjutan

String adalah tipe data yang sangat penting dan sering digunakan. Mari kita lihat beberapa operasinya lebih detail.

#### Indexing dan Slicing

String adalah urutan karakter, jadi Anda bisa mengakses karakternya menggunakan indeks (dimulai dari 0) atau mengambil sebagian (slice).

*   **Indexing:** Mengambil satu karakter. Indeks negatif dimulai dari akhir (-1 adalah karakter terakhir, -2 adalah kedua terakhir, dst.). Mengakses indeks di luar jangkauan akan menyebabkan `IndexError`.
*   **Slicing:** Mengambil sebagian string. Format: `[start:stop:step]`.
    *   `start`: Indeks awal (inklusif, default 0).
    *   `stop`: Indeks akhir (**eksklusif**, default akhir string).
    *   `step`: Lompatan antar indeks (default 1). `step` negatif membalik urutan.

```python
teks = "Belajar Python"
# Indeks: 01234567890123
#        B e l a j a r   P y t h o n
# Negatif:-4-3-2-1

# Indexing
print(f"Karakter ke-0: {teks[0]}")   # Output: B
print(f"Karakter ke-8: {teks[8]}")   # Output: P
print(f"Karakter terakhir (-1): {teks[-1]}")  # Output: n
print(f"Karakter ke-2 dari akhir (-2): {teks[-2]}") # Output: o
# print(teks[14]) # IndexError

# Slicing
print(f"Slice [0:7]: {teks[0:7]}")  # Output: Belajar (indeks 0 sampai sebelum 7)
print(f"Slice [8:]: {teks[8:]}")   # Output: Python (indeks 8 sampai akhir)
print(f"Slice [:7]: {teks[:7]}")   # Output: Belajar (awal sampai sebelum 7)
print(f"Slice [:]: {teks[:]}")    # Output: Belajar Python (salinan seluruh string)
print(f"Slice [0:14:2]: {teks[0:14:2]}")# Output: BljrPto (lompatan 2)
print(f"Slice [::-1]: {teks[::-1]}") # Output: nohtyP rajaleB (membalik string)
print(f"Slice [5:1:-1]: {teks[5:1:-1]}") # Output: ajal (dari indeks 5 mundur sampai sebelum 1)
```

Ingat: String bersifat *immutable*. Operasi slicing atau metode string selalu membuat string *baru*, tidak mengubah string asli.

```python
nama_awal = "Andi"
# nama_awal[0] = "B" # Ini akan menghasilkan TypeError! String tidak bisa diubah.
nama_baru = "B" + nama_awal[1:] # Membuat string baru
print(f"Nama baru: {nama_baru}") # Output: Budi
```

#### Metode String Umum (`upper()`, `lower()`, `strip()`, `split()`, `join()`, `replace()`, `find()`, `startswith()`, `endswith()`, dll)

String memiliki banyak metode bawaan yang sangat berguna untuk manipulasi teks. Metode dipanggil menggunakan notasi titik (`.`) setelah variabel string. Metode ini mengembalikan *string baru* (atau kadang tipe lain seperti list untuk `split()`).

*   `upper()`: Mengubah semua huruf menjadi kapital.
*   `lower()`: Mengubah semua huruf menjadi kecil.
*   `capitalize()`: Mengubah huruf pertama string menjadi kapital, sisanya kecil.
*   `title()`: Mengubah huruf pertama *setiap kata* menjadi kapital.
*   `strip()`: Menghapus whitespace (spasi, tab, newline) dari *awal dan akhir* string. `lstrip()` hanya dari kiri, `rstrip()` hanya dari kanan. Bisa juga diberi argumen karakter yang ingin dihapus.
*   `split(separator=None, maxsplit=-1)`: Memecah string menjadi **list** berdasarkan `separator`.
    *   Jika `separator` tidak diberikan atau `None`, memecah berdasarkan whitespace (satu atau lebih spasi/tab/newline) dan mengabaikan string kosong.
    *   Jika `separator` diberikan (misal `','` atau `'-'`), memecah tepat di separator tersebut.
    *   `maxsplit` membatasi jumlah pemecahan.
*   `join(iterable)`: Menggabungkan elemen-elemen dari `iterable` (seperti list of strings) menjadi satu string, dengan *string pemanggil* sebagai pemisah antar elemen.
*   `replace(old, new, count=-1)`: Mengganti semua kemunculan substring `old` dengan `new`. `count` opsional membatasi jumlah penggantian.
*   `find(substring, start=0, end=len(string))`: Mencari `substring` dalam string (atau dalam slice `start:end`), mengembalikan indeks **pertama kali ditemukan**, atau **-1** jika tidak ditemukan.
*   `index(substring, start=0, end=len(string))`: Sama seperti `find()`, tapi membangkitkan **`ValueError`** jika `substring` tidak ditemukan (bukan -1).
*   `startswith(prefix, start=0, end=len(string))`: Mengembalikan `True` jika string dimulai dengan `prefix`.
*   `endswith(suffix, start=0, end=len(string))`: Mengembalikan `True` jika string diakhiri dengan `suffix`.
*   `count(substring, start=0, end=len(string))`: Menghitung berapa kali `substring` muncul dalam string.
*   `isdigit()`: `True` jika semua karakter adalah digit (0-9) dan string tidak kosong.
*   `isalpha()`: `True` jika semua karakter adalah huruf alfabet dan string tidak kosong.
*   `isalnum()`: `True` jika semua karakter alfanumerik (huruf atau angka) dan string tidak kosong.
*   `isspace()`: `True` jika semua karakter adalah whitespace dan string tidak kosong.
*   `islower()`: `True` jika semua huruf adalah lowercase.
*   `isupper()`: `True` jika semua huruf adalah uppercase.
*   `istitle()`: `True` jika string dalam format title case.

```python
kalimat = "   Python itu Seru dan Mudah!   "
kata_kunci = "pemrograman,python,mudah"
url = "https://www.example.com/data"

print(f"Original: '{kalimat}'")
print(f"upper(): '{kalimat.upper()}'")        # Output:    PYTHON ITU SERU DAN MUDAH!
print(f"lower(): '{kalimat.lower()}'")        # Output:    python itu seru dan mudah!
print(f"strip(): '{kalimat.strip()}'")        # Output: Python itu Seru dan Mudah!
print(f"capitalize(): '{kalimat.strip().capitalize()}'") # Output: Python itu seru dan mudah!
print(f"title(): '{kalimat.strip().title()}'") # Output: Python Itu Seru Dan Mudah!

# strip karakter spesifik
judul = "---Judul Utama---"
print(f"strip('-'): '{judul.strip('-')}'") # Output: Judul Utama

# split
daftar_kata = kalimat.strip().split() # Memecah berdasarkan spasi
print(f"split(): {daftar_kata}")            # Output: ['Python', 'itu', 'Seru', 'dan', 'Mudah!']
tags = kata_kunci.split(',')
print(f"split(','): {tags}")            # Output: ['pemrograman', 'python', 'mudah']

# join
pemisah = " | "
print(f"join(tags): '{pemisah.join(tags)}'") # Output: pemrograman | python | mudah

# replace
print(f"replace('Python', 'Pemrograman'): '{kalimat.replace('Python', 'Pemrograman')}'")
print(f"replace('!', '.', 1): '{kalimat.replace('!', '.', 1)}'") # Ganti ! pertama saja

# find & index
print(f"find('itu'): {kalimat.find('itu')}")      # Output: 10 (indeks pertama)
print(f"find('Java'): {kalimat.find('Java')}")     # Output: -1 (tidak ditemukan)
# print(f"index('Java'): {kalimat.index('Java')}") # ValueError

# startswith & endswith
print(f"kalimat starts '   P'? {kalimat.startswith('   P')}") # True
print(f"kalimat.strip() ends '!': {kalimat.strip().endswith('!')}") # True
print(f"url starts 'https': {url.startswith('https')}") # True

# count
print(f"count 'a': {kalimat.lower().count('a')}") # Hitung 'a' (setelah lower case)

# is... methods
angka_str = "12345"
huruf_str = "Python"
alpha_num = "Python3"
spasi_str = "   \t\n"
print(f"'{angka_str}'.isdigit()? {angka_str.isdigit()}") # True
print(f"'{huruf_str}'.isalpha()? {huruf_str.isalpha()}") # True
print(f"'{alpha_num}'.isalnum()? {alpha_num.isalnum()}") # True
print(f"'{kalimat}'.islower()? {kalimat.islower()}") # False
print(f"'judul'.istitle()? {'Judul Contoh'.istitle()}") # True
print(f"'{spasi_str}'.isspace()? {spasi_str.isspace()}") # True
```

#### F-Strings (Formatted String Literals)

Diperkenalkan di Python 3.6, f-string adalah cara paling modern, mudah dibaca, dan seringkali paling efisien untuk memformat string dengan menyisipkan nilai variabel atau hasil ekspresi. Awali string literal dengan huruf `f` atau `F` (sebelum tanda kutip), lalu masukkan variabel atau ekspresi di dalam kurung kurawal `{}`.

```python
nama = "Citra"
umur = 22
pekerjaan = "Software Engineer"
gaji = 15500750.50
list_hobi = ["Membaca", "Coding", "Hiking"]

# Cara lama (kurang disarankan sekarang)
# print("Nama: " + nama + ", Umur: " + str(umur)) # Kurang efisien, rawan TypeError
# print("Nama: %s, Umur: %d" % (nama, umur)) # Gaya C-style (lama)
# print("Nama: {}, Umur: {}".format(nama, umur)) # Metode .format() (masih oke, tapi f-string lebih ringkas)

# Menggunakan F-String (DISARANKAN)
print(f"--- Profil {nama} ---")
print(f"Usia: {umur} tahun")
print(f"Pekerjaan: {pekerjaan}")

# Bisa memasukkan ekspresi langsung di dalam {}
print(f"Dalam 5 tahun, {nama} akan berumur {umur + 5} tahun.")
print(f"Nama dalam huruf kapital: {nama.upper()}")
print(f"Jumlah hobi: {len(list_hobi)}")
print(f"Hobi pertama: {list_hobi[0]}")

# Opsi formatting di dalam {} setelah titik dua ':'
# :.2f -> format float 2 angka desimal
# :, -> gunakan koma sebagai pemisah ribuan
# :>10 -> rata kanan dalam 10 karakter
# :<10 -> rata kiri dalam 10 karakter
# :^10 -> rata tengah dalam 10 karakter
# :05d -> format integer, padding dengan 0 hingga 5 digit
# :% -> format sebagai persentase
print(f"Gaji: Rp {gaji:,.2f}")
print(f"Diskon: {0.15:.1%}") # 0.15 menjadi 15.0%

item = "Buku"
harga = 55000
print(f"Item: {item:<10} | Harga: Rp {harga:>10,}") # Rata kiri dan kanan
print(f"Item: {item:^10} | Harga: Rp {harga:^10,}") # Rata tengah

nomor_urut = 7
print(f"ID Pelanggan: {nomor_urut:04d}") # Output: 0007

# Debugging mudah dengan f-string (Python 3.8+)
# Menulis {variable=} akan mencetak nama variabel dan nilainya
print(f"Debugging: {nama=}, {umur=}") # Output: Debugging: nama='Citra', umur=22
```

F-string sangat fleksibel dan membuat pemformatan string menjadi jauh lebih intuitif di Python.

---

## 4. Struktur Kontrol Alur (Control Flow)

Struktur kontrol alur menentukan urutan eksekusi pernyataan dalam program Anda. Python menyediakan beberapa struktur kontrol alur utama: pernyataan kondisional (`if`/`elif`/`else`) untuk membuat keputusan, dan perulangan (`for`/`while`) untuk mengulangi blok kode.

### Pernyataan Kondisional (`if`, `elif`, `else`)

Memungkinkan program Anda menjalankan blok kode yang berbeda berdasarkan apakah suatu kondisi bernilai benar (`True`) atau salah (`False`).

*   **`if`:** Blok kode di bawah `if` hanya dijalankan jika `kondisi` setelah `if` bernilai `True`.
*   **`elif` (else if):** Memeriksa kondisi tambahan *hanya jika* kondisi `if` (atau `elif` sebelumnya) bernilai `False`. Bisa ada nol atau lebih `elif`. Urutan `elif` penting.
*   **`else`:** Blok kode di bawah `else` hanya dijalankan *jika* semua kondisi `if` dan `elif` sebelumnya bernilai `False`. Hanya bisa ada satu `else` di akhir (dan ini opsional).

**Sintaks Dasar:**

```python
if kondisi_1:
    # Blok kode jika kondisi_1 True
    # Harus diindentasi
    print("Eksekusi blok if")
elif kondisi_2:
    # Blok kode jika kondisi_1 False DAN kondisi_2 True
    print("Eksekusi blok elif pertama")
elif kondisi_3:
    # Blok kode jika kondisi_1 dan kondisi_2 False, DAN kondisi_3 True
    print("Eksekusi blok elif kedua")
# ... bisa ada elif lain ...
else:
    # Blok kode jika SEMUA kondisi di atas False
    print("Eksekusi blok else")

# Kode ini akan selalu dijalankan setelah blok if-elif-else selesai
print("Setelah struktur if-elif-else")
```

**Penting:**
*   Setiap `kondisi` adalah ekspresi yang dievaluasi menjadi `True` atau `False`.
*   Tanda titik dua (`:`) **wajib** ada di akhir setiap baris `if`, `elif`, dan `else`.
*   Blok kode di bawah setiap kondisi **harus diindentasi** secara konsisten (biasanya 4 spasi).

**Contoh Penilaian Nilai:**

```python
nilai_ujian = 78

if nilai_ujian >= 90:
    predikat = "A"
    print("Luar biasa!")
elif nilai_ujian >= 80: # Cek ini jika nilai < 90
    predikat = "B"
    print("Bagus!")
elif nilai_ujian >= 70: # Cek ini jika nilai < 80
    predikat = "C"
    print("Cukup.")
elif nilai_ujian >= 60: # Cek ini jika nilai < 70
    predikat = "D"
    print("Perlu belajar lagi.")
else: # Jika nilai < 60
    predikat = "E"
    print("Gagal.")

print(f"Nilai Anda: {nilai_ujian}, Predikat: {predikat}")
# Output:
# Cukup.
# Nilai Anda: 78, Predikat: C
```

**Contoh dengan Boolean dan Logika:**

```python
suhu = 15 # derajat Celcius
hujan = False

if suhu < 10:
    print("Sangat dingin, pakai jaket tebal!")
elif suhu < 20: # Antara 10 (inklusif) dan 20 (eksklusif)
    print("Sejuk, jaket tipis cukup.")
    if hujan: # Cek tambahan di dalam elif
        print("Dan jangan lupa bawa payung!")
elif suhu < 30: # Antara 20 (inklusif) dan 30 (eksklusif)
    print("Cuaca nyaman.")
else: # Suhu 30 atau lebih
    print("Panas! Cari tempat teduh.")

if not hujan:
    print("Hari ini tidak hujan.")
```

**"Truthiness" dan "Falsiness":**
Dalam konteks kondisional (`if`, `while`), Python menganggap nilai-nilai berikut sebagai `False` (Falsy):
*   Konstanta `False`
*   Konstanta `None`
*   Angka nol dari semua tipe numerik (`0`, `0.0`, `0j`)
*   Urutan (sequence) dan koleksi (collection) yang kosong: `""` (string kosong), `[]` (list kosong), `()` (tuple kosong), `{}` (dictionary kosong), `set()` (set kosong), `range(0)`
*   Objek dari kelas kustom yang memiliki metode `__bool__()` yang mengembalikan `False` atau `__len__()` yang mengembalikan `0`.

Semua nilai lain pada umumnya dianggap `True` (Truthy).

```python
nama = input("Masukkan nama (biarkan kosong jika anonim): ")

if nama: # Mengecek apakah string 'nama' tidak kosong (truthy)
    print(f"Halo, {nama}!")
else: # Jika string 'nama' kosong (falsy)
    print("Halo, Pengguna Anonim!")

data = []
if data: # Mengecek apakah list 'data' tidak kosong
    print("Memproses data...")
else:
    print("Tidak ada data untuk diproses.")
```

#### Logika Bersarang (Nested Conditions)

Anda dapat menempatkan pernyataan `if`/`elif`/`else` di dalam blok `if`/`elif`/`else` lainnya.

```python
umur = 25
warga_negara = "Indonesia"
punya_kartu_pemilih = True

if umur >= 17:
    print("Usia memenuhi syarat untuk memilih.")
    if warga_negara == "Indonesia":
        print("Kewarganegaraan memenuhi syarat.")
        if punya_kartu_pemilih:
            print("Anda boleh memilih!")
        else:
            print("Anda perlu mendaftar sebagai pemilih terlebih dahulu.")
            # Bisa ada if/elif/else lagi di sini
    else:
        print(f"Maaf, hanya WNI yang boleh memilih (Anda: {warga_negara}).")
else:
    print(f"Maaf, usia Anda ({umur}) belum cukup untuk memilih.")
```
**Perhatian:** Kondisi bersarang yang terlalu dalam (lebih dari 2-3 level) bisa membuat kode sulit dibaca dan dipelihara. Pertimbangkan untuk menyederhanakan logika atau menggunakan fungsi bantuan jika perlu.

#### Ekspresi Kondisional (Operator Ternary)

Python menyediakan cara ringkas untuk menulis pernyataan `if-else` sederhana dalam satu baris, terutama berguna untuk penugasan nilai berdasarkan kondisi.

**Sintaks:** `nilai_jika_true if kondisi else nilai_jika_false`

```python
umur = 16
status = "Dewasa" if umur >= 18 else "Remaja/Anak-anak"
print(f"Status berdasarkan usia {umur}: {status}") # Output: Remaja/Anak-anak

nilai = 85
keterangan_lulus = "Lulus" if nilai >= 70 else "Gagal"
print(f"Hasil ujian (Nilai: {nilai}): {keterangan_lulus}") # Output: Lulus

# Bisa juga digunakan dalam ekspresi lain
diskon = 0.1 if status == "Dewasa" else 0.05
print(f"Diskon yang berlaku: {diskon:.0%}") # Output: 5%
```
Gunakan operator ternary untuk ekspresi yang benar-benar sederhana agar mudah dibaca. Untuk logika yang lebih kompleks atau jika ada beberapa tindakan yang perlu dilakukan, `if-else` standar lebih disukai.

### Perulangan (`for` loop)

Perulangan `for` digunakan untuk melakukan **iterasi** (mengulangi serangkaian tindakan) pada **urutan (sequence)** atau objek **iterable** lainnya. Iterable adalah objek apa pun yang dapat mengembalikan elemennya satu per satu, seperti list, tuple, dictionary, set, string, file, dan objek `range`. Loop `for` akan mengeksekusi blok kode untuk setiap item dalam iterable tersebut.

**Sintaks Dasar:**

```python
for variabel_item in iterable:
    # Blok kode yang akan diulang untuk setiap item
    # Gunakan 'variabel_item' di dalam blok ini untuk mengakses item saat ini
    print(f"Memproses item: {variabel_item}")
    # ... lakukan sesuatu dengan item ...

# Kode ini dijalankan setelah loop selesai
print("Loop for selesai.")
```

*   `iterable`: Objek yang akan diiterasi (misalnya list, string, range).
*   `variabel_item`: Variabel yang akan otomatis menyimpan nilai item dari `iterable` pada setiap putaran (iterasi) loop. Anda bebas menamai variabel ini (misalnya `item`, `huruf`, `angka`, `kunci`).
*   Blok kode di bawah `for` **harus diindentasi**.

#### Iterasi Melalui Urutan (List, Tuple, String, dll)

```python
# Iterasi melalui List
buah = ["apel", "pisang", "mangga", "jeruk"]
print("Daftar Buah:")
for item_buah in buah:
    print(f"- {item_buah.capitalize()}")

# Iterasi melalui String
nama = "PYTHON"
print("\nKarakter dalam nama:")
for karakter in nama:
    print(karakter, end=" | ") # Output: P | Y | T | H | O | N |
print("\n") # Pindah baris setelah loop selesai

# Iterasi melalui Tuple
koordinat = (10, 20, 30)
print("Koordinat:")
for k in koordinat:
    print(f"  Nilai: {k}")

# Iterasi melalui Dictionary (defaultnya mengiterasi kunci/keys)
data_nilai = {"Andi": 85, "Budi": 90, "Citra": 78}
print("\nNama siswa (dari kunci dict):")
for nama_siswa in data_nilai: # Sama dengan 'for nama_siswa in data_nilai.keys():'
    print(f"- {nama_siswa}")

print("\nNilai siswa (dari values dict):")
for nilai_siswa in data_nilai.values():
    print(f"- {nilai_siswa}")

print("\nNama dan Nilai (dari items dict):")
for nama_siswa, nilai_siswa in data_nilai.items(): # .items() mengembalikan pasangan (key, value)
    print(f"- {nama_siswa}: {nilai_siswa}")
```

#### Fungsi `range()`

Fungsi `range()` sangat berguna untuk melakukan perulangan sejumlah kali tertentu atau menghasilkan urutan angka integer secara efisien. `range()` menghasilkan objek *iterable* (bukan list langsung, ini menghemat memori untuk range yang besar).

*   `range(stop)`: Menghasilkan angka dari 0 hingga `stop - 1`.
*   `range(start, stop)`: Menghasilkan angka dari `start` hingga `stop - 1`.
*   `range(start, stop, step)`: Menghasilkan angka dari `start` hingga `stop - 1`, dengan lompatan `step`. `step` bisa negatif untuk hitungan mundur.

```python
# Mencetak angka 0 sampai 4
print("Range(5):")
for i in range(5):
    print(i, end=" ") # Output: 0 1 2 3 4

# Mencetak angka 2 sampai 5
print("\nRange(2, 6):")
for i in range(2, 6):
    print(i, end=" ") # Output: 2 3 4 5

# Mencetak angka genap dari 10 sampai 18
print("\nRange(10, 20, 2):")
for i in range(10, 20, 2):
    print(i, end=" ") # Output: 10 12 14 16 18

# Menghitung mundur dari 5 ke 1
print("\nRange(5, 0, -1):")
for i in range(5, 0, -1):
    print(i, end=" ") # Output: 5 4 3 2 1
print()

# Menggunakan range untuk mengakses elemen list berdasarkan indeks
warna = ["merah", "kuning", "hijau", "biru"]
print("\nWarna berdasarkan indeks:")
for i in range(len(warna)): # len(warna) adalah 4, jadi range(4) -> 0, 1, 2, 3
    print(f"Indeks {i}: {warna[i]}")
```
Meskipun Anda *bisa* mengakses elemen list dengan `range(len(list))`, seringkali lebih Pythonic untuk mengiterasi langsung `for item in list` jika Anda tidak memerlukan indeksnya. Jika Anda memerlukan indeks *dan* item, gunakan `enumerate()`:

```python
print("\nWarna dengan enumerate:")
for indeks, nama_warna in enumerate(warna): # enumerate menghasilkan (indeks, item)
    print(f"Indeks {indeks}: {nama_warna}")
```

#### Perulangan Bersarang (Nested Loops)

Anda bisa menempatkan satu loop (`for` atau `while`) di dalam loop lainnya. Loop dalam akan menyelesaikan semua iterasinya untuk *setiap satu iterasi* dari loop luar.

```python
# Contoh: Mencetak kombinasi pasangan angka
print("Perulangan Bersarang (Kombinasi):")
for i in range(1, 4): # Loop luar (1, 2, 3)
    for j in ['a', 'b']: # Loop dalam ('a', 'b')
        print(f"({i}, {j})", end=" ")
# Output: (1, a) (1, b) (2, a) (2, b) (3, a) (3, b)
print()

# Contoh: Membuat papan catur sederhana (8x8)
print("\nPapan Catur:")
ukuran = 8
for baris in range(ukuran):
    for kolom in range(ukuran):
        # Cetak '#' jika jumlah baris+kolom genap, ' ' jika ganjil
        if (baris + kolom) % 2 == 0:
            print("#", end="")
        else:
            print(" ", end="")
    print() # Pindah baris setelah satu baris selesai
```
Hati-hati dengan perulangan bersarang yang terlalu banyak atau dengan iterable yang besar, karena kompleksitasnya bisa meningkat secara eksponensial (misal O(n*m) atau O(n^2)).

### Perulangan (`while` loop)

Perulangan `while` akan terus mengeksekusi blok kode **selama (while)** kondisi yang diberikan setelah kata kunci `while` bernilai `True`.

**Sintaks Dasar:**

```python
while kondisi:
    # Blok kode yang dijalankan selama kondisi True
    # Harus diindentasi
    print("Masih dalam loop while...")
    # PENTING: Pastikan ada sesuatu di dalam blok ini
    # yang pada akhirnya akan membuat 'kondisi' menjadi False,
    # atau gunakan pernyataan 'break' untuk keluar. Jika tidak,
    # Anda akan membuat loop tak terbatas (infinite loop).

# Kode ini dijalankan setelah kondisi menjadi False
print("Loop while selesai.")
```

*   `kondisi`: Ekspresi yang dievaluasi menjadi `True` atau `False` **sebelum** setiap iterasi.
*   Loop akan berhenti ketika `kondisi` pertama kali dievaluasi menjadi `False`.

**Contoh:**

```python
# Menghitung mundur dari 5
hitung_mundur = 5
print("Hitung Mundur:")
while hitung_mundur > 0:
    print(f"{hitung_mundur}...")
    hitung_mundur -= 1 # Penting! Kurangi nilai agar loop berhenti

print("Meluncur!")

# Contoh: Menunggu input spesifik dari pengguna
perintah = ""
print("\nKetik 'selesai' untuk berhenti.")
while perintah.lower() != "selesai":
    perintah = input("Masukkan perintah: ")
    if perintah.lower() != "selesai":
        print(f"Anda mengetik: '{perintah}'. Menunggu lagi...")

print("Program berhenti.")
```

#### Loop Tak Terbatas (Infinite Loop) dan Cara Menghentikannya

Jika kondisi dalam `while` loop tidak pernah menjadi `False` (dan tidak ada `break`), loop akan berjalan selamanya (atau sampai program dihentikan secara paksa, misalnya dengan menekan `Ctrl+C` di terminal).

```python
# Contoh infinite loop (HATI-HATI!)
# counter = 0
# while True: # Kondisi selalu True
#     print(f"Looping tak terbatas... ({counter})")
#     counter += 1
#     # Anda perlu menambahkan kondisi untuk keluar, misalnya:
#     if counter >= 10:
#         print("Mencapai batas, keluar dari loop.")
#         break # Keluar dari loop while
```

Infinite loop terkadang disengaja, misalnya dalam program yang perlu terus berjalan mendengarkan event (seperti server web atau GUI), tetapi harus selalu ada mekanisme (seperti `break` berdasarkan input atau kondisi tertentu) untuk menghentikannya secara terprogram jika diperlukan.

### Kontrol Perulangan (`break`, `continue`, `pass`)

Pernyataan ini digunakan untuk mengubah alur eksekusi normal di dalam loop (`for` atau `while`).

#### `break`: Menghentikan Loop

Pernyataan `break` akan segera **menghentikan** eksekusi loop **terdalam** tempat ia berada (baik `for` maupun `while`). Eksekusi program akan dilanjutkan ke pernyataan pertama *setelah* blok loop tersebut.

```python
# Mencari angka pertama yang habis dibagi 7 dalam list
angka = [12, 17, 23, 28, 31, 40, 49, 50]
angka_ditemukan = None # Untuk menyimpan hasil

print("\nMencari kelipatan 7:")
for num in angka:
    print(f"Memeriksa {num}...")
    if num % 7 == 0:
        print(f"Ditemukan! Angka kelipatan 7 pertama adalah {num}")
        angka_ditemukan = num
        break # Keluar dari loop for karena sudah ketemu
    # Kode di bawah break dalam iterasi ini tidak akan dijalankan jika break terjadi
    print(f"{num} bukan kelipatan 7.")

if angka_ditemukan is not None:
    print(f"Hasil akhir: {angka_ditemukan}")
else:
    print("Tidak ada kelipatan 7 yang ditemukan dalam list.")
```

#### `continue`: Melanjutkan ke Iterasi Berikutnya

Pernyataan `continue` akan segera **menghentikan iterasi saat ini** dan melompat ke **awal iterasi berikutnya** dari loop terdekat. Kode di bawah `continue` dalam iterasi saat ini akan dilewati.

```python
# Mencetak hanya angka ganjil dari 1 sampai 10
print("\nMencetak angka ganjil (1-10):")
for i in range(1, 11):
    if i % 2 == 0: # Jika angka genap...
        continue   # ...lewati sisa kode di iterasi ini, lanjut ke i berikutnya
    # Kode ini hanya dijalankan jika i ganjil (karena continue dilewati)
    print(i, end=" ") # Output: 1 3 5 7 9
print()

# Contoh dalam while: Memproses input, abaikan baris kosong
print("\nMasukkan teks (ketik 'stop' untuk berhenti):")
while True:
    baris = input("> ")
    if baris.lower() == 'stop':
        break # Keluar dari loop utama
    if not baris.strip(): # Jika baris kosong atau hanya whitespace
        print("(Melewati baris kosong)")
        continue # Lanjut ke input berikutnya
    # Proses baris yang tidak kosong
    print(f"Memproses: '{baris.upper()}'")
```

#### `pass`: Pernyataan Kosong (Placeholder)

Pernyataan `pass` adalah operasi null; secara harfiah tidak melakukan apa-apa ketika dieksekusi. Ini digunakan ketika sintaks Python memerlukan sebuah pernyataan (misalnya di dalam blok `if`, `for`, `def`, `class`), tetapi Anda belum ingin menulis logika apa pun atau memang tidak ada aksi yang perlu dilakukan pada kondisi tersebut.

```python
# Contoh penggunaan pass sebagai placeholder

def fungsi_yang_belum_diimplementasi():
    pass # TODO: Tambahkan logika nanti

class KelasMinimal:
    pass # Kerangka kelas paling dasar

angka = 10
if angka > 50:
    # Belum tahu mau diapakan jika angka > 50
    pass
else:
    print("Angka tidak lebih besar dari 50")

# Contoh dalam loop (agak dibuat-buat untuk ilustrasi)
for i in range(5):
    if i == 2:
        # Mungkin ada kondisi khusus untuk i=2 tapi belum butuh aksi
        pass
        print("(Melewati angka 2 tanpa aksi khusus)")
    else:
        print(f"Memproses angka: {i}")
```
`pass` sangat berguna sebagai *placeholder* selama proses pengembangan kode agar struktur sintaksis tetap valid.

### Klausa `else` pada Loop

Baik loop `for` maupun `while` di Python dapat memiliki klausa `else` opsional. Blok `else` ini unik karena akan dieksekusi **hanya jika loop selesai secara normal**, yaitu *tanpa* dihentikan oleh pernyataan `break`. Jika loop berhenti karena `break`, blok `else` akan **dilewati**.

Ini sangat berguna untuk skenario seperti pencarian, di mana Anda ingin melakukan sesuatu jika item yang dicari *tidak* ditemukan setelah memeriksa semua elemen (loop selesai tanpa `break`).

```python
# Contoh dengan for...else (mencari item)
cari_buah = "durian"
tas_buah = ["apel", "mangga", "jeruk", "pisang"]

print(f"\nMencari '{cari_buah}' di dalam tas...")
for buah in tas_buah:
    print(f"Memeriksa: {buah}")
    if buah == cari_buah:
        print(f"'{cari_buah}' ditemukan!")
        break # Keluar dari loop karena sudah ketemu
else:
    # Blok ini HANYA dijalankan jika loop for selesai TANPA break
    print(f"Maaf, '{cari_buah}' tidak ada di dalam tas.")

print("-" * 20)

cari_buah_2 = "mangga"
print(f"\nMencari '{cari_buah_2}' di dalam tas...")
for buah in tas_buah:
    print(f"Memeriksa: {buah}")
    if buah == cari_buah_2:
        print(f"'{cari_buah_2}' ditemukan!")
        break
else:
    # Blok ini TIDAK dijalankan karena ada break
    print(f"Maaf, '{cari_buah_2}' tidak ada di dalam tas.")


# Contoh dengan while...else (mencoba beberapa kali)
import random
percobaan = 0
batas_percobaan = 3
angka_rahasia = 7

print("\nMencoba menebak angka (maks 3 kali):")
while percobaan < batas_percobaan:
    percobaan += 1
    tebakan = random.randint(1, 10) # Angka acak 1-10
    print(f"Percobaan {percobaan}: Menebak {tebakan}")
    if tebakan == angka_rahasia:
        print("Tebakan benar!")
        break # Keluar dari loop while karena berhasil
else:
    # Blok ini HANYA dijalankan jika loop while selesai
    # karena kondisi (percobaan < batas_percobaan) menjadi False
    # (artinya semua percobaan gagal, tidak ada break)
    print(f"Gagal menebak angka {angka_rahasia} dalam {batas_percobaan} percobaan.")
```
Fitur `else` pada loop ini adalah salah satu keunikan Python yang bisa sangat berguna untuk membuat kode pencarian atau percobaan menjadi lebih bersih.

---

## 5. Struktur Data

Struktur data adalah cara fundamental untuk mengorganisir dan menyimpan data dalam program agar dapat diakses dan dimodifikasi secara efisien. Python menyediakan beberapa struktur data bawaan (built-in) yang sangat kuat dan fleksibel. Yang paling penting dan sering digunakan adalah:

*   **List:** Kumpulan item yang terurut dan dapat diubah (mutable).
*   **Tuple:** Kumpulan item yang terurut dan tidak dapat diubah (immutable).
*   **Set:** Kumpulan item unik yang tidak terurut (unordered).
*   **Dictionary:** Kumpulan pasangan kunci-nilai (key-value pairs).

Mari kita bahas masing-masing.

### List

List adalah salah satu struktur data paling serbaguna di Python. Karakteristiknya:
*   **Terurut (Ordered):** Item disimpan dalam urutan tertentu, dan urutan ini tidak berubah kecuali Anda mengubahnya.
*   **Dapat Diubah (Mutable):** Anda dapat menambah, menghapus, atau mengubah item dalam list setelah list dibuat.
*   **Memperbolehkan Duplikasi:** List bisa berisi item yang sama lebih dari satu kali.
*   **Heterogen:** List bisa berisi item dari tipe data yang berbeda (misalnya, integer, string, dan list lain dalam satu list).

List didefinisikan menggunakan kurung siku `[]` dengan elemen-elemen dipisahkan oleh koma.

#### Membuat List

```python
# List kosong
list_kosong = []
list_kosong_lain = list() # Menggunakan konstruktor (kurang umum untuk list kosong)

# List berisi integer
angka = [1, 5, 2, 8, 3, 5] # Boleh ada duplikat (angka 5)

# List berisi string
nama_hari = ["Senin", "Selasa", "Rabu", "Kamis", "Jumat", "Sabtu", "Minggu"]

# List campuran (heterogen)
campuran = [10, "Python", 3.14, True, None, ["a", "b"]] # Berisi list lain

print(f"List kosong: {list_kosong}")
print(f"List angka: {angka}")
print(f"List nama_hari: {nama_hari}")
print(f"List campuran: {campuran}")

# Membuat list dari iterable lain (misal string atau tuple)
list_dari_string = list("halo")
print(f"List dari 'halo': {list_dari_string}") # Output: ['h', 'a', 'l', 'o']
list_dari_tuple = list((1, 2, 3))
print(f"List dari tuple (1,2,3): {list_dari_tuple}") # Output: [1, 2, 3]
```

#### Mengakses Elemen (Indexing dan Slicing)

Sama seperti string, Anda dapat mengakses elemen list menggunakan **indeks** (mulai dari 0) dan mengambil sub-bagian menggunakan **slicing**.

```python
warna = ["merah", "kuning", "hijau", "biru", "ungu"]
# Indeks:   0        1         2       3       4
# Negatif: -5       -4        -3      -2      -1

# Indexing
print(f"Warna pertama (indeks 0): {warna[0]}")    # Output: merah
print(f"Warna ketiga (indeks 2): {warna[2]}")    # Output: hijau
print(f"Warna terakhir (indeks -1): {warna[-1]}")   # Output: ungu
# print(warna[5])  # Ini akan menghasilkan IndexError

# Slicing [start:stop:step]
print(f"Slice [1:4]: {warna[1:4]}")  # Output: ['kuning', 'hijau', 'biru'] (indeks 1 sampai sebelum 4)
print(f"Slice [:3]: {warna[:3]}")   # Output: ['merah', 'kuning', 'hijau'] (dari awal sampai sebelum 3)
print(f"Slice [2:]: {warna[2:]}")   # Output: ['hijau', 'biru', 'ungu'] (dari indeks 2 sampai akhir)
print(f"Slice [::2]: {warna[::2]}")  # Output: ['merah', 'hijau', 'ungu'] (setiap elemen ke-2)
print(f"Slice [::-1]: {warna[::-1]}") # Output: ['ungu', 'biru', 'hijau', 'kuning', 'merah'] (membalik list)

# Slicing menghasilkan list baru (salinan dangkal)
warna_slice = warna[1:3]
print(f"Slice asli: {warna_slice}")
warna_slice[0] = "JINGGA" # Mengubah slice
print(f"Slice diubah: {warna_slice}")
print(f"List warna asli (tidak berubah): {warna}") # List asli tidak terpengaruh
```

#### Memodifikasi List (Mutable)

Karena list bersifat *mutable*, Anda dapat mengubah isinya setelah list dibuat.

```python
angka = [10, 20, 30, 40, 50]
print(f"List angka awal: {angka}")

# 1. Mengubah elemen berdasarkan indeks
angka[1] = 25 # Ganti elemen di indeks 1
print(f"Setelah ubah indeks 1: {angka}") # Output: [10, 25, 30, 40, 50]

# 2. Mengubah beberapa elemen menggunakan slicing
angka[2:4] = [35, 45] # Ganti elemen di indeks 2 dan 3
print(f"Setelah ubah slice [2:4]: {angka}") # Output: [10, 25, 35, 45, 50]

# 3. Menggunakan slicing untuk menyisipkan/menghapus
#    (Jumlah elemen pengganti tidak harus sama dengan yang diganti)
angka[1:3] = [100, 200, 300] # Ganti 2 elemen (indeks 1, 2) dengan 3 elemen baru
print(f"Setelah ubah slice [1:3] dgn 3 elemen: {angka}") # Output: [10, 100, 200, 300, 45, 50]

angka[0:2] = [5] # Ganti 2 elemen (indeks 0, 1) dengan 1 elemen baru
print(f"Setelah ubah slice [0:2] dgn 1 elemen: {angka}") # Output: [5, 200, 300, 45, 50]

angka[1:1] = [6, 7, 8] # Sisipkan elemen di indeks 1 (tidak menghapus apa pun)
print(f"Setelah sisip di [1:1]: {angka}") # Output: [5, 6, 7, 8, 200, 300, 45, 50]

# 4. Menghapus elemen menggunakan slicing
angka[1:4] = [] # Hapus elemen dari indeks 1 sampai sebelum 4
print(f"Setelah hapus slice [1:4]: {angka}") # Output: [5, 200, 300, 45, 50]

# 5. Menghapus elemen menggunakan del
del angka[0] # Hapus elemen di indeks 0
print(f"Setelah del angka[0]: {angka}") # Output: [200, 300, 45, 50]
del angka[1:3] # Hapus slice
print(f"Setelah del angka[1:3]: {angka}") # Output: [200, 50]
```

#### Metode List (`append()`, `insert()`, `extend()`, `remove()`, `pop()`, `clear()`, `index()`, `count()`, `sort()`, `reverse()`)

List memiliki banyak metode bawaan untuk memanipulasinya. Metode ini dipanggil pada objek list menggunakan notasi titik (`.`). Sebagian besar metode ini memodifikasi list *secara langsung* (in-place), artinya list aslinya yang berubah, dan metode tersebut biasanya mengembalikan `None` (kecuali `pop()`, `index()`, `count()`, `copy()`).

*   `append(item)`: Menambahkan `item` tunggal ke **akhir** list. Modifikasi in-place.
*   `insert(index, item)`: Menyisipkan `item` pada `index` yang ditentukan. Elemen setelahnya akan bergeser ke kanan. Modifikasi in-place.
*   `extend(iterable)`: Menambahkan semua elemen dari `iterable` (seperti list lain, tuple, string) ke akhir list. Mirip dengan operator `+` pada list (`list1 + list2`), tapi `extend` memodifikasi list asli (in-place), sedangkan `+` membuat list baru.
*   `remove(item)`: Menghapus **kemunculan pertama** dari `item` dalam list. Menghasilkan `ValueError` jika item tidak ditemukan. Modifikasi in-place.
*   `pop(index=-1)`: Menghapus dan **mengembalikan** elemen pada `index` yang diberikan. Jika `index` tidak diberikan (atau `-1`), menghapus dan mengembalikan elemen **terakhir**. Menghasilkan `IndexError` jika indeks tidak valid atau list kosong. Modifikasi in-place.
*   `clear()`: Menghapus **semua** elemen dari list, menjadikannya list kosong. Modifikasi in-place.
*   `index(item, start=0, end=len(list))`: Mengembalikan **indeks** dari **kemunculan pertama** `item`. Bisa diberi `start` dan `end` opsional untuk mencari hanya dalam slice tersebut. Menghasilkan `ValueError` jika item tidak ditemukan. Tidak mengubah list.
*   `count(item)`: Mengembalikan **jumlah** berapa kali `item` muncul dalam list. Tidak mengubah list.
*   `sort(key=None, reverse=False)`: Mengurutkan elemen list **secara langsung (in-place)**. Secara default, mengurutkan secara menaik (ascending).
    *   `key`: Fungsi opsional yang akan dipanggil pada setiap elemen sebelum perbandingan (misal `key=str.lower` untuk mengurutkan string tanpa memperhatikan huruf besar/kecil, atau `key=len` untuk mengurutkan berdasarkan panjang).
    *   `reverse=True`: Mengurutkan secara menurun (descending).
    *   Agar `sort()` bekerja, elemen dalam list harus dapat dibandingkan satu sama lain (misal, semua angka, atau semua string). Mencampur tipe yang tidak bisa dibandingkan (seperti int dan string) akan error.
*   `reverse()`: Membalik urutan elemen list **secara langsung (in-place)**.
*   `copy()`: Mengembalikan *salinan dangkal (shallow copy)* dari list. List baru dibuat, tetapi jika list berisi objek mutable lain (seperti list lain), objek tersebut *tidak* disalin secara mendalam, hanya referensinya yang disalin.

```python
buah = ["pisang", "apel", "jeruk"]
print(f"List buah awal: {buah}")

# append()
buah.append("mangga")
print(f"Setelah append('mangga'): {buah}") # ['pisang', 'apel', 'jeruk', 'mangga']

# insert()
buah.insert(1, "anggur") # Sisipkan 'anggur' di indeks 1
print(f"Setelah insert(1, 'anggur'): {buah}") # ['pisang', 'anggur', 'apel', 'jeruk', 'mangga']

# extend()
buah_lain = ["nanas", "semangka"]
buah.extend(buah_lain)
print(f"Setelah extend(['nanas', 'semangka']): {buah}") # ['pisang', 'anggur', 'apel', 'jeruk', 'mangga', 'nanas', 'semangka']
# Bandingkan dengan +:
buah_baru = buah + ["kiwi"] # Membuat list baru, buah tidak berubah
print(f"Buah baru (+ kiwi): {buah_baru}")
print(f"Buah asli setelah +: {buah}") # Tetap sama

# remove()
buah.remove("apel") # Hapus 'apel' pertama
print(f"Setelah remove('apel'): {buah}") # ['pisang', 'anggur', 'jeruk', 'mangga', 'nanas', 'semangka']
# buah.remove("durian") # Akan menghasilkan ValueError

# pop()
elemen_terakhir = buah.pop() # Hapus & ambil elemen terakhir ('semangka')
print(f"Elemen terakhir yg di-pop: {elemen_terakhir}")
print(f"List setelah pop(): {buah}") # ['pisang', 'anggur', 'jeruk', 'mangga', 'nanas']

elemen_indeks_0 = buah.pop(0) # Hapus & ambil elemen indeks 0 ('pisang')
print(f"Elemen indeks 0 yg di-pop: {elemen_indeks_0}")
print(f"List setelah pop(0): {buah}") # ['anggur', 'jeruk', 'mangga', 'nanas']

# index()
indeks_jeruk = buah.index("jeruk")
print(f"Indeks 'jeruk': {indeks_jeruk}") # Output: 1
# indeks_apel = buah.index("apel") # Akan ValueError karena 'apel' sudah dihapus

# count()
angka_lagi = [1, 2, 5, 2, 3, 2, 4, 2]
jumlah_angka_2 = angka_lagi.count(2)
print(f"Jumlah angka 2 dalam {angka_lagi}: {jumlah_angka_2}") # Output: 4

# sort()
angka_acak = [50, 10, 40, 20, 30, 10]
print(f"\nAngka acak sebelum sort: {angka_acak}")
angka_acak.sort() # Mengurutkan naik (in-place)
print(f"Angka acak setelah sort(): {angka_acak}") # [10, 10, 20, 30, 40, 50]

angka_acak.sort(reverse=True) # Mengurutkan turun
print(f"Angka acak setelah sort(reverse=True): {angka_acak}") # [50, 40, 30, 20, 10, 10]

kata = ["apel", "Jeruk", "pisang", "Anggur"]
print(f"\nKata sebelum sort: {kata}")
kata.sort() # Default sort case-sensitive (Kapital duluan)
print(f"Kata setelah sort default: {kata}") # ['Anggur', 'Jeruk', 'apel', 'pisang']

kata.sort(key=str.lower) # Sort case-insensitive
print(f"Kata setelah sort(key=str.lower): {kata}") # ['Anggur', 'apel', 'Jeruk', 'pisang']

# Sort berdasarkan panjang string
kata.sort(key=len)
print(f"Kata setelah sort(key=len): {kata}") # ['apel', 'Jeruk', 'pisang', 'Anggur']

# reverse()
angka_urut = [1, 2, 3, 4, 5]
print(f"\nAngka urut sebelum reverse: {angka_urut}")
angka_urut.reverse() # Membalik urutan (in-place)
print(f"Angka urut setelah reverse(): {angka_urut}") # [5, 4, 3, 2, 1]

# copy()
list_asli = [1, 2, [10, 20]] # List berisi list lain
list_salinan = list_asli.copy()
list_referensi = list_asli # Ini BUKAN salinan, hanya nama lain untuk list yg sama

print(f"\nList Asli: {list_asli}")
print(f"List Salinan: {list_salinan}")
print(f"List Referensi: {list_referensi}")

# Modifikasi salinan (tidak mempengaruhi asli)
list_salinan.append(4)
list_salinan[0] = 100
print(f"\nList Asli setelah modif salinan: {list_asli}") # [1, 2, [10, 20]]
print(f"List Salinan setelah modif salinan: {list_salinan}") # [100, 2, [10, 20], 4]

# Modifikasi referensi (mempengaruhi asli)
list_referensi.append(5)
print(f"\nList Asli setelah modif referensi: {list_asli}") # [1, 2, [10, 20], 5]
print(f"List Referensi setelah modif referensi: {list_referensi}") # Sama dengan list_asli

# Perhatian: copy() adalah shallow copy
list_salinan[2][0] = 99 # Mengubah elemen *di dalam* list bersarang pada salinan
print(f"\nList Asli setelah modif list bersarang di salinan: {list_asli}") # [1, 2, [99, 20], 5] (IKUT BERUBAH!)
print(f"List Salinan setelah modif list bersarang di salinan: {list_salinan}") # [100, 2, [99, 20], 4]
# Untuk salinan independen penuh (deep copy), gunakan modul 'copy': import copy; list_deep = copy.deepcopy(list_asli)

# clear()
list_salinan.clear()
print(f"\nList salinan setelah clear(): {list_salinan}") # Output: []
```

#### List Comprehensions (Cara Cepat Membuat List)

Cara yang sangat Pythonic, ringkas, dan seringkali lebih efisien untuk membuat list baru berdasarkan iterable yang sudah ada. Sintaksnya menggabungkan loop `for` dan (opsional) `if` di dalam kurung siku `[]`.

**Sintaks:** `[ekspresi for item in iterable if kondisi]`

*   `ekspresi`: Operasi yang dilakukan pada setiap `item` untuk menghasilkan elemen list baru.
*   `for item in iterable`: Loop standar untuk iterasi.
*   `if kondisi` (opsional): Filter; hanya `item` yang memenuhi `kondisi` yang akan diproses oleh `ekspresi`.

```python
# Contoh 1: Membuat list kuadrat dari 0 sampai 9
# Cara lama dengan loop for
kuadrat_lama = []
for x in range(10):
    kuadrat_lama.append(x**2)

# Cara dengan list comprehension
kuadrat_comp = [x**2 for x in range(10)]

print(f"Kuadrat (cara lama): {kuadrat_lama}")
print(f"Kuadrat (comprehension): {kuadrat_comp}")
# Output keduanya: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

# Contoh 2: Membuat list huruf kapital dari sebuah string
kata = "Python"
huruf_kapital = [karakter.upper() + "!" for karakter in kata]
print(f"Huruf kapital dengan '!': {huruf_kapital}") # Output: ['P!', 'Y!', 'T!', 'H!', 'O!', 'N!']

# Contoh 3: Membuat list angka genap dari list lain (filter)
angka = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
angka_genap = [n for n in angka if n % 2 == 0]
print(f"Angka genap dari {angka}: {angka_genap}") # Output: [2, 4, 6, 8, 10]

# Contoh 4: Menggabungkan ekspresi dan kondisi
# Ambil kuadrat dari angka ganjil antara 0-9
kuadrat_ganjil = [x**2 for x in range(10) if x % 2 != 0]
print(f"Kuadrat ganjil (0-9): {kuadrat_ganjil}") # Output: [1, 9, 25, 49, 81]

# Contoh 5: List comprehension bersarang (membuat list flat dari list of lists)
matriks = [[1, 2, 3], [4, 5], [6, 7, 8, 9]]
flat_list = [elemen for baris in matriks for elemen in baris]
print(f"Flat list dari {matriks}: {flat_list}") # Output: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```
List comprehension seringkali lebih disukai daripada loop `for` dengan `append()` untuk membuat list karena lebih ringkas dan terkadang lebih cepat. Namun, jika logikanya sangat kompleks, loop `for` biasa mungkin lebih mudah dibaca.

#### List Bersarang (Nested Lists)

List dapat berisi list lain sebagai elemennya. Ini memungkinkan pembuatan struktur data multi-dimensi seperti matriks atau tabel.

```python
matriks_3x3 = [
    [1, 2, 3],  # Baris 0
    [4, 5, 6],  # Baris 1
    [7, 8, 9]   # Baris 2
]

print(f"Matriks: {matriks_3x3}")

# Mengakses elemen: matriks[indeks_baris][indeks_kolom]
print(f"Elemen baris 1, kolom 2: {matriks_3x3[0][1]}") # Output: 2 (ingat indeks mulai dari 0)
print(f"Elemen baris 3, kolom 1: {matriks_3x3[2][0]}") # Output: 7
print(f"Baris kedua (indeks 1): {matriks_3x3[1]}")   # Output: [4, 5, 6]

# Mengubah elemen dalam list bersarang
matriks_3x3[1][1] = 99
print(f"Matriks setelah diubah [1][1]: {matriks_3x3}")
# Output: [[1, 2, 3], [4, 99, 6], [7, 8, 9]]

# Iterasi melalui list bersarang
print("\nElemen matriks satu per satu:")
for baris in matriks_3x3:
    print(f"  Memproses baris: {baris}")
    for elemen in baris:
        print(f"    Elemen: {elemen}")
```

### Tuple

Tuple mirip dengan list, namun dengan satu perbedaan kunci: tuple bersifat **tidak dapat diubah (immutable)** setelah dibuat. Karakteristiknya:
*   **Terurut (Ordered):** Item disimpan dalam urutan tertentu.
*   **Tidak Dapat Diubah (Immutable):** Anda *tidak bisa* menambah, menghapus, atau mengubah item dalam tuple setelah tuple dibuat.
*   **Memperbolehkan Duplikasi:** Tuple bisa berisi item yang sama lebih dari satu kali.
*   **Heterogen:** Tuple bisa berisi item dari tipe data yang berbeda.

Tuple didefinisikan menggunakan kurung biasa `()` dengan elemen-elemen dipisahkan oleh koma. Kurung `()` terkadang opsional jika konteksnya jelas.

#### Membuat Tuple

```python
# Tuple kosong
tuple_kosong = ()
tuple_kosong_lain = tuple() # Konstruktor

# Tuple berisi integer
angka_tuple = (1, 5, 2, 8, 3, 5) # Boleh duplikat

# Tuple berisi string
nama_bulan = ("Januari", "Februari", "Maret")

# Tuple campuran
campuran_tuple = (20, "Java", 2.71, False, [10, 20]) # Boleh berisi objek mutable

# Tuple dengan satu elemen (PERHATIKAN KOMA di akhir!)
tuple_satu_elemen = (10,) # Koma wajib untuk membedakan dari ekspresi biasa
bukan_tuple = (10)       # Ini adalah integer 10 yang dikurung

print(tuple_kosong)        # Output: ()
print(angka_tuple)         # Output: (1, 5, 2, 8, 3, 5)
print(campuran_tuple)      # Output: (20, 'Java', 2.71, False, [10, 20])
print(f"Tuple satu elemen: {tuple_satu_elemen}, tipe: {type(tuple_satu_elemen)}") # Output: (10,), <class 'tuple'>
print(f"Bukan tuple: {bukan_tuple}, tipe: {type(bukan_tuple)}")       # Output: 10, <class 'int'>

# Kurung () terkadang opsional saat mendefinisikan tuple (packing)
koordinat = 10, 20, 30 # Python otomatis membuat tuple
print(f"Koordinat (tanpa kurung): {koordinat}, tipe: {type(koordinat)}") # Output: (10, 20, 30), <class 'tuple'>

# Membuat tuple dari iterable lain
tuple_dari_list = tuple([1, 2, 2, 3])
print(f"Tuple dari list [1,2,2,3]: {tuple_dari_list}") # Output: (1, 2, 2, 3)
tuple_dari_string = tuple("abc")
print(f"Tuple dari string 'abc': {tuple_dari_string}") # Output: ('a', 'b', 'c')
```

#### Mengakses Elemen (Immutable)

Anda bisa mengakses elemen tuple menggunakan indexing dan slicing, sama seperti list. Namun, Anda **tidak bisa** mengubah, menambah, atau menghapus elemen tuple setelah dibuat.

```python
data_tuple = ('a', 'b', 'c', 'd', 'e')

print(f"Elemen ke-0: {data_tuple[0]}")    # Output: a
print(f"Elemen terakhir: {data_tuple[-1]}")   # Output: e
print(f"Slice [1:3]: {data_tuple[1:3]}")  # Output: ('b', 'c')

# Mencoba mengubah elemen akan menghasilkan TypeError
# data_tuple[0] = 'x' # TypeError: 'tuple' object does not support item assignment

# Metode seperti append, insert, remove, pop, sort TIDAK ADA untuk tuple
# del data_tuple[0]    # TypeError: 'tuple' object doesn't support item deletion
```

**Penting:** Meskipun tuple itu sendiri *immutable*, jika tuple berisi objek *mutable* (seperti list), objek di dalamnya *masih bisa* diubah. Tuple hanya menjamin referensi ke objek tersebut tidak berubah.

```python
tuple_dengan_list = (1, 2, [30, 40])
print(f"Tuple awal: {tuple_dengan_list}")

# Mengubah elemen di dalam list yang ada di tuple (INI BOLEH)
tuple_dengan_list[2][0] = 99
tuple_dengan_list[2].append(50)
print(f"Tuple setelah modifikasi list di dalamnya: {tuple_dengan_list}")
# Output: (1, 2, [99, 40, 50])

# Tapi Anda tetap tidak bisa mengganti list itu sendiri dengan list baru
# tuple_dengan_list[2] = ["x", "y"] # TypeError
```

#### Kapan Menggunakan Tuple?

Tuple digunakan ketika Anda memiliki kumpulan data yang **urutannya penting** dan Anda ingin **memastikan data tersebut tidak berubah** setelah dibuat. Kasus penggunaan umum:

1.  **Integritas Data:** Untuk data yang seharusnya konstan, seperti koordinat RGB (misal `(255, 0, 0)` untuk merah), data record yang tidak boleh diubah.
2.  **Kunci Dictionary:** Karena *immutable*, tuple (yang hanya berisi elemen *immutable* lainnya seperti string, angka, tuple lain) bisa digunakan sebagai kunci dalam dictionary, sedangkan list tidak bisa (karena list mutable).
    ```python
    lokasi = {}
    koordinat_jkt = ( -6.2088, 106.8456 )
    koordinat_bdg = ( -6.9175, 107.6191 )
    lokasi[koordinat_jkt] = "Jakarta"
    lokasi[koordinat_bdg] = "Bandung"
    # lokasi[[1, 2]] = "Tidak bisa" # TypeError: unhashable type: 'list'
    print(f"Lokasi: {lokasi}")
    print(f"Nama lokasi untuk {koordinat_jkt}: {lokasi[koordinat_jkt]}")
    ```
3.  **Pengembalian Fungsi:** Fungsi seringkali mengembalikan beberapa nilai, dan Python secara otomatis membungkusnya dalam sebuah tuple.
    ```python
    def bagi_dan_sisa(a, b):
        hasil_bagi = a // b
        sisa_bagi = a % b
        return hasil_bagi, sisa_bagi # Otomatis jadi tuple (hasil_bagi, sisa_bagi)

    h, s = bagi_dan_sisa(17, 5)
    print(f"17 dibagi 5: hasil {h}, sisa {s}") # Output: hasil 3, sisa 2
    ```
4.  **Format String:** Tuple sering digunakan dalam format string gaya lama (`%`) (meskipun f-string lebih disarankan sekarang). `print("Nama: %s, Usia: %d" % ("Ali", 25))`
5.  **Sedikit Lebih Cepat & Hemat Memori:** Karena sifatnya yang *immutable*, tuple umumnya sedikit lebih cepat untuk diiterasi dan membutuhkan sedikit lebih sedikit memori daripada list dengan elemen yang sama. Namun, perbedaan ini biasanya tidak signifikan kecuali dalam skala yang sangat besar atau dalam kode yang sangat kritis performa.
6.  **Struktur Data Tetap:** Menunjukkan kepada pembaca kode bahwa kumpulan data ini dimaksudkan untuk tidak berubah.

#### Tuple Unpacking

Fitur yang sangat berguna di Python yang memungkinkan Anda menugaskan elemen-elemen dalam tuple (atau list, atau iterable lain) ke beberapa variabel secara langsung dalam satu baris. Jumlah variabel di sebelah kiri harus sesuai dengan jumlah elemen dalam iterable (kecuali menggunakan `*`).

```python
# Unpacking dasar
data_pelanggan = ("Budi", 30, "budi@email.com")
nama, usia, email = data_pelanggan # Jumlah variabel = jumlah elemen tuple

print(f"Nama: {nama}")
print(f"Usia: {usia}")
print(f"Email: {email}")

# Unpacking dalam loop for (untuk iterable berisi iterable)
pasangan = [(1, 'a'), (2, 'b'), (3, 'c')]
print("\nUnpacking dalam loop:")
for angka, huruf in pasangan:
    print(f"Angka: {angka}, Huruf: {huruf}")

# Unpacking untuk menukar variabel (cara Pythonic tanpa variabel sementara)
a = 10
b = 20
print(f"\nSebelum tukar: a={a}, b={b}")
a, b = b, a # Buat tuple (b, a) lalu unpack ke a dan b
print(f"Setelah tukar: a={a}, b={b}") # Output: a=20, b=10

# Extended Unpacking (Python 3.x) - Menggunakan '*'
# '*' akan menangkap sisa elemen sebagai sebuah list
angka_banyak = (1, 2, 3, 4, 5, 6, 7)
pertama, kedua, *tengah, terakhir = angka_banyak

print(f"\nExtended Unpacking:")
print(f"Pertama: {pertama}")     # Output: 1
print(f"Kedua: {kedua}")       # Output: 2
print(f"Tengah: {tengah}")     # Output: [3, 4, 5, 6] (selalu list, bisa kosong)
print(f"Terakhir: {terakhir}")   # Output: 7

# '*' bisa di posisi lain
*awal, kedua_akhir, akhir = angka_banyak
print(f"Awal: {awal}") # Output: [1, 2, 3, 4, 5]
print(f"Kedua Akhir: {kedua_akhir}") # Output: 6
print(f"Akhir: {akhir}") # Output: 7

# Mengabaikan nilai yang tidak diperlukan dengan underscore (_)
# _ adalah konvensi untuk variabel yang nilainya tidak akan digunakan
data_lengkap = ("Citra", 25, "Jakarta", "0812345")
nama_saja, _, kota_saja, _ = data_lengkap
print(f"\nNama: {nama_saja}, Kota: {kota_saja}")
```

Tuple hanya memiliki dua metode utama (karena immutable):
*   `count(item)`: Menghitung berapa kali `item` muncul dalam tuple.
*   `index(item)`: Mencari indeks pertama kali `item` muncul dalam tuple (error jika tidak ada).

### Set

Set adalah kumpulan item yang **tidak terurut (unordered)** dan **tidak mengizinkan duplikasi elemen (setiap elemen unik)**. Karakteristiknya:
*   **Tidak Terurut (Unordered):** Elemen dalam set tidak memiliki posisi atau indeks tertentu. Urutan saat Anda mencetak set bisa berubah-ubah dan tidak bisa diandalkan. Anda tidak bisa mengakses elemen menggunakan `set[0]`.
*   **Unik:** Setiap elemen dalam set harus unik. Jika Anda mencoba menambahkan elemen yang sudah ada, set tidak akan berubah.
*   **Mutable:** Anda dapat menambah atau menghapus elemen dari set setelah set dibuat (meskipun elemen di dalamnya harus immutable agar bisa dimasukkan ke set).
*   **Heterogen (Elemen Harus Immutable):** Set bisa berisi campuran tipe data, **TAPI** elemen-elemen itu sendiri harus *immutable* (seperti angka, string, tuple). Anda tidak bisa memasukkan list atau dictionary ke dalam set.

Set sangat efisien untuk:
*   Mengecek keanggotaan (`item in my_set`) - sangat cepat (rata-rata O(1)).
*   Menghilangkan duplikasi dari urutan lain.
*   Melakukan operasi matematika himpunan (union, intersection, difference).

Set didefinisikan menggunakan kurung kurawal `{}` atau fungsi `set()`.

**Perhatian:** Untuk membuat set *kosong*, Anda **harus** menggunakan `set()`, karena `{}` akan membuat *dictionary* kosong.

#### Membuat Set

```python
# Set kosong (WAJIB pakai set())
set_kosong = set()
print(f"Set kosong: {set_kosong}, tipe: {type(set_kosong)}") # Output: set(), <class 'set'>

# Membuat set dengan elemen
angka_set = {1, 2, 3, 4, 5, 5, 4, 2} # Duplikasi (5, 4, 2) akan otomatis diabaikan
print(f"Set angka: {angka_set}") # Output: {1, 2, 3, 4, 5} (urutan bisa berbeda!)

huruf_set = {'a', 'b', 'c'}
print(f"Set huruf: {huruf_set}")

# Membuat set dari iterable lain (menghilangkan duplikat)
list_duplikat = [1, 1, 2, 3, 3, 3, 4, 5, 5]
set_dari_list = set(list_duplikat)
print(f"Set dari list {list_duplikat}: {set_dari_list}") # Output: {1, 2, 3, 4, 5}

set_dari_string = set("programming") # Membuat set dari karakter unik string
print(f"Set dari 'programming': {set_dari_string}") # Output: {'r', 'o', 'g', 'a', 'm', 'i', 'p', 'n'} (urutan acak)

# Set dengan tipe campuran (elemen harus immutable)
campuran_set = {1, "hello", 3.14, True, ("a", 1)} # Tuple boleh karena immutable
# campuran_error = {1, [2, 3]} # TypeError: unhashable type: 'list'
print(f"Set campuran: {campuran_set}")
```

#### Karakteristik (Tidak Terurut, Unik)

*   **Tidak Terurut:** Anda tidak bisa mengandalkan urutan elemen.
    ```python
    print(f"Set angka lagi: {angka_set}") # Urutannya mungkin berbeda dari sebelumnya
    # print(angka_set[0]) # TypeError: 'set' object is not subscriptable
    ```
*   **Unik:** Menambahkan elemen yang sudah ada tidak berpengaruh.
    ```python
    angka_set.add(3) # Mencoba menambahkan 3 lagi
    angka_set.add(6) # Menambahkan 6 (baru)
    print(f"Set angka setelah add(3) dan add(6): {angka_set}") # Output: {1, 2, 3, 4, 5, 6}
    ```
*   **Tes Keanggotaan Cepat:** `in` dan `not in` sangat efisien pada set.
    ```python
    print(f"Apakah 4 ada di set? {4 in angka_set}") # Output: True
    print(f"Apakah 10 ada di set? {10 in angka_set}") # Output: False
    ```

#### Operasi Set (Union, Intersection, Difference, Symmetric Difference)

Ini adalah kekuatan utama dari set, meniru operasi himpunan matematika.

*   **Union (`|` atau `.union()`):** Menggabungkan semua elemen unik dari dua set atau lebih. Hasilnya adalah set baru.
*   **Intersection (`&` atau `.intersection()`):** Menghasilkan set baru yang berisi elemen yang ada di *semua* set yang dioperasikan.
*   **Difference (`-` atau `.difference()`):** Menghasilkan set baru yang berisi elemen yang ada di set pertama tetapi *tidak* ada di set kedua (dan set-set berikutnya jika ada). Urutan penting.
*   **Symmetric Difference (`^` atau `.symmetric_difference()`):** Menghasilkan set baru yang berisi elemen yang ada di *salah satu* set, tetapi *tidak* di keduanya.

```python
set_A = {1, 2, 3, 4, 5}
set_B = {4, 5, 6, 7, 8}
set_C = {1, 10}

print(f"Set A: {set_A}")
print(f"Set B: {set_B}")
print(f"Set C: {set_C}")

# Union (Gabungan Unik)
union_AB = set_A | set_B
# atau union_AB = set_A.union(set_B)
print(f"Union A | B: {union_AB}") # Output: {1, 2, 3, 4, 5, 6, 7, 8}

# Intersection (Irisan)
intersect_AB = set_A & set_B
# atau intersect_AB = set_A.intersection(set_B)
print(f"Intersection A & B: {intersect_AB}") # Output: {4, 5}

intersect_AC = set_A.intersection(set_C)
print(f"Intersection A & C: {intersect_AC}") # Output: {1}

intersect_BC = set_B & set_C
print(f"Intersection B & C: {intersect_BC}") # Output: set() (kosong)

# Difference (Selisih)
diff_A_B = set_A - set_B # Elemen di A tapi tidak di B
# atau diff_A_B = set_A.difference(set_B)
print(f"Difference A - B: {diff_A_B}") # Output: {1, 2, 3}

diff_B_A = set_B - set_A # Elemen di B tapi tidak di A
print(f"Difference B - A: {diff_B_A}") # Output: {8, 6, 7}

# Symmetric Difference (Elemen unik di salah satu, tapi tidak di keduanya)
sym_diff_AB = set_A ^ set_B # (A U B) - (A n B)
# atau sym_diff_AB = set_A.symmetric_difference(set_B)
print(f"Symmetric Difference A ^ B: {sym_diff_AB}") # Output: {1, 2, 3, 6, 7, 8}

# Operasi bisa melibatkan lebih dari 2 set (untuk union, intersection)
union_ABC = set_A.union(set_B, set_C)
print(f"Union A, B, C: {union_ABC}") # {1, 2, 3, 4, 5, 6, 7, 8, 10}

intersect_AB_A = set_A.intersection(set_B, set_A) # Intersection A, B, dan A lagi
print(f"Intersection A, B, A: {intersect_AB_A}") # {4, 5}
```

Selain operasi yang menghasilkan set baru, ada juga metode *update* yang memodifikasi set asli secara in-place:
*   `update(other)` atau `|=`: Tambahkan semua elemen dari `other` ke set ini.
*   `intersection_update(other)` atau `&=`: Simpan hanya elemen yang juga ada di `other`.
*   `difference_update(other)` atau `-=`: Hapus elemen yang ada di `other` dari set ini.
*   `symmetric_difference_update(other)` atau `^=`: Simpan elemen yang ada di salah satu set tapi tidak di keduanya.

```python
set_D = {10, 20, 30}
set_E = {30, 40, 50}
print(f"\nSet D awal: {set_D}")
set_D.symmetric_difference_update(set_E) # D ^= E
print(f"Set D setelah symm_diff_update(E): {set_D}") # Output: {10, 20, 40, 50}
```

Set juga memiliki metode perbandingan himpunan:
*   `isdisjoint(other)`: `True` jika tidak ada elemen yang sama antara kedua set (irisannya kosong).
*   `issubset(other)` atau `<=`: `True` jika semua elemen set ini ada di `other`. `set_A <= set_B`
*   `issuperset(other)` atau `>=`: `True` jika set ini mengandung semua elemen `other`. `set_A >= set_B`
*   `<`: Proper subset (subset, tapi tidak sama).
*   `>`: Proper superset (superset, tapi tidak sama).

```python
set_X = {1, 2}
set_Y = {1, 2, 3}
set_Z = {4, 5}

print(f"\nSet X: {set_X}, Set Y: {set_Y}, Set Z: {set_Z}")
print(f"X isdisjoint Z? {set_X.isdisjoint(set_Z)}") # True
print(f"X isdisjoint Y? {set_X.isdisjoint(set_Y)}") # False

print(f"X issubset Y? {set_X.issubset(set_Y)}") # True
print(f"X <= Y? {set_X <= set_Y}")           # True
print(f"Y <= X? {set_Y <= set_X}")           # False
print(f"X < Y? {set_X < set_Y}")            # True (proper subset)
print(f"Y < Y? {set_Y < set_Y}")            # False

print(f"Y issuperset X? {set_Y.issuperset(set_X)}") # True
print(f"Y >= X? {set_Y >= set_X}")           # True
print(f"X >= Y? {set_X >= set_Y}")           # False
print(f"Y > X? {set_Y > set_X}")            # True (proper superset)
```

#### Metode Set (`add()`, `update()`, `remove()`, `discard()`, `pop()`, `clear()`)

Metode untuk memodifikasi isi set (selain operasi himpunan update).

*   `add(item)`: Menambahkan `item` ke set. Jika item sudah ada, tidak melakukan apa-apa. Modifikasi in-place.
*   `update(iterable)`: Menambahkan semua elemen dari `iterable` ke set. Sama dengan operator `|=`. Modifikasi in-place.
*   `remove(item)`: Menghapus `item` dari set. Menghasilkan **`KeyError`** jika item tidak ditemukan. Modifikasi in-place.
*   `discard(item)`: Menghapus `item` dari set. **Tidak** menghasilkan error jika item tidak ditemukan (lebih aman jika Anda tidak yakin itemnya ada). Modifikasi in-place.
*   `pop()`: Menghapus dan mengembalikan **sebuah elemen sembarang (arbitrary)** dari set. Karena set tidak terurut, Anda tidak bisa memprediksi elemen mana yang akan dihapus. Menghasilkan `KeyError` jika set kosong. Modifikasi in-place.
*   `clear()`: Menghapus semua elemen dari set. Modifikasi in-place.
*   `copy()`: Mengembalikan salinan dangkal (shallow copy) dari set.

```python
my_set = {10, 20}
print(f"\nSet awal: {my_set}")

# add()
my_set.add(30)
my_set.add(10) # Tidak ada efek karena 10 sudah ada
print(f"Setelah add(30) dan add(10): {my_set}") # {10, 20, 30} (urutan bisa beda)

# update()
my_set.update([30, 40, 50], {50, 60}, "hi") # Bisa dari berbagai iterable
print(f"Setelah update(...): {my_set}") # {10, 20, 30, 40, 50, 60, 'h', 'i'}

# remove()
my_set.remove(20)
print(f"Setelah remove(20): {my_set}")
# my_set.remove(99) # Akan menghasilkan KeyError

# discard()
my_set.discard(40)
my_set.discard(99) # Tidak error meskipun 99 tidak ada
print(f"Setelah discard(40) dan discard(99): {my_set}")

# pop()
try:
    elemen_sembarang = my_set.pop()
    print(f"Elemen yang di-pop (sembarang): {elemen_sembarang}")
    print(f"Set setelah pop: {my_set}")
    elemen_sembarang_lagi = my_set.pop()
    print(f"Elemen pop lagi: {elemen_sembarang_lagi}")
    print(f"Set setelah pop lagi: {my_set}")
except KeyError:
    print("Set sudah kosong, tidak bisa pop.")

# clear()
my_set.clear()
print(f"Set setelah clear: {my_set}") # Output: set()
# my_set.pop() # Sekarang akan KeyError
```

#### Kapan Menggunakan Set?

1.  **Menghilangkan Duplikat:** Cara paling mudah dan efisien untuk mendapatkan elemen unik dari list atau iterable lain. `list_unik = list(set(list_dengan_duplikat))`
2.  **Tes Keanggotaan Cepat:** Jika Anda perlu sering memeriksa apakah suatu item ada dalam kumpulan data besar, set jauh lebih cepat daripada list (`item in my_set` vs `item in my_list`).
3.  **Operasi Himpunan:** Ketika Anda perlu melakukan operasi matematika himpunan seperti union, intersection, difference, dll.

### Dictionary

Dictionary (dict) adalah struktur data yang menyimpan data sebagai pasangan **kunci-nilai (key-value pairs)**. Karakteristiknya:
*   **Mutable:** Anda dapat menambah, mengubah, atau menghapus pasangan kunci-nilai setelah dictionary dibuat.
*   **Tidak Terurut (Ordered di Python 3.7+):**
    *   Sebelum Python 3.7, dictionary dianggap tidak terurut. Anda tidak bisa mengandalkan urutan item.
    *   **Sejak Python 3.7**, dictionary **menjamin** urutan item sesuai dengan **urutan penyisipan (insertion order)**. Ini adalah perilaku standar CPython dan menjadi bagian dari spesifikasi bahasa sejak Python 3.7.
*   **Kunci Harus Unik dan Immutable:** Setiap kunci dalam dictionary harus unik. Kunci juga harus bertipe data *immutable* (seperti string, angka, tuple yang hanya berisi immutable). Anda tidak bisa menggunakan list sebagai kunci.
*   **Nilai Boleh Apa Saja:** Nilai (value) yang terkait dengan kunci bisa berupa tipe data apa saja (termasuk list, dictionary lain, dll.) dan boleh duplikat.
*   **Diakses Menggunakan Kunci:** Anda mengambil nilai dari dictionary menggunakan kuncinya, bukan menggunakan indeks numerik seperti list/tuple.

Dictionary didefinisikan menggunakan kurung kurawal `{}` dengan pasangan `key: value` dipisahkan oleh koma.

#### Membuat Dictionary (Key-Value Pairs)

```python
# Dictionary kosong
dict_kosong = {}
dict_kosong_lain = dict() # Konstruktor

# Dictionary data mahasiswa (kunci: string, nilai: campuran)
mahasiswa = {
    "nama": "Budi Santoso",
    "nim": "123456",
    "prodi": "Informatika",
    "angkatan": 2021,
    "lulus": False,
    "mata_kuliah": ["Kalkulus", "Daspro", "Logika"], # Nilai bisa list
    "nilai": {"Kalkulus": "A", "Daspro": "B+"} # Nilai bisa dict lain
}
print(f"Dict mahasiswa:\n{mahasiswa}\n")

# Dictionary dengan kunci integer
kode_pos = {
    10110: "Jakarta Pusat",
    40111: "Bandung",
    50111: "Semarang"
}
print(f"Dict kode_pos: {kode_pos}\n")

# Membuat dictionary dari list tuple (atau iterable pasangan lainnya)
pasangan_kunci_nilai = [('a', 1), ('b', 2), ('c', 3), ('a', 99)] # Kunci 'a' duplikat, yg terakhir dipakai
dict_dari_pasangan = dict(pasangan_kunci_nilai)
print(f"Dict dari list pasangan: {dict_dari_pasangan}") # Output: {'a': 99, 'b': 2, 'c': 3}

# Menggunakan argumen keyword pada konstruktor dict() (kunci harus string yg valid sbg identifier)
dict_keyword = dict(nama="Citra", usia=25, kota="Bandung")
print(f"Dict dari keyword args: {dict_keyword}") # Output: {'nama': 'Citra', 'usia': 25, 'kota': 'Bandung'}
```

#### Mengakses Nilai (Menggunakan Key)

Anda mengakses nilai dalam dictionary menggunakan kuncinya di dalam kurung siku `[]`, mirip indexing tapi pakai kunci.

```python
mahasiswa = {
    "nama": "Budi Santoso",
    "nim": "123456",
    "prodi": "Informatika",
    "nilai": {"Kalkulus": "A", "Daspro": "B+"}
}

# Mengakses nilai
print(f"Nama Mahasiswa: {mahasiswa['nama']}") # Output: Budi Santoso
print(f"Program Studi: {mahasiswa['prodi']}") # Output: Informatika
print(f"Nilai Kalkulus: {mahasiswa['nilai']['Kalkulus']}") # Akses dict bersarang

# Jika kunci TIDAK ADA, akan menghasilkan KeyError
# print(mahasiswa['alamat']) # KeyError: 'alamat'

# Cara Lebih Aman: Menggunakan metode get()
# get(key, default=None) -> mengembalikan nilai jika key ada,
#                          atau 'default' jika key tidak ada (defaultnya None)
alamat = mahasiswa.get('alamat') # Kunci 'alamat' tidak ada -> mengembalikan None
print(f"Alamat (get): {alamat}") # Output: None

kota_default = "Belum Ditentukan"
kota = mahasiswa.get('kota', kota_default) # Beri nilai default jika tidak ada
print(f"Kota (get dgn default): {kota}") # Output: Belum Ditentukan

nim = mahasiswa.get('nim', 'NIM Tidak Ada') # Kunci 'nim' ada
print(f"NIM (get): {nim}") # Output: 123456
```
Menggunakan `get()` lebih disukai daripada akses `[]` jika Anda tidak yakin apakah kunci tersebut ada, untuk menghindari `KeyError` yang menghentikan program.

#### Memodifikasi Dictionary (Mutable)

Anda dapat menambah pasangan baru, mengubah nilai yang sudah ada, atau menghapus pasangan kunci-nilai.

```python
profil = {"nama": "Dewi", "usia": 28, "kota": "Yogyakarta"}
print(f"Profil awal: {profil}")

# 1. Menambah pasangan baru / Mengubah nilai yang sudah ada
#    Jika kunci belum ada, pasangan baru ditambahkan.
#    Jika kunci sudah ada, nilainya diperbarui (ditimpa).
profil["pekerjaan"] = "Data Analyst" # Tambah kunci baru 'pekerjaan'
profil["usia"] = 29                 # Ubah nilai kunci 'usia' yang sudah ada
profil["email"] = "dewi@mail.com"   # Tambah kunci baru 'email'

print(f"Setelah menambah/ubah: {profil}")
# Output (urutan mungkin beda sebelum 3.7):
# {'nama': 'Dewi', 'usia': 29, 'kota': 'Yogyakarta', 'pekerjaan': 'Data Analyst', 'email': 'dewi@mail.com'}

# 2. Menghapus pasangan kunci-nilai

#    a) Menggunakan del
del profil["kota"] # Hapus pasangan dengan kunci 'kota'
print(f"Setelah del profil['kota']: {profil}")
# del profil['negara'] # Akan menghasilkan KeyError jika kunci tidak ada

#    b) Menggunakan pop(key, default)
#       Menghapus pasangan dengan 'key' dan MENGEMBALIKAN nilainya.
#       Jika key tidak ada, mengembalikan 'default' (jika diberikan), atau error.
pekerjaan_dihapus = profil.pop("pekerjaan")
print(f"Pekerjaan yang di-pop: {pekerjaan_dihapus}") # Output: Data Analyst
print(f"Setelah pop('pekerjaan'): {profil}") # Output: {'nama': 'Dewi', 'usia': 29, 'email': 'dewi@mail.com'}

# Coba pop kunci yg tidak ada dengan default -> tidak error
negara = profil.pop('negara', 'Indonesia')
print(f"Negara (pop dgn default): {negara}") # Output: Indonesia
print(f"Profil setelah pop negara: {profil}") # Tidak berubah

# Coba pop kunci yg tidak ada tanpa default -> error
# status = profil.pop('status') # KeyError

#    c) Menggunakan popitem()
#       Menghapus dan mengembalikan pasangan (key, value) terakhir yang dimasukkan (LIFO - Last In First Out) di Python 3.7+.
#       Sebelum Python 3.7, menghapus pasangan acak.
#       Menghasilkan KeyError jika dictionary kosong.
item_terakhir = profil.popitem()
print(f"Item yang di-pop (terakhir): {item_terakhir}") # Output: ('email', 'dewi@mail.com')
print(f"Profil setelah popitem(): {profil}") # Output: {'nama': 'Dewi', 'usia': 29}

#    d) Menggunakan clear() -> Menghapus SEMUA item
# profil.clear()
# print(f"Profil setelah clear(): {profil}") # Output: {}

# 3. Menggabungkan/Memperbarui dengan dictionary lain (update())
data_tambahan = {"kota": "Surabaya", "usia": 30, "status": "Aktif"} # 'usia' akan diperbarui
profil.update(data_tambahan)
# Bisa juga: profil.update(kota="Surabaya", usia=30, status="Aktif")
print(f"Profil setelah update(): {profil}")
# Output: {'nama': 'Dewi', 'usia': 30, 'kota': 'Surabaya', 'status': 'Aktif'}
```

#### Metode Dictionary (`keys()`, `values()`, `items()`, `get()`, `pop()`, `popitem()`, `update()`, `clear()`)

Beberapa metode penting lainnya:

*   `keys()`: Mengembalikan objek *view* yang berisi semua kunci dictionary. View ini dinamis (berubah jika dict berubah) dan bisa diiterasi.
*   `values()`: Mengembalikan *view object* yang berisi semua nilai dictionary.
*   `items()`: Mengembalikan *view object* yang berisi pasangan `(key, value)` sebagai tuple. Sangat berguna untuk iterasi.
*   `setdefault(key, default=None)`: Jika `key` ada di dictionary, kembalikan nilainya. Jika tidak, sisipkan `key` dengan nilai `default` ke dalam dictionary, lalu kembalikan `default`. Berguna untuk menginisialisasi kunci jika belum ada.
*   `copy()`: Mengembalikan salinan dangkal (shallow copy) dari dictionary.

```python
kontak = {"Andi": "0812", "Budi": "0856", "Citra": "0878"}
print(f"\nKontak awal: {kontak}")

print(f"Kunci (keys view): {kontak.keys()}")     # Output: dict_keys(['Andi', 'Budi', 'Citra'])
print(f"Nilai (values view): {kontak.values()}")   # Output: dict_values(['0812', '0856', '0878'])
print(f"Item (items view): {kontak.items()}")    # Output: dict_items([('Andi', '0812'), ('Budi', '0856'), ('Citra', '0878')])

# View objects bisa diubah menjadi list jika perlu (membuat salinan statis)
list_kunci = list(kontak.keys())
print(f"List kunci: {list_kunci}") # Output: ['Andi', 'Budi', 'Citra']

# View objects dinamis
dict_nilai = {'a': 1}
views_nilai = dict_nilai.values()
print(f"Views nilai awal: {views_nilai}") # dict_values([1])
dict_nilai['b'] = 2
print(f"Views nilai setelah tambah: {views_nilai}") # dict_values([1, 2]) (ikut berubah)

# setdefault()
# Coba dapatkan nomor Dewi, jika tidak ada, tambahkan & beri default
nomor_dewi = kontak.setdefault("Dewi", "Nomor Belum Ada")
print(f"Nomor Dewi (setdefault): {nomor_dewi}") # Output: Nomor Belum Ada
print(f"Kontak setelah setdefault Dewi: {kontak}") # 'Dewi' ditambahkan

# Coba dapatkan nomor Andi (sudah ada)
nomor_andi = kontak.setdefault("Andi", "XXX") # Andi sudah ada, nilai tidak diubah
print(f"Nomor Andi (setdefault): {nomor_andi}") # Output: 0812 (nilai lama dikembalikan)
print(f"Kontak setelah setdefault Andi: {kontak}") # Tidak berubah
```

#### Iterasi Melalui Dictionary

Ada beberapa cara umum untuk melakukan iterasi (loop) pada dictionary:

```python
data_produk = {"B001": "Laptop", "B002": "Mouse", "B003": "Keyboard"}
print("\n--- Iterasi Dictionary ---")

# 1. Iterasi melalui kunci (ini adalah default jika Anda loop langsung dict)
print("Iterasi Kunci (default):")
for kode in data_produk: # Sama dengan 'for kode in data_produk.keys():'
    nilai = data_produk[kode] # Ambil nilai pakai kunci
    print(f"  Kode: {kode} -> Produk: {nilai}")

# 2. Iterasi melalui nilai
print("\nIterasi Nilai:")
for nama_produk in data_produk.values():
    print(f"- {nama_produk}")

# 3. Iterasi melalui item (pasangan kunci-nilai) - paling umum jika butuh keduanya
print("\nIterasi Item (Kunci & Nilai):")
for kode, nama_produk in data_produk.items():
    print(f"  Kode: {kode}, Nama Produk: {nama_produk}")
```

#### Dictionary Comprehensions

Mirip list/set comprehensions, ini adalah cara ringkas untuk membuat dictionary baru dari iterable lain.

**Sintaks:** `{key_ekspresi: value_ekspresi for item in iterable if kondisi}`

```python
# Membuat dictionary kuadrat {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
dict_kuadrat = {x: x**2 for x in range(5)}
print(f"\nDict Kuadrat: {dict_kuadrat}")

# Membuat dictionary dari dua list (kunci dan nilai)
list_kunci = ['a', 'b', 'c', 'd']
list_nilai = [10, 20, 30, 40]
# zip() menggabungkan dua iterable menjadi pasangan tuple
dict_gabungan = {k: v for k, v in zip(list_kunci, list_nilai)}
print(f"Dict Gabungan dari zip: {dict_gabungan}") # {'a': 10, 'b': 20, 'c': 30, 'd': 40}

# Membuat dictionary baru dengan nilai > 50 dari dict lain (filter)
dict_asli = {"apel": 30, "pisang": 60, "jeruk": 80, "mangga": 20}
dict_filter = {k: v for k, v in dict_asli.items() if v > 50}
print(f"Dict Filter (nilai > 50): {dict_filter}") # {'pisang': 60, 'jeruk': 80}

# Tukar kunci dan nilai (hati-hati jika nilai tidak unik)
dict_tukar = {v: k for k, v in dict_asli.items()}
print(f"Dict Tukar Kunci-Nilai: {dict_tukar}") # {30: 'apel', 60: 'pisang', 80: 'jeruk', 20: 'mangga'}
```

#### Dictionary Bersarang (Nested Dictionaries)

Dictionary bisa berisi dictionary lain sebagai nilainya. Ini sangat berguna untuk merepresentasikan struktur data yang kompleks atau objek JSON.

```python
database_pegawai = {
    "P001": {
        "nama": "Agus",
        "jabatan": "Manager",
        "gaji": 15000000,
        "kontak": {"email": "agus@corp.com", "telepon": "0811"}
    },
    "P002": {
        "nama": "Sari",
        "jabatan": "Staff",
        "gaji": 8000000,
        "kontak": {"email": "sari@corp.com"} # Mungkin tidak punya telepon
    },
    "P003": {
        "nama": "Joko",
        "jabatan": "Staff",
        "gaji": 8500000,
        "kontak": {"email": "joko@corp.com", "telepon": "0833"}
    }
}
print("\n--- Database Pegawai (Nested Dict) ---")

# Mengakses data bersarang
print(f"Nama Pegawai P002: {database_pegawai['P002']['nama']}")   # Output: Sari
print(f"Gaji Pegawai P003: {database_pegawai['P003']['gaji']}")     # Output: 8500000
print(f"Email Pegawai P001: {database_pegawai['P001']['kontak']['email']}") # Output: agus@corp.com

# Menggunakan get() untuk keamanan saat akses bersarang
telp_sari = database_pegawai.get("P002", {}).get("kontak", {}).get("telepon", "Tidak Ada")
print(f"Telepon Sari: {telp_sari}") # Output: Tidak Ada

# Menambah data pegawai baru
database_pegawai["P004"] = {
    "nama": "Rina",
    "jabatan": "Supervisor",
    "gaji": 11000000,
    "kontak": {"email": "rina@corp.com"}
}

# Iterasi melalui dictionary bersarang
print("\nData Semua Pegawai:")
for id_pegawai, data_peg in database_pegawai.items():
    print(f"ID: {id_pegawai}")
    for kunci, nilai in data_peg.items():
        if isinstance(nilai, dict): # Jika nilainya dict lagi
             print(f"  {kunci.capitalize()}:")
             for sub_kunci, sub_nilai in nilai.items():
                 print(f"    {sub_kunci.capitalize()}: {sub_nilai}")
        else:
             print(f"  {kunci.capitalize()}: {nilai}")
    print("-" * 15) # Pemisah antar pegawai
```

---

## 6. Fungsi

Fungsi adalah blok kode terorganisir dan dapat digunakan kembali (reusable) yang dirancang untuk melakukan tugas tertentu. Menggunakan fungsi membantu membuat kode lebih modular, mudah dibaca, mudah di-debug, dan mengurangi pengulangan kode (prinsip DRY - Don't Repeat Yourself).

### Mendefinisikan Fungsi (`def`)

Di Python, Anda mendefinisikan fungsi menggunakan kata kunci `def`, diikuti dengan nama fungsi (konvensi `snake_case`), tanda kurung `()`, dan diakhiri dengan titik dua `:`. Kode di dalam fungsi (badan fungsi/function body) harus diindentasi.

```python
# Mendefinisikan fungsi sederhana tanpa input
def sapa_dunia():
  """
  Fungsi ini mencetak pesan sapaan standar.
  Ini adalah contoh docstring multi-baris.
  """
  pesan = "Halo, Dunia!"
  print(pesan)

# Mendefinisikan fungsi lain
def cetak_pemisah(karakter="-", panjang=20):
  """Mencetak garis pemisah dengan karakter dan panjang tertentu."""
  print(karakter * panjang)
```

**Docstrings (String Dokumentasi):** Sangat disarankan untuk menyertakan string literal (biasanya multi-baris dengan `"""..."""`) tepat setelah baris `def`. Ini adalah *docstring* yang menjelaskan apa yang dilakukan fungsi, parameternya, apa yang dikembalikan, dll. Docstring ini dapat diakses menggunakan `help(nama_fungsi)` atau `nama_fungsi.__doc__`.

### Memanggil Fungsi

Setelah fungsi didefinisikan, Anda dapat *memanggil* atau *menjalankannya* (execute) dengan menuliskan nama fungsi diikuti tanda kurung `()`. Jika fungsi memerlukan argumen, Anda menyediakannya di dalam tanda kurung.

```python
print("Memanggil fungsi sapa_dunia:")
sapa_dunia() # Panggil fungsi pertama

print("\nMemanggil fungsi cetak_pemisah:")
cetak_pemisah() # Panggil dengan argumen default
cetak_pemisah("*", 30) # Panggil dengan argumen custom
cetak_pemisah(panjang=10, karakter="=") # Panggil dengan argumen keyword

print("\nMemanggil sapa_dunia lagi:")
sapa_dunia()

# Mengakses docstring
print("\nDocstring sapa_dunia():")
print(sapa_dunia.__doc__)
# help(cetak_pemisah) # Akan menampilkan docstring di konsol interaktif
```

### Parameter dan Argumen

Fungsi dapat menerima input agar lebih fleksibel. Input ini didefinisikan sebagai **parameter** dalam definisi fungsi dan diberikan sebagai **argumen** saat fungsi dipanggil.

*   **Parameter:** Variabel yang tercantum di dalam tanda kurung pada definisi fungsi (`def nama_fungsi(parameter1, parameter2):`). Mereka bertindak sebagai placeholder untuk nilai yang akan diterima fungsi.
*   **Argumen:** Nilai aktual yang Anda kirim ke fungsi saat Anda memanggilnya (`nama_fungsi(argumen1, argumen2)`).

```python
# Fungsi dengan satu parameter 'nama'
def sapa_pengguna(nama): # 'nama' adalah parameter
  """Menyapa pengguna dengan nama spesifik."""
  print(f"Halo, {nama}! Selamat datang di program ini.")

# Memanggil fungsi dengan argumen "Budi"
sapa_pengguna("Budi") # "Budi" adalah argumen untuk parameter 'nama'

# Memanggil fungsi dengan argumen "Ani"
nama_lain = "Ani"
sapa_pengguna(nama_lain) # Variabel juga bisa jadi argumen

# Fungsi dengan dua parameter
def hitung_luas_persegi_panjang(panjang, lebar): # 'panjang' dan 'lebar' adalah parameter
  """Menghitung luas persegi panjang."""
  luas = panjang * lebar
  print(f"Persegi panjang dengan P={panjang} dan L={lebar} memiliki luas = {luas}")

# Memanggil fungsi 'hitung_luas_persegi_panjang' dengan argumen 10 dan 5
hitung_luas_persegi_panjang(10, 5) # 10 -> panjang, 5 -> lebar (argumen positional)
```

#### Jenis Argumen

Python sangat fleksibel dalam cara argumen dapat diteruskan ke fungsi:

1.  **Argumen Positional:** Argumen diteruskan ke fungsi berdasarkan **posisinya**. Argumen pertama yang Anda berikan saat pemanggilan akan cocok dengan parameter pertama dalam definisi fungsi, argumen kedua cocok dengan parameter kedua, dan seterusnya. **Urutan sangat penting.**
    ```python
    def info_bio(nama, usia, kota):
      print(f"Nama: {nama}, Usia: {usia}, Kota: {kota}")

    # Argumen positional: "Citra" -> nama, 25 -> usia, "Jakarta" -> kota
    info_bio("Citra", 25, "Jakarta")
    # info_bio(25, "Citra", "Jakarta") # Ini salah secara logika karena urutan tidak cocok
    ```

2.  **Argumen Keyword:** Anda dapat secara eksplisit menentukan argumen mana yang cocok dengan parameter mana dengan menggunakan `nama_parameter=nilai` saat memanggil fungsi. **Urutan argumen keyword tidak penting**, selama mereka muncul *setelah* semua argumen positional (jika ada). Ini membuat pemanggilan fungsi lebih jelas, terutama jika ada banyak parameter atau parameter opsional.
    ```python
    def info_bio(nama, usia, kota):
      print(f"Nama: {nama}, Usia: {usia}, Kota: {kota}")

    # Menggunakan argumen keyword (urutan bebas)
    info_bio(nama="Doni", kota="Surabaya", usia=30)
    info_bio(kota="Bandung", nama="Eka", usia=22)

    # Kombinasi positional dan keyword (positional HARUS duluan)
    info_bio("Fani", kota="Medan", usia=28)
    # info_bio(nama="Gita", 35, kota="Bali") # Salah! Argumen positional tidak boleh setelah keyword
    info_bio("Gita", usia=35, kota="Bali") # Benar
    ```

3.  **Parameter Default:** Anda dapat memberikan nilai default untuk satu atau lebih parameter dalam *definisi* fungsi. Jika argumen untuk parameter tersebut *tidak* diberikan saat pemanggilan, nilai default akan digunakan. Parameter dengan nilai default **harus diletakkan setelah** parameter tanpa nilai default dalam definisi fungsi.
    ```python
    def kirim_pesan(penerima, pesan, prioritas="Normal"): # 'prioritas' punya default
      """Mengirim pesan dengan prioritas tertentu."""
      print(f"Mengirim ke: {penerima}")
      print(f"Pesan: {pesan}")
      print(f"Prioritas: {prioritas}")
      print("---")

    kirim_pesan("Andi", "Meeting jam 10 pagi") # 'prioritas' pakai default "Normal"
    kirim_pesan("Budi", "Tolong cek email!", prioritas="Tinggi") # Memberi argumen untuk 'prioritas'
    kirim_pesan(pesan="Jangan lupa laporan!", penerima="Citra") # Pakai keyword
    ```
    **Perhatian penting dengan nilai default mutable:** Hindari menggunakan objek mutable (seperti list `[]` atau dictionary `{}`) sebagai nilai default secara langsung. Objek default dibuat *hanya sekali* saat fungsi didefinisikan, bukan setiap kali dipanggil. Ini bisa menyebabkan perilaku tak terduga jika objek default tersebut dimodifikasi di dalam fungsi.
    ```python
    # Contoh BURUK: Jangan gunakan list mutable sebagai default
    def tambah_item_buruk(item, keranjang=[]):
        keranjang.append(item)
        return keranjang

    list1 = tambah_item_buruk("apel")
    print(f"List 1 (buruk): {list1}") # ['apel']
    list2 = tambah_item_buruk("pisang") # Modifikasi list default yang SAMA!
    print(f"List 2 (buruk): {list2}") # ['apel', 'pisang'] -> TIDAK DIHARAPKAN!

    # Cara yang BENAR: Gunakan None sebagai default dan buat objek baru di dalam fungsi
    def tambah_item_baik(item, keranjang=None):
        if keranjang is None:
            keranjang = [] # Buat list baru jika tidak ada yang diberikan
        keranjang.append(item)
        return keranjang

    list3 = tambah_item_baik("apel")
    print(f"\nList 3 (baik): {list3}") # ['apel']
    list4 = tambah_item_baik("pisang") # Membuat list baru karena default None
    print(f"List 4 (baik): {list4}") # ['pisang'] -> SESUAI HARAPAN!
    list5 = tambah_item_baik("jeruk", ["mangga"]) # Menambah ke list yg sudah ada
    print(f"List 5 (baik): {list5}") # ['mangga', 'jeruk']
    ```

4.  **Argumen Arbitrer (`*args`):** Memungkinkan fungsi menerima sejumlah argumen *positional* yang tidak ditentukan sebelumnya. Argumen-argumen ini akan dikumpulkan ke dalam sebuah **tuple**. Nama `args` adalah konvensi, Anda bisa menggunakan nama lain diawali `*` (misal `*values`). Parameter `*args` harus diletakkan *setelah* parameter positional/default biasa.
    ```python
    def jumlahkan_semua(*angka): # 'angka' akan menjadi tuple
      """Menjumlahkan semua angka yang diberikan sebagai argumen."""
      print(f"Menerima tuple angka: {angka}")
      total = 0
      for n in angka:
          if isinstance(n, (int, float)):
              total += n
          else:
              print(f"Peringatan: Melewati nilai non-angka: {n}")
      return total

    print(f"\nJumlah (1, 2, 3): {jumlahkan_semua(1, 2, 3)}")
    print(f"Jumlah (10, 20, 30, 40, 50): {jumlahkan_semua(10, 20, 30, 40, 50)}")
    print(f"Jumlah (5): {jumlahkan_semua(5)}")
    print(f"Jumlah (): {jumlahkan_semua()}") # Tuple kosong
    print(f"Jumlah (1, 'a', 2.5): {jumlahkan_semua(1, 'a', 2.5)}")
    ```

5.  **Argumen Keyword Arbitrer (`**kwargs`):** Memungkinkan fungsi menerima sejumlah argumen *keyword* yang tidak ditentukan sebelumnya. Argumen-argumen ini akan dikumpulkan ke dalam sebuah **dictionary**. Nama `kwargs` adalah konvensi, Anda bisa menggunakan nama lain diawali `**` (misal `**options`). Parameter `**kwargs` harus diletakkan *paling akhir* dalam daftar parameter.
    ```python
    def cetak_info_lengkap(id_utama, *args, **kwargs):
      """Mencetak ID utama, argumen positional, dan keyword tambahan."""
      print(f"ID Utama: {id_utama}")

      if args:
          print("Info Tambahan (Positional):")
          for i, val in enumerate(args):
              print(f"  - Arg {i+1}: {val}")

      if kwargs: # Cek jika dictionary kwargs tidak kosong
          print("Detail Tambahan (Keyword):")
          for kunci, nilai in kwargs.items():
              print(f"  - {kunci.replace('_', ' ').title()}: {nilai}")
      print("-" * 20)

    cetak_info_lengkap("ID001")
    cetak_info_lengkap("ID002", "Status Aktif", 100) # 100 dan "Status Aktif" masuk ke *args
    cetak_info_lengkap("ID003", nama="Produk A", harga=50000, stok=10) # nama, harga, stok masuk ke **kwargs
    cetak_info_lengkap("ID004", "Prioritas Tinggi", "Data Valid",
                       pembuat="Admin", tanggal_buat="2024-01-15", lokasi="Gudang B")
    ```
    **Urutan umum parameter:** `posisional, default, *args, **kwargs`.

### Nilai Kembali (`return`)

Secara default, fungsi di Python mengembalikan `None` jika tidak ada pernyataan `return` eksplisit atau jika `return` dieksekusi tanpa nilai. Anda dapat menggunakan pernyataan `return` untuk mengirimkan satu atau lebih nilai kembali ke kode yang memanggil fungsi. Ketika `return` dieksekusi, fungsi segera berhenti dan nilai yang ditentukan dikembalikan.

```python
def kalikan(a, b):
  """Mengalikan dua angka dan mengembalikan hasilnya."""
  hasil = a * b
  return hasil # Mengembalikan nilai dari variabel hasil

# Memanggil fungsi dan menyimpan nilai kembaliannya
hasil_perkalian = kalikan(6, 7)
print(f"Hasil perkalian 6 * 7 = {hasil_perkalian}")

# Bisa juga digunakan langsung dalam ekspresi lain
print(f"5 * 8 + 2 = {kalikan(5, 8) + 2}")

# Fungsi tanpa return eksplisit akan mengembalikan None
def cetak_pesan(pesan):
  print(f"Pesan: {pesan}")
  # Tidak ada return di sini

nilai_kembalian = cetak_pesan("Ini hanya dicetak.")
print(f"Nilai kembalian dari cetak_pesan: {nilai_kembalian}") # Output: None

# Fungsi bisa berhenti lebih awal dengan return
def cari_angka(list_angka, target):
  """Mencari indeks angka target dalam list."""
  for indeks, angka in enumerate(list_angka):
    if angka == target:
      print(f"Target {target} ditemukan di indeks {indeks}.")
      return indeks # Keluar dari fungsi segera setelah ditemukan
  # Kode ini hanya jalan jika loop selesai tanpa menemukan target
  print(f"Target {target} tidak ditemukan dalam list.")
  return -1 # Mengembalikan nilai penanda (misal -1) jika tidak ketemu

indeks_ketemu = cari_angka([10, 20, 30, 40, 50], 30) # Output: Target 30 ditemukan...
print(f"Hasil pencarian 30: {indeks_ketemu}") # Output: 2

indeks_tdk_ketemu = cari_angka([10, 20, 30], 99) # Output: Target 99 tidak...
print(f"Hasil pencarian 99: {indeks_tdk_ketemu}") # Output: -1
```

#### Mengembalikan Beberapa Nilai (sebagai Tuple)

Jika Anda menulis `return nilai1, nilai2, nilai3`, Python secara otomatis akan membungkus nilai-nilai tersebut ke dalam sebuah **tuple** sebelum mengembalikannya. Anda dapat menangkap hasil ini sebagai satu tuple atau langsung melakukan unpacking ke beberapa variabel.

```python
import math

def hitung_lingkaran(radius):
  """Menghitung luas dan keliling lingkaran."""
  if radius < 0:
      return None, None # Kembalikan None jika input tidak valid

  luas = math.pi * radius**2
  keliling = 2 * math.pi * radius
  return luas, keliling # Mengembalikan dua nilai (otomatis jadi tuple)

# Memanggil fungsi dan menangkap kedua nilai via unpacking
luas_ling, kel_ling = hitung_lingkaran(7)
if luas_ling is not None:
    print(f"\nLingkaran radius 7:")
    print(f"  Luas: {luas_ling:.2f}")
    print(f"  Keliling: {kel_ling:.2f}")

# Bisa juga ditangkap sebagai satu tuple
hasil_hitungan = hitung_lingkaran(10)
if hasil_hitungan != (None, None):
    print(f"\nHasil hitungan (radius 10) sebagai tuple: {hasil_hitungan}")
    print(f"Tipe hasil_hitungan: {type(hasil_hitungan)}")
    # Akses via indeks tuple
    print(f"  Luas dari tuple: {hasil_hitungan[0]:.2f}")
    print(f"  Keliling dari tuple: {hasil_hitungan[1]:.2f}")

hasil_invalid = hitung_lingkaran(-5)
print(f"\nHasil untuk radius -5: {hasil_invalid}") # Output: (None, None)
```

### Scope Variabel (LEGB Rule: Local, Enclosing, Global, Built-in)

Scope (lingkup) menentukan di mana saja dalam program sebuah variabel dapat diakses atau dikenali. Python menggunakan aturan LEGB untuk mencari nama variabel:

1.  **L - Local Scope:** Variabel yang didefinisikan di dalam fungsi saat ini. Ini adalah scope pertama yang diperiksa. Variabel ini hanya ada selama fungsi tersebut dieksekusi.
2.  **E - Enclosing Function Locals Scope:** Jika fungsi didefinisikan di dalam fungsi lain (fungsi bersarang/nested function), Python akan mencari variabel di scope fungsi yang melingkupinya (enclosing function). Ini dicari jika variabel tidak ditemukan di scope Local.
3.  **G - Global Scope:** Variabel yang didefinisikan di level teratas modul (di luar semua fungsi). Ini dicari jika variabel tidak ditemukan di scope Local dan Enclosing.
4.  **B - Built-in Scope:** Nama-nama yang sudah ada di Python secara bawaan (misalnya fungsi `print()`, `len()`, `type()`, nama exceptions seperti `ValueError`). Ini adalah scope terakhir yang diperiksa.

```python
# Global Scope
pesan_global = "Ini variabel global"
angka_global = 100

def fungsi_luar():
    # Enclosing Function Scope
    pesan_enclosing = "Ini variabel enclosing"
    angka_luar = 20

    def fungsi_dalam():
        # Local Scope
        pesan_lokal = "Ini variabel lokal"
        angka_dalam = 5

        # Mencari variabel:
        print(f"Dalam fungsi_dalam:")
        print(f"  Mencari pesan_lokal: {pesan_lokal}") # L -> Ditemukan
        print(f"  Mencari pesan_enclosing: {pesan_enclosing}") # E -> Ditemukan
        print(f"  Mencari pesan_global: {pesan_global}") # G -> Ditemukan
        # print(pesan_tidak_ada) # Akan NameError

        # Memodifikasi variabel lokal (boleh)
        angka_dalam_baru = angka_dalam + 1
        print(f"  Angka dalam baru: {angka_dalam_baru}")

        # Membaca variabel enclosing dan global (boleh)
        print(f"  Membaca angka_luar: {angka_luar}")
        print(f"  Membaca angka_global: {angka_global}")

        # Mencoba modifikasi global/enclosing tanpa keyword akan membuat variabel LOKAL baru!
        # angka_global = 999 # Ini membuat variabel 'angka_global' LOKAL di fungsi_dalam
        # angka_luar = 25   # Ini membuat variabel 'angka_luar' LOKAL di fungsi_dalam

    print(f"\nDalam fungsi_luar (sebelum panggil fungsi_dalam):")
    print(f"  pesan_enclosing: {pesan_enclosing}")
    # print(pesan_lokal) # NameError: pesan_lokal tidak ada di scope ini

    fungsi_dalam() # Panggil fungsi dalam

    print(f"\nDalam fungsi_luar (setelah panggil fungsi_dalam):")
    print(f"  angka_luar masih: {angka_luar}") # Tidak berubah jika 'fungsi_dalam' tidak pakai nonlocal

# Panggil fungsi luar
fungsi_luar()

print(f"\nDi scope Global:")
print(f"  pesan_global: {pesan_global}")
print(f"  angka_global masih: {angka_global}") # Tidak berubah jika 'fungsi_dalam' tidak pakai global
# print(pesan_enclosing) # NameError
# print(pesan_lokal) # NameError
```

#### Keyword `global`

Jika Anda ingin *memodifikasi* variabel yang ada di **Global Scope** dari dalam sebuah fungsi, Anda harus mendeklarasikannya menggunakan kata kunci `global` di awal fungsi.

```python
counter_global = 0 # Variabel global

def increment_global():
  global counter_global # Beri tahu Python kita ingin mengubah 'counter_global' global
  counter_global += 1
  print(f"  Counter di dalam fungsi: {counter_global}")

print(f"Counter global sebelum: {counter_global}")
increment_global()
increment_global()
print(f"Counter global sesudah: {counter_global}") # Output: 2
```
**Penggunaan `global` sebaiknya diminimalkan** karena dapat membuat alur data sulit dilacak dan melanggar prinsip enkapsulasi. Lebih baik melewatkan nilai sebagai argumen dan mengembalikan hasil jika memungkinkan.

#### Keyword `nonlocal`

Digunakan dalam **fungsi bersarang** untuk menunjukkan bahwa Anda ingin *memodifikasi* variabel yang ada di **Enclosing Function Scope** (bukan Local dan bukan Global).

```python
def fungsi_luar_nonlocal():
    angka = 10 # Variabel di scope enclosing

    def fungsi_dalam_nonlocal():
        nonlocal angka # Merujuk ke 'angka' di fungsi_luar_nonlocal
        angka += 5 # Modifikasi variabel enclosing
        print(f"    Angka di dalam fungsi_dalam: {angka}")

    print(f"  Angka sebelum fungsi_dalam dipanggil: {angka}")
    fungsi_dalam_nonlocal()
    print(f"  Angka setelah fungsi_dalam dipanggil: {angka}") # Nilai sudah berubah

print("\nContoh dengan nonlocal:")
fungsi_luar_nonlocal()
```

### Docstrings (Dokumentasi Fungsi)

Sangat penting untuk mendokumentasikan fungsi Anda menggunakan docstring. Ini membantu orang lain (dan diri Anda di masa depan) memahami cara menggunakan fungsi tanpa perlu membaca seluruh kodenya.

**Konvensi Umum (Google Style / NumPy Style / reStructuredText):**
*   Gunakan tanda kutip tiga (`"""Docstring di sini"""`).
*   Baris pertama: Ringkasan singkat fungsi (kalimat imperatif), diakhiri titik.
*   Baris kedua: Kosong.
*   Berikutnya: Penjelasan lebih detail (jika perlu).
*   Bagian `Args:` (atau `Parameters:`): Jelaskan setiap parameter, tipe data yang diharapkan, dan artinya.
*   Bagian `Returns:`: Jelaskan nilai yang dikembalikan oleh fungsi dan tipe datanya.
*   Bagian `Raises:` (opsional): Jelaskan exception apa saja yang mungkin dibangkitkan oleh fungsi dan dalam kondisi apa.

```python
def hitung_rata_rata(daftar_angka):
  """Menghitung nilai rata-rata dari sebuah list atau tuple angka.

  Args:
    daftar_angka (list or tuple): Sebuah list atau tuple yang berisi
      angka (int atau float). Iterable ini tidak boleh kosong.

  Returns:
    float: Nilai rata-rata dari angka dalam input.
           Mengembalikan 0.0 jika iterable input kosong setelah validasi
           (meskipun idealnya mungkin raise error).

  Raises:
    TypeError: Jika input bukan list atau tuple, atau jika salah satu
               elemen di dalamnya bukan int atau float.
    ValueError: Jika daftar_angka kosong (alternatif selain return 0.0).
  """
  if not isinstance(daftar_angka, (list, tuple)):
    raise TypeError("Input harus berupa list atau tuple.")
  if not daftar_angka:
    # Alternatif: raise ValueError("Daftar angka tidak boleh kosong.")
    print("Peringatan: Daftar angka kosong, mengembalikan 0.0")
    return 0.0

  total = 0
  jumlah_valid = 0
  for angka in daftar_angka:
    if not isinstance(angka, (int, float)):
      raise TypeError(f"Elemen '{angka}' bukan tipe numerik yang valid.")
    total += angka
    jumlah_valid += 1

  # Hindari ZeroDivisionError jika implementasi diubah untuk raise ValueError di atas
  # if jumlah_valid == 0:
  #     return 0.0 # Atau raise error

  return total / jumlah_valid

# Cara melihat docstring:
# help(hitung_rata_rata)
print("\nDocstring hitung_rata_rata:")
print(hitung_rata_rata.__doc__)
```

### Fungsi Lambda (Fungsi Anonim)

Fungsi lambda adalah cara ringkas untuk membuat fungsi kecil **tanpa nama** (anonim) dalam satu baris. Mereka sering digunakan ketika Anda membutuhkan fungsi sederhana untuk waktu yang singkat, misalnya sebagai argumen untuk fungsi tingkat tinggi seperti `map()`, `filter()`, atau `sorted()`.

**Sintaks:** `lambda arguments: expression`

*   `lambda`: Kata kunci penanda.
*   `arguments`: Satu atau lebih argumen (dipisahkan koma), sama seperti parameter fungsi biasa.
*   `: `: Pemisah antara argumen dan ekspresi.
*   `expression`: **Satu ekspresi tunggal** yang akan dievaluasi dan hasilnya **otomatis dikembalikan**. Lambda tidak bisa berisi pernyataan multi-baris, `if/else` kompleks (kecuali ternary), `for/while`, atau `return` eksplisit.

```python
# Fungsi biasa untuk menambah 10
def tambah_sepuluh(x):
  return x + 10

# Fungsi lambda yang setara
tambah_sepuluh_lambda = lambda x: x + 10

print(f"\nFungsi biasa: {tambah_sepuluh(5)}")      # Output: 15
print(f"Fungsi lambda: {tambah_sepuluh_lambda(5)}") # Output: 15

# Lambda dengan beberapa argumen
perkalian = lambda a, b: a * b
print(f"Perkalian lambda (6, 7): {perkalian(6, 7)}") # Output: 42

# Lambda tanpa argumen
sapa_lambda = lambda: "Halo dari lambda!"
print(f"Sapa lambda: {sapa_lambda()}") # Output: Halo dari lambda!

# Penggunaan umum lambda dengan fungsi lain:

angka = [1, 2, 3, 4, 5, 6]

# map(function, iterable): Terapkan function ke setiap item iterable
kuadrat = list(map(lambda x: x**2, angka))
print(f"Hasil map kuadrat: {kuadrat}") # [1, 4, 9, 16, 25, 36]

# filter(function, iterable): Ambil item dari iterable jika function(item) True
genap = list(filter(lambda x: x % 2 == 0, angka))
print(f"Hasil filter genap: {genap}") # [2, 4, 6]

# sorted(iterable, key=function): Urutkan iterable berdasarkan hasil key function
pasangan = [(1, 'c'), (3, 'a'), (2, 'b')]
# Urutkan berdasarkan elemen kedua (huruf)
urut_huruf = sorted(pasangan, key=lambda item: item[1])
print(f"Sorted berdasarkan huruf: {urut_huruf}") # [(3, 'a'), (2, 'b'), (1, 'c')]
# Urutkan berdasarkan elemen pertama (angka)
urut_angka = sorted(pasangan, key=lambda item: item[0])
print(f"Sorted berdasarkan angka: {urut_angka}") # [(1, 'c'), (2, 'b'), (3, 'a')]
```
Lambda sangat berguna untuk operasi singkat, tetapi jika logika Anda memerlukan lebih dari satu ekspresi atau menjadi kompleks, lebih baik gunakan fungsi `def` biasa agar lebih mudah dibaca dan dipelihara.

### Rekursi

Rekursi adalah teknik pemrograman di mana sebuah fungsi memanggil dirinya sendiri untuk menyelesaikan sub-masalah yang lebih kecil dari masalah asli. Fungsi rekursif harus memiliki dua komponen penting:

1.  **Kasus Dasar (Base Case):** Satu atau lebih kondisi di mana fungsi *tidak* memanggil dirinya sendiri lagi, melainkan mengembalikan hasil langsung. Ini adalah kondisi berhenti yang mencegah rekursi tak terbatas.
2.  **Langkah Rekursif (Recursive Step):** Bagian di mana fungsi memanggil dirinya sendiri, biasanya dengan argumen yang dimodifikasi sehingga lebih mendekati kasus dasar.

**Contoh klasik: Menghitung Faktorial (n!)**
n! = n * (n-1) * (n-2) * ... * 1
0! = 1 (Kasus Dasar)

```python
def faktorial_rekursif(n):
  """Menghitung faktorial n menggunakan rekursi."""
  # Validasi input (bukan bagian inti rekursi, tapi penting)
  if not isinstance(n, int) or n < 0:
      raise ValueError("Input harus integer non-negatif")

  # Kasus Dasar: n = 0
  if n == 0:
    print("  -> Kasus Dasar: faktorial(0) = 1")
    return 1
  # Langkah Rekursif: n > 0
  else:
    print(f"  -> Memanggil faktorial({n-1}) dari faktorial({n})")
    hasil_sebelumnya = faktorial_rekursif(n - 1) # Panggil diri sendiri
    hasil = n * hasil_sebelumnya
    print(f"  <- Kembali dari faktorial({n-1}), hasil={hasil_sebelumnya}. Menghitung {n} * {hasil_sebelumnya} = {hasil}")
    return hasil

print("Menghitung faktorial 4:")
hasil_fact_4 = faktorial_rekursif(4)
print(f"Hasil faktorial 4 = {hasil_fact_4}")

# Output akan menunjukkan alur pemanggilan:
# Menghitung faktorial 4:
#   -> Memanggil faktorial(3) dari faktorial(4)
#   -> Memanggil faktorial(2) dari faktorial(3)
#   -> Memanggil faktorial(1) dari faktorial(2)
#   -> Memanggil faktorial(0) dari faktorial(1)
#   -> Kasus Dasar: faktorial(0) = 1
#   <- Kembali dari faktorial(0), hasil=1. Menghitung 1 * 1 = 1
#   <- Kembali dari faktorial(1), hasil=1. Menghitung 2 * 1 = 2
#   <- Kembali dari faktorial(2), hasil=2. Menghitung 3 * 2 = 6
#   <- Kembali dari faktorial(3), hasil=6. Menghitung 4 * 6 = 24
# Hasil faktorial 4 = 24

# Bandingkan dengan versi iteratif (loop)
def faktorial_iteratif(n):
    if not isinstance(n, int) or n < 0:
        raise ValueError("Input harus integer non-negatif")
    hasil = 1
    for i in range(1, n + 1):
        hasil *= i
    return hasil

print(f"\nFaktorial 4 (iteratif): {faktorial_iteratif(4)}") # Output: 24
```
Rekursi bisa menjadi cara yang elegan dan intuitif untuk menyelesaikan masalah yang secara alami dapat dipecah menjadi sub-masalah yang sama (seperti menelusuri struktur pohon, beberapa algoritma sorting/searching). Namun, rekursi seringkali:
*   **Kurang efisien** daripada solusi iteratif (menggunakan loop) karena adanya overhead pemanggilan fungsi (setiap panggilan menyimpan state di call stack).
*   **Bisa lebih sulit dipahami** atau di-debug alurnya.
*   **Memiliki batas kedalaman rekursi** di Python (default biasanya 1000) untuk mencegah *stack overflow error*. Anda bisa mengubah batas ini (dengan `sys.setrecursionlimit()`), tetapi biasanya lebih baik mendesain ulang algoritma jika Anda mencapainya.

Pilih rekursi jika ia secara signifikan menyederhanakan logika dan keterbacaan kode untuk masalah yang cocok, tetapi pertimbangkan alternatif iteratif untuk efisiensi atau jika batas kedalaman menjadi masalah.

---

## 7. Modul dan Paket

Saat program Python Anda tumbuh lebih besar, menempatkan semua kode dalam satu file `.py` menjadi tidak praktis dan sulit dikelola. Python menyediakan mekanisme untuk mengorganisir kode ke dalam unit-unit yang lebih kecil dan dapat digunakan kembali: **modul** dan **paket**.

### Apa itu Modul?

Secara sederhana, **modul** adalah sebuah file Python (`.py`) yang berisi definisi dan pernyataan Python (fungsi, kelas, variabel). Modul memungkinkan Anda untuk:

*   **Mengorganisir Kode:** Memecah program besar menjadi file-file yang lebih kecil, logis, dan terfokus pada fungsionalitas tertentu (misalnya, satu modul untuk operasi database, satu lagi untuk utilitas string).
*   **Reusabilitas Kode:** Menggunakan kembali fungsi, kelas, atau variabel yang telah Anda definisikan dalam satu modul di modul atau program lain tanpa perlu menyalin kodenya.
*   **Namespacing:** Mencegah konflik nama. Variabel atau fungsi dalam satu modul memiliki *namespace* (ruang nama) sendiri, sehingga tidak akan bentrok dengan nama yang sama di modul lain atau di skrip utama Anda, kecuali jika Anda mengimpornya secara eksplisit dengan cara tertentu.

Contoh: Anda bisa membuat file `kalkulator.py` yang berisi fungsi `tambah`, `kurang`, dll., lalu menggunakan fungsi-fungsi tersebut di file `main.py`.

### Mengimpor Modul (`import`, `from ... import ...`, `import ... as ...`)

Untuk menggunakan kode (fungsi, kelas, variabel) dari modul lain, Anda perlu *mengimpornya* ke dalam file Python Anda saat ini menggunakan pernyataan `import`. Ada beberapa cara untuk melakukan impor:

1.  **`import nama_modul`**
    *   Mengimpor seluruh modul.
    *   Untuk mengakses isi modul (misalnya fungsi `fungsi_x` atau variabel `VAR_Y`), Anda **harus** menggunakan nama modul diikuti titik (`.`): `nama_modul.fungsi_x`, `nama_modul.VAR_Y`.
    *   Ini adalah cara impor yang **paling direkomendasikan** secara umum karena menjaga namespace tetap jelas dan eksplisit. Anda selalu tahu dari modul mana sebuah nama berasal.

    ```python
    # Misalkan ada file bernama 'matematika_ku.py' berisi:
    # PI = 3.14159
    # def luas_lingkaran(radius):
    #   return PI * radius**2
    # def keliling_lingkaran(radius):
    #   return 2 * PI * radius

    # Di file lain (misal main.py):
    import matematika_ku

    jari_jari = 5
    luas = matematika_ku.luas_lingkaran(jari_jari)
    keliling = matematika_ku.keliling_lingkaran(jari_jari)
    nilai_pi = matematika_ku.PI

    print(f"Lingkaran radius {jari_jari}:")
    print(f"  Luas = {luas:.2f}")
    print(f"  Keliling = {keliling:.2f}")
    print(f"  Nilai PI yang digunakan = {nilai_pi}")
    ```

2.  **`import nama_modul as alias`**
    *   Mengimpor seluruh modul tetapi memberinya **nama alias (nama panggilan)** yang lebih pendek atau lebih deskriptif.
    *   Anda kemudian menggunakan `alias.nama_objek` untuk mengakses isinya.
    *   Berguna jika nama modul asli terlalu panjang atau ada potensi konflik dengan nama lain di kode Anda.

    ```python
    import matematika_ku as mtk # Memberi alias 'mtk'
    import pandas as pd        # Alias sangat umum untuk library populer
    import numpy as np

    luas = mtk.luas_lingkaran(10)
    print(f"\nLuas (via alias 'mtk'): {luas:.2f}")

    # data = {'col1': [1, 2], 'col2': [3, 4]}
    # df = pd.DataFrame(data=data) # Menggunakan alias 'pd' untuk pandas
    ```

3.  **`from nama_modul import nama_objek1, nama_objek2, ...`**
    *   Mengimpor hanya objek (fungsi, kelas, variabel) **tertentu** dari modul langsung ke dalam namespace skrip Anda saat ini.
    *   Anda dapat menggunakan `nama_objek1`, `nama_objek2` secara langsung **tanpa** perlu mengetikkan `nama_modul.` di depannya.
    *   Bisa membuat kode sedikit lebih ringkas, tetapi dapat menyebabkan **kebingungan atau konflik nama** jika nama yang sama diimpor dari modul berbeda atau sudah didefinisikan di skrip Anda. Gunakan dengan hati-hati.

    ```python
    from matematika_ku import luas_lingkaran, PI # Hanya impor 2 objek ini
    # keliling_lingkaran tidak diimpor

    luas_langsung = luas_lingkaran(3) # Panggil langsung
    print(f"\nLuas langsung (radius 3): {luas_langsung:.2f}")
    print(f"Nilai PI langsung: {PI}")

    # keliling = keliling_lingkaran(3) # NameError! Karena tidak diimpor
    # print(matematika_ku.PI)          # NameError! Karena modul 'matematika_ku' tidak diimpor secara keseluruhan
    ```

4.  **`from nama_modul import nama_objek as alias_objek`**
    *   Mengimpor objek spesifik tetapi memberinya nama alias. Berguna untuk menghindari konflik nama atau membuat nama lebih pendek.

    ```python
    from matematika_ku import luas_lingkaran as hitung_luas
    from os.path import join as gabung_path

    luas = hitung_luas(4) # Gunakan alias 'hitung_luas'
    print(f"\nLuas (via alias objek): {luas:.2f}")

    path_file = gabung_path("folder", "subfolder", "file.txt")
    print(f"Path tergabung: {path_file}")
    ```

5.  **`from nama_modul import *` (Hindari Jika Memungkinkan!)**
    *   Mengimpor **semua** nama publik (yang tidak diawali `_`) dari modul ke namespace saat ini.
    *   Anda bisa memanggil semua fungsi/variabel dari modul tersebut secara langsung.
    *   **Ini umumnya dianggap praktik buruk (bad practice)** karena:
        *   **Polusi Namespace (Namespace Pollution):** Membanjiri namespace Anda dengan banyak nama, meningkatkan risiko konflik nama yang tidak disengaja dengan nama yang Anda definisikan sendiri atau dari impor lain.
        *   **Ketidakjelasan Sumber:** Sulit untuk melacak dari modul mana sebuah fungsi atau variabel berasal, membuat kode lebih sulit dibaca, dipahami, dan di-debug.
    *   Gunakan hanya dalam kasus yang sangat spesifik (misalnya, di shell interaktif Python untuk kenyamanan sementara) atau jika modul dirancang khusus untuk penggunaan ini (jarang terjadi dan biasanya didokumentasikan). Lebih baik impor secara eksplisit.

    ```python
    # Contoh (TIDAK DIREKOMENDASIKAN dalam skrip):
    # from matematika_ku import *
    # l = luas_lingkaran(1) # Bisa dipanggil langsung
    # k = keliling_lingkaran(1) # Bisa dipanggil langsung
    # print(PI) # Bisa diakses langsung
    ```

### Python Standard Library

Python hadir dengan "batteries included", artinya ia memiliki perpustakaan standar (Standard Library) yang sangat luas berisi banyak modul siap pakai untuk berbagai tugas umum. Anda tidak perlu menginstalnya secara terpisah; mereka sudah menjadi bagian dari instalasi Python Anda.

Beberapa contoh modul standar yang sering digunakan:

*   `math`: Fungsi matematika tingkat lanjut (trigonometri, logaritma, akar kuadrat, konstanta pi, e, dll.).
*   `random`: Fungsi untuk menghasilkan angka acak, memilih item acak dari urutan, mengacak urutan.
*   `datetime`: Kelas dan fungsi untuk bekerja dengan tanggal, waktu, zona waktu, dan durasi.
*   `os`: Berinteraksi dengan sistem operasi (misal: `os.getcwd()`, `os.listdir()`, `os.path.join()`, `os.makedirs()`, `os.environ`).
*   `sys`: Akses ke parameter dan fungsi spesifik interpreter Python (misal: `sys.argv` untuk argumen baris perintah, `sys.path` untuk path pencarian modul, `sys.exit()`).
*   `json`: Membaca (decode) dan menulis (encode) data dalam format JSON (JavaScript Object Notation).
*   `csv`: Membaca dan menulis file CSV (Comma Separated Values).
*   `re`: Operasi ekspresi reguler (Regular Expressions) untuk pencocokan pola teks yang kompleks.
*   `collections`: Struktur data tambahan seperti `defaultdict`, `Counter`, `deque`, `namedtuple`.
*   `urllib`: Modul untuk bekerja dengan URL (misalnya, mengambil data dari web, meskipun library pihak ketiga `requests` seringkali lebih mudah digunakan).
*   `itertools`: Fungsi untuk membuat iterator untuk perulangan yang efisien.
*   `functools`: Alat untuk bekerja dengan fungsi (misal: `partial`, `reduce`, `wraps` untuk decorator).

```python
import math
import random
import datetime
import os

# Menggunakan math
print(f"Akar kuadrat 16: {math.sqrt(16)}") # 4.0
print(f"Nilai pi: {math.pi}")

# Menggunakan random
angka_acak = random.randint(1, 100) # Integer acak antara 1 dan 100 (inklusif)
print(f"Angka acak: {angka_acak}")
pilihan = random.choice(["apel", "jeruk", "mangga"]) # Pilih satu item acak
print(f"Buah pilihan acak: {pilihan}")

# Menggunakan datetime
sekarang = datetime.datetime.now()
print(f"Tanggal dan waktu sekarang: {sekarang}")
print(f"Hanya tanggal: {sekarang.date()}")
print(f"Format custom: {sekarang.strftime('%Y-%m-%d %H:%M:%S')}") # Format YYYY-MM-DD HH:MM:SS

# Menggunakan os
dir_sekarang = os.getcwd() # Get current working directory
print(f"Direktori kerja saat ini: {dir_sekarang}")
# print(f"Isi direktori: {os.listdir(dir_sekarang)}") # Daftar file/folder
```

Anda sangat dianjurkan untuk menjelajahi dokumentasi Python Standard Library ([https://docs.python.org/3/library/](https://docs.python.org/3/library/)) untuk melihat modul apa saja yang tersedia sebelum Anda mencoba menulis ulang fungsionalitas umum atau mencari library pihak ketiga.

### Membuat Modul Sendiri

Membuat modul sendiri sangat mudah:

1.  Buat file Python baru (misal, `utilitas_string.py`).
2.  Tulis fungsi, kelas, atau variabel yang Anda inginkan di dalamnya.

```python
# File: utilitas_string.py

"""Modul ini berisi fungsi-fungsi utilitas untuk string."""

VERSI = "1.0"

def balik_string(s):
  """Mengembalikan string yang dibalik."""
  if not isinstance(s, str):
    return None # Atau raise TypeError
  return s[::-1]

def hitung_vokal(s):
  """Menghitung jumlah huruf vokal (a, i, u, e, o) dalam string (case-insensitive)."""
  if not isinstance(s, str):
    return 0
  vokal = "aiueo"
  jumlah = 0
  for huruf in s.lower(): # Ubah ke lowercase untuk case-insensitive
    if huruf in vokal:
      jumlah += 1
  return jumlah

# Kode ini hanya akan berjalan jika utilitas_string.py dijalankan sebagai script utama
# Bukan saat diimpor sebagai modul ke file lain.
if __name__ == "__main__":
  print(f"--- Menjalankan tes untuk modul utilitas_string (Versi {VERSI}) ---")

  teks_asli = "Python"
  teks_terbalik = balik_string(teks_asli)
  print(f"Membalik '{teks_asli}': '{teks_terbalik}'") # Output: 'nohtyP'

  kalimat = "Belajar Programming itu Menyenangkan"
  jml_vokal = hitung_vokal(kalimat)
  print(f"Jumlah vokal dalam '{kalimat}': {jml_vokal}") # Output: 11

  print("--- Tes Selesai ---")

```

3.  Di file Python lain (yang berada di direktori yang sama, atau di direktori yang ada dalam `sys.path` Python), impor dan gunakan modul Anda.

```python
# File: program_utama.py

import utilitas_string # Impor seluruh modul
# Atau: from utilitas_string import balik_string, hitung_vokal, VERSI
# Atau: import utilitas_string as ustr

kalimat_tes = "Halo Semuanya"

# Menggunakan fungsi dari modul
kalimat_terbalik = utilitas_string.balik_string(kalimat_tes)
print(f"'{kalimat_tes}' dibalik menjadi '{kalimat_terbalik}'")

jumlah_huruf_vokal = utilitas_string.hitung_vokal(kalimat_tes)
print(f"Jumlah vokal di '{kalimat_tes}': {jumlah_huruf_vokal}")

# Mengakses variabel dari modul
print(f"Versi modul utilitas string: {utilitas_string.VERSI}")

# Jika Anda menjalankan program_utama.py, output dari blok
# if __name__ == "__main__": di utilitas_string.py TIDAK akan muncul.
```

### Blok `if __name__ == "__main__":`

Anda akan sering melihat blok `if __name__ == "__main__":` di banyak file Python. Apa tujuannya?

*   Setiap modul Python memiliki variabel bawaan spesial bernama `__name__`.
*   Ketika Python menjalankan sebuah file sebagai **script utama** (misalnya Anda mengetik `python nama_file.py` di terminal), Python akan secara otomatis mengatur nilai `__name__` untuk file tersebut menjadi string `"__main__"`.
*   Ketika sebuah file Python **diimpor** sebagai modul ke file lain, Python akan mengatur nilai `__name__` untuk file yang diimpor tersebut menjadi **nama file modul itu sendiri** (tanpa ekstensi `.py`, misalnya `"utilitas_string"`).

Blok `if __name__ == "__main__":` memanfaatkan perilaku ini. Kode yang ditulis di dalam blok ini **hanya akan dieksekusi** ketika file tersebut dijalankan **secara langsung sebagai script utama**, dan **tidak akan dieksekusi** ketika file tersebut **diimpor sebagai modul**.

Ini sangat berguna untuk:

*   Menyertakan **kode pengujian (testing)** atau **contoh penggunaan** modul di dalam file modul itu sendiri tanpa mengganggu pengguna yang mengimpor modul tersebut.
*   Membuat modul yang bisa berfungsi ganda: sebagai **library** (kumpulan fungsi/kelas untuk diimpor) dan juga sebagai **program mandiri** yang bisa dijalankan dari baris perintah (misalnya untuk melakukan tugas spesifik menggunakan fungsi di dalamnya).

Lihat contoh di `utilitas_string.py` di atas. Jika Anda menjalankan `python utilitas_string.py`, Anda akan melihat output "--- Menjalankan tes..." dll. Jika Anda menjalankan `python program_utama.py` (yang mengimpor `utilitas_string`), output tes tersebut tidak akan muncul.

### Paket (Packages)

Ketika proyek Anda memiliki banyak modul, mengelompokkan modul-modul yang terkait secara logis menjadi **paket** adalah langkah selanjutnya dalam organisasi kode. Paket memungkinkan Anda menstrukturkan namespace modul menggunakan "dotted module names" (nama modul bertitik), seperti `paket.subpaket.modul`.

Secara fisik di sistem file, **paket adalah sebuah direktori** yang berisi:

1.  **Modul-modul Python** (`.py` files) yang merupakan bagian dari paket tersebut.
2.  Sebuah file khusus (bisa kosong) bernama `__init__.py`. Keberadaan file ini **penting** karena memberi tahu Python bahwa direktori tersebut harus diperlakukan sebagai sebuah paket (bukan direktori biasa).
3.  (Opsional) **Sub-paket**, yaitu direktori lain di dalam direktori paket yang juga berisi file `__init__.py` dan modul-modulnya sendiri.

**Contoh Struktur Direktori Paket:**

```
proyek_toko/
│
├── main.py                # Script utama yang menggunakan paket toko
│
└── toko/                  # <-- Direktori Paket Utama 'toko'
    │
    ├── __init__.py        # <-- Menandakan 'toko' sebagai paket
    │
    ├── produk.py          # Modul untuk data produk
    ├── keranjang.py       # Modul untuk keranjang belanja
    │
    └── pembayaran/        # <-- Sub-paket 'pembayaran'
        │
        ├── __init__.py    # <-- Menandakan 'pembayaran' sebagai sub-paket
        │
        ├── kartu_kredit.py # Modul proses kartu kredit
        └── transfer_bank.py # Modul proses transfer bank
```

### Mengimpor dari Paket

Anda mengimpor modul atau sub-paket dari dalam paket menggunakan notasi titik (`.`) yang mencerminkan struktur direktorinya.

```python
# Contoh isi file main.py (di luar direktori toko)

# Cara 1: Impor modul spesifik menggunakan path lengkap
import toko.produk
import toko.pembayaran.kartu_kredit

# Mengakses isinya
apel = toko.produk.get_info("Apel")
print(f"Info Apel: {apel}")
hasil_bayar = toko.pembayaran.kartu_kredit.proses_pembayaran(12345, 50000)
print(f"Hasil Bayar KK: {hasil_bayar}")


# Cara 2: Impor objek spesifik dari modul dalam paket
from toko.keranjang import tambah_item, lihat_keranjang
from toko.pembayaran.transfer_bank import buat_va

tambah_item("Pisang", 2)
keranjang = lihat_keranjang()
print(f"\nKeranjang saat ini: {keranjang}")
nomor_va = buat_va(101, 75000)
print(f"Nomor VA: {nomor_va}")


# Cara 3: Impor modul/sub-paket dengan alias
import toko.produk as prod
from toko.pembayaran import transfer_bank as tf

info_jeruk = prod.get_info("Jeruk")
print(f"\nInfo Jeruk (alias): {info_jeruk}")
hasil_tf = tf.cek_status(nomor_va)
print(f"Status Transfer: {hasil_tf}")

# Cara 4: Impor objek langsung dari paket/sub-paket (jika didefinisikan di __init__.py)
# Misal jika toko/__init__.py berisi 'from .produk import get_info'
# Maka bisa:
# from toko import get_info
# info_mangga = get_info("Mangga")
```

### File `__init__.py`

File `__init__.py`, meskipun bisa kosong, memiliki beberapa peran penting:

1.  **Penanda Paket:** Peran utamanya adalah memberi tahu Python bahwa direktori yang memuatnya harus diperlakukan sebagai paket. Tanpanya (di versi Python < 3.3), Python tidak akan mengenali direktori tersebut saat impor. Meskipun Python 3.3+ memperkenalkan "implicit namespace packages", tetap merupakan praktik terbaik untuk menyertakan `__init__.py` demi kejelasan dan kompatibilitas, serta untuk fungsionalitas di bawah ini.
2.  **Kode Inisialisasi Paket:** Kode yang Anda tulis di dalam `__init__.py` akan dieksekusi **satu kali** ketika paket atau salah satu modul/sub-paket di dalamnya pertama kali diimpor dalam sesi Python. Ini bisa digunakan untuk melakukan setup yang diperlukan oleh paket, seperti mengatur koneksi, memuat konfigurasi awal, atau mendefinisikan variabel level paket.
3.  **Membuat Antarmuka Paket Lebih Mudah:** Anda dapat mengimpor nama-nama (fungsi, kelas) dari sub-modul Anda ke dalam `__init__.py` paket. Ini memungkinkan pengguna paket mengimpor nama-nama tersebut langsung dari level paket atas, tanpa perlu mengetahui struktur internal sub-modulnya.
4.  **Mengontrol Impor Bintang (`__all__`):** Anda dapat mendefinisikan sebuah list bernama `__all__` di dalam `__init__.py` untuk secara eksplisit menentukan nama-nama (string nama modul, sub-paket, fungsi, kelas) apa saja yang akan diimpor ketika seseorang menggunakan sintaks `from nama_paket import *`. Jika `__all__` tidak didefinisikan, `from nama_paket import *` hanya akan mengimpor nama-nama yang didefinisikan *di dalam* `__init__.py` itu sendiri (termasuk yang diimpor ke dalamnya), tetapi *tidak* secara otomatis mengimpor sub-modul dari paket tersebut. Mendefinisikan `__all__` dianggap praktik yang baik jika Anda ingin mendukung `import *` untuk paket Anda, karena membuat API publik paket menjadi eksplisit.

```python
# Contoh isi file toko/__init__.py

print(f"Paket 'toko' sedang diinisialisasi...")

# Membuat fungsi/kelas dari submodul lebih mudah diakses
from .produk import get_info as info_produk
from .keranjang import tambah_item, lihat_keranjang
from . import pembayaran # Impor sub-paket pembayaran

# Mendefinisikan apa yang secara publik tersedia via 'from toko import *'
# (jika tidak didefinisikan, 'import *' hanya akan mengimpor 'info_produk',
# 'tambah_item', 'lihat_keranjang', dan 'pembayaran' yang didefinisikan/diimpor di atas)
__all__ = [
    'info_produk',      # Nama fungsi yang diimpor di atas
    'tambah_item',      # Nama fungsi lain
    'lihat_keranjang',  # Nama fungsi lain
    'pembayaran',       # Nama sub-paket yang diimpor
    'produk',           # Nama sub-modul (jika ingin diekspos juga)
    'keranjang'         # Nama sub-modul lain
]

# Variabel level paket
NAMA_TOKO = "Toko Python Jaya"

```

Dengan `__init__.py` di atas, pengguna bisa melakukan:

```python
import toko

# Mengakses nama yang diimpor di __init__.py
info = toko.info_produk("Sepatu")
toko.tambah_item("Kaos", 1)
print(toko.NAMA_TOKO)

# Mengakses sub-paket yang diimpor di __init__.py
toko.pembayaran.transfer_bank.buat_va(201, 1000)

# Jika __all__ didefinisikan, ini akan mengimpor nama-nama di __all__
# from toko import *
# ker = lihat_keranjang()
# info_baju = info_produk("Baju")
# print(pembayaran) # Sub-paket pembayaran juga terimpor
```

Tanda titik (`.`) dalam impor seperti `from .produk import get_info` disebut **relative import**. Ini digunakan *di dalam* paket untuk mengimpor modul atau sub-paket lain yang berada dalam paket yang sama atau direktori induknya (`..`).
*   `.modul`: Impor `modul` dari direktori saat ini (direktori `__init__.py`).
*   `..modul`: Impor `modul` dari direktori induk.
*   `.paket.modul`: Impor `modul` dari `paket` di direktori saat ini.

### Menginstal Paket Eksternal dengan `pip`

Salah satu kekuatan terbesar Python adalah ekosistem paket pihak ketiga yang sangat kaya, yang tersedia di **Python Package Index (PyPI)** ([https://pypi.org/](https://pypi.org/)). PyPI adalah repositori pusat untuk ribuan library dan framework yang dibuat oleh komunitas Python, mencakup hampir semua kebutuhan pemrograman.

Anda dapat menginstal, meng-upgrade, dan mengelola paket-paket ini menggunakan alat baris perintah bernama `pip`, yang biasanya sudah terinstal secara otomatis bersama Python versi modern.

**Operasi `pip` Umum (jalankan di terminal/command prompt):**

*   **Mencari Paket:** Anda bisa mencari paket langsung di situs web PyPI ([https://pypi.org/](https://pypi.org/)).
*   **Menginstal Paket:**
    ```bash
    # Format dasar: pip install nama_paket
    pip install requests    # Instal library populer untuk HTTP requests
    pip install pandas      # Instal library populer untuk analisis data
    pip install flask       # Instal microframework web Flask
    ```
    **Penting:** Sangat disarankan untuk menginstal paket ke dalam **lingkungan virtual (`venv`)** yang aktif, bukan ke instalasi Python global Anda (lihat bagian venv di bawah).
*   **Menginstal Versi Spesifik:**
    ```bash
    pip install requests==2.27.1  # Instal versi 2.27.1 tepat
    pip install numpy>=1.20.0     # Instal versi 1.20.0 atau yang lebih baru
    pip install django<4.0        # Instal versi Django terbaru sebelum 4.0
    ```
*   **Menginstal dari File Requirements:** (Sangat umum untuk proyek)
    ```bash
    pip install -r requirements.txt
    ```
*   **Melihat Paket Terinstal:**
    ```bash
    pip list       # Menampilkan semua paket di lingkungan saat ini
    pip freeze     # Menampilkan paket terinstal dlm format requirements.txt
    ```
*   **Melihat Informasi Detail Paket:**
    ```bash
    pip show nama_paket
    ```
*   **Meng-upgrade Paket:**
    ```bash
    pip install --upgrade nama_paket
    # atau
    pip install -U nama_paket
    ```
*   **Menghapus Paket:**
    ```bash
    pip uninstall nama_paket
    ```
    `pip` akan meminta konfirmasi sebelum menghapus.

### Lingkungan Virtual (`venv`)

Seperti yang telah disinggung di bagian Persiapan Lingkungan, penggunaan lingkungan virtual adalah praktik **fundamental** dan **sangat direkomendasikan** untuk *setiap* proyek Python.

**Mengapa `venv` Penting (Ringkasan):**

*   **Isolasi:** Menjaga dependensi (paket & versinya) untuk setiap proyek tetap terpisah. Proyek A bisa pakai `requests` versi 2.25, sementara Proyek B pakai `requests` versi 2.28, tanpa konflik.
*   **Reproduktibilitas:** Memastikan proyek dapat dijalankan di mesin lain (atau oleh rekan tim) dengan dependensi yang sama persis, menggunakan `requirements.txt`.
*   **Kebersihan Sistem:** Menjaga instalasi Python global Anda tetap bersih dari paket-paket spesifik proyek.

**Cara Menggunakan `venv` (Modul bawaan):**

1.  **Buat `venv`:** Di direktori utama proyek Anda, jalankan:
    ```bash
    python3 -m venv nama_lingkungan # Ganti 'nama_lingkungan' (umumnya 'venv' atau 'env')
    # Contoh: python3 -m venv venv
    ```
2.  **Aktifkan `venv`:**
    *   macOS/Linux: `source nama_lingkungan/bin/activate` (misal: `source venv/bin/activate`)
    *   Windows CMD: `.\nama_lingkungan\Scripts\activate.bat` (misal: `.\venv\Scripts\activate.bat`)
    *   Windows PowerShell: `.\nama_lingkungan\Scripts\Activate.ps1` (misal: `.\venv\Scripts\Activate.ps1`)
    Prompt terminal Anda akan berubah (biasanya diawali nama lingkungan).
3.  **Instal Paket:** Gunakan `pip install` seperti biasa. Paket akan terinstal *hanya* di dalam `venv` yang aktif.
    ```bash
    (venv) pip install flask requests Pillow
    ```
4.  **Bekerja:** Jalankan skrip Python Anda. Skrip akan menggunakan interpreter Python dan paket dari `venv` aktif.
5.  **Rekam Dependensi:** Setelah selesai menambah/mengubah dependensi:
    ```bash
    (venv) pip freeze > requirements.txt
    ```
    Commit `requirements.txt` ke Git, tapi **jangan commit** direktori `venv` itu sendiri (tambahkan `nama_lingkungan/` ke `.gitignore`).
6.  **Instal Dependensi (di tempat lain/oleh orang lain):**
    ```bash
    # Setelah membuat & mengaktifkan venv baru
    (venv) pip install -r requirements.txt
    ```
7.  **Deaktivasi `venv`:** Ketik `deactivate` di terminal.

Selalu biasakan bekerja di dalam lingkungan virtual yang aktif untuk proyek Python Anda.

---

## 8. Input/Output File (File I/O)

Hampir setiap program perlu berinteraksi dengan file di sistem penyimpanan, baik untuk membaca data konfigurasi, memproses input data, maupun menyimpan hasil output. Python menyediakan fungsi bawaan dan modul standar untuk melakukan operasi Input/Output (I/O) file dengan cara yang relatif mudah dan lintas platform.

### Membuka dan Menutup File (`open()`, `close()`)

Langkah pertama untuk bekerja dengan file adalah **membukanya** menggunakan fungsi bawaan `open()`. Fungsi ini mengembalikan **objek file** (juga disebut *file handle*), yang kemudian Anda gunakan untuk melakukan operasi baca atau tulis.

```python
# Sintaks dasar: open(nama_file, mode='r', encoding=None)

# Membuka file untuk dibaca (mode default 'r')
try:
    file_objek_baca = open("data_saya.txt", "r")
    # ... lakukan operasi baca ...
    print("File data_saya.txt berhasil dibuka untuk dibaca.")
    # PENTING: Tutup file setelah selesai!
    file_objek_baca.close()
    print("File data_saya.txt ditutup.")
except FileNotFoundError:
    print("Error: file data_saya.txt tidak ditemukan.")
except Exception as e:
    print(f"Error lain saat membuka file baca: {e}")


# Membuka file untuk ditulis (mode 'w')
# HATI-HATI: Mode 'w' akan MENGHAPUS isi file jika sudah ada!
# Jika file belum ada, file baru akan dibuat.
try:
    file_objek_tulis = open("output_saya.txt", "w")
    # ... lakukan operasi tulis ...
    print("\nFile output_saya.txt berhasil dibuka/dibuat untuk ditulis.")
    file_objek_tulis.close() # Tutup file!
    print("File output_saya.txt ditutup.")
except IOError as e: # IOError atau subclassnya seperti PermissionError
    print(f"Error saat membuka file tulis: {e}")


# Membuka file untuk ditambahkan (mode 'a' - append)
# Data baru akan ditambahkan di AKHIR file jika sudah ada.
# Jika file belum ada, file baru akan dibuat.
try:
    file_objek_tambah = open("log_aplikasi.log", "a")
    # ... lakukan operasi tulis (menambahkan) ...
    print("\nFile log_aplikasi.log berhasil dibuka/dibuat untuk ditambahkan.")
    file_objek_tambah.close() # Tutup file!
    print("File log_aplikasi.log ditutup.")
except IOError as e:
    print(f"Error saat membuka file tambah: {e}")

```

**Pentingnya Menutup File (`close()`):**
Menutup file secara eksplisit menggunakan `file_objek.close()` sangat penting karena:
*   **Flushing Buffer:** Memastikan semua data yang Anda tulis (yang mungkin masih ada di buffer memori sistem operasi) benar-benar tersimpan ke perangkat penyimpanan fisik (disk).
*   **Melepaskan Sumber Daya:** Melepaskan *file descriptor* atau *handle* yang digunakan oleh sistem operasi untuk file tersebut. Jika program Anda membuka terlalu banyak file tanpa menutupnya, Anda bisa kehabisan sumber daya ini.
*   **Memungkinkan Proses Lain:** Memastikan proses lain dapat mengakses file tersebut jika diperlukan (terutama di beberapa sistem operasi).

Namun, mengandalkan pemanggilan `close()` secara manual memiliki kelemahan:
*   Mudah lupa dipanggil.
*   Jika terjadi *exception* di antara `open()` dan `close()`, maka `close()` mungkin tidak akan pernah dieksekusi, menyebabkan file tetap terbuka dan potensi masalah di atas.

Oleh karena itu, cara yang **jauh lebih baik dan aman** adalah menggunakan **context manager** dengan pernyataan `with`.

### Mode Akses File

Parameter kedua pada `open()` adalah string *mode* yang menentukan bagaimana file akan dibuka dan operasi apa yang diizinkan. Mode-mode utama:

*   `'r'`: **Read (Baca)** - Default. Membuka file **hanya untuk dibaca**. Penunjuk file berada di awal file. Menimbulkan `FileNotFoundError` jika file tidak ada.
*   `'w'`: **Write (Tulis)** - Membuka file **hanya untuk ditulis**. **Menghapus (truncate) isi file menjadi kosong jika file sudah ada.** Membuat file baru jika tidak ada. Penunjuk file berada di awal file.
*   `'a'`: **Append (Tambah)** - Membuka file **hanya untuk ditulis**, menambahkan data baru di **akhir file**. Tidak menghapus isi file yang sudah ada. Membuat file baru jika tidak ada. Penunjuk file berada di akhir file.
*   `'x'`: **Exclusive Creation (Buat Eksklusif)** - Membuat file baru dan membukanya **hanya untuk ditulis**. Menimbulkan `FileExistsError` jika file sudah ada.
*   `'b'`: **Binary Mode (Mode Biner)** - Ditambahkan ke mode lain (misal `'rb'`, `'wb'`, `'ab'`, `'xb'`). Membuka file dalam mode biner. Digunakan untuk file yang **bukan teks biasa**, seperti gambar, audio, video, file executable, data terkompresi, dll. Data dibaca/ditulis sebagai objek `bytes`, bukan `str`. Encoding/decoding tidak dilakukan secara otomatis.
*   `'t'`: **Text Mode (Mode Teks)** - Default. Ditambahkan ke mode lain (misal `'rt'`, `'wt'`, `'at'`, `'xt'`). Membuka file dalam mode teks. Data dibaca/ditulis sebagai objek `str`. Python secara otomatis menangani **encoding** (mengubah bytes dari file menjadi string saat membaca) dan **decoding** (mengubah string menjadi bytes saat menulis) berdasarkan `encoding` yang ditentukan atau default sistem. Python juga menangani konversi karakter akhir baris (newline) antar sistem operasi secara otomatis (biasanya).
*   `'+'`: **Update (Baca dan Tulis)** - Ditambahkan ke mode lain (`'r+'`, `'w+'`, `'a+'`). Membuka file untuk operasi **baca dan tulis**.
    *   `'r+'`: Baca dan tulis. File harus ada. Penunjuk di awal.
    *   `'w+'`: Tulis dan baca. Menghapus isi file jika ada, membuat jika tidak ada. Penunjuk di awal.
    *   `'a+'`: Tambah dan baca. Membuat jika tidak ada. Penunjuk di akhir untuk tulis, tapi bisa dipindah untuk baca.

**Penting: Encoding Teks**
Saat bekerja dalam mode teks (`'t'` atau default), sangat penting untuk menentukan *encoding* teks yang benar, terutama jika file Anda mungkin berisi karakter di luar standar ASCII (misalnya huruf beraksen, karakter non-Latin, emoji). Encoding yang paling umum dan direkomendasikan secara luas saat ini adalah **UTF-8**.

```python
# Membuka file teks untuk dibaca dengan encoding UTF-8 (Sangat Direkomendasikan)
try:
    # Jika tidak pakai 'with', file harus ditutup manual
    f = open("file_utf8.txt", "r", encoding="utf-8")
    print("\nMembuka file_utf8.txt dengan encoding utf-8.")
    # ... baca dari f ...
    f.close()
except Exception as e:
    print(f"Error: {e}")

# Membuka file teks untuk ditulis dengan encoding UTF-8
try:
    f = open("output_utf8.txt", "w", encoding="utf-8")
    print("Membuka/membuat output_utf8.txt dengan encoding utf-8.")
    # ... tulis ke f ...
    f.close()
except Exception as e:
    print(f"Error: {e}")

# Membuka file gambar (biner) untuk dibaca
try:
    f_bin = open("logo.png", "rb") # Mode 'rb' (read binary)
    print("\nMembuka logo.png dalam mode biner.")
    # ... baca bytes dari f_bin ...
    f_bin.close()
except Exception as e:
    print(f"Error: {e}")
```
Jika Anda tidak menentukan `encoding` saat membuka file teks, Python akan menggunakan encoding default sistem (yang bisa berbeda antar OS atau bahkan antar konfigurasi mesin, misal `cp1252` di Windows bhs Inggris, `utf-8` di Linux/macOS modern). Mengandalkan default dapat menyebabkan `UnicodeDecodeError` atau `UnicodeEncodeError` jika file berisi karakter yang tidak valid untuk encoding default tersebut, atau data bisa rusak secara diam-diam. **Selalu tentukan `encoding="utf-8"` untuk file teks kecuali Anda tahu pasti file tersebut menggunakan encoding lain.**

### Menggunakan `with` untuk File Handling (Cara Terbaik!)

Pernyataan `with` menyediakan mekanisme **context management**. Ketika digunakan dengan `open()`, ia memastikan bahwa file akan **selalu ditutup secara otomatis** pada akhir blok `with`, **bahkan jika terjadi error** di dalam blok tersebut. Ini membuat kode lebih bersih, lebih aman, dan lebih mudah dibaca karena Anda tidak perlu khawatir memanggil `close()` secara manual.

```python
# Sintaks dasar with open:
# with open("nama_file", "mode", encoding="utf-8") as nama_variabel_file:
#     # Kode untuk bekerja dengan file (membaca/menulis)
#     # Gunakan 'nama_variabel_file' untuk akses objek file
# # Di sini, setelah keluar dari blok 'with', file DIJAMIN sudah tertutup.

# Contoh membaca file dengan 'with'
file_input = "data_penting.txt"
print(f"\nMencoba membaca '{file_input}' menggunakan 'with':")
try:
    with open(file_input, "r", encoding="utf-8") as f_in:
        print("  File berhasil dibuka.")
        konten = f_in.read() # Baca seluruh konten
        print(f"  Isi file ({len(konten)} karakter):")
        print(konten[:100] + "..." if len(konten) > 100 else konten) # Cetak maks 100 karakter
    # File f_in otomatis tertutup di sini.
    print("  Blok 'with' selesai, file sudah ditutup.")
except FileNotFoundError:
    print(f"  Error: file '{file_input}' tidak ditemukan.")
except UnicodeDecodeError:
    print(f"  Error: file '{file_input}' tidak bisa dibaca dengan encoding UTF-8.")
except Exception as e:
    print(f"  Error lain saat membaca: {e}")

# Contoh menulis file dengan 'with'
file_output = "laporan_baru.txt"
data_laporan = ["Laporan Penjualan\n", "="*20 + "\n", "Produk A: 10 unit\n", "Produk B: 5 unit\n"]
print(f"\nMencoba menulis ke '{file_output}' menggunakan 'with':")
try:
    with open(file_output, "w", encoding="utf-8") as f_out:
        print(f"  File '{file_output}' dibuka/dibuat untuk ditulis.")
        f_out.write("Dibuat pada: " + str(datetime.datetime.now()) + "\n\n")
        f_out.writelines(data_laporan) # Menulis list of strings
    # File f_out otomatis tertutup di sini.
    print(f"  Berhasil menulis ke '{file_output}', file sudah ditutup.")
except IOError as e:
    print(f"  Error saat menulis file: {e}")

```

**Kesimpulan: Selalu gunakan `with open(...)` saat bekerja dengan file di Python.** Ini adalah praktik standar industri dan cara paling Pythonic untuk menangani file.

### Membaca File

Setelah file dibuka dalam mode baca (atau mode update `+`), ada beberapa cara umum untuk membaca kontennya menggunakan metode objek file:

1.  **`read(size=-1)`:**
    *   Membaca dan mengembalikan konten file sebagai **satu string tunggal** (jika mode teks) atau **objek bytes tunggal** (jika mode biner).
    *   Jika argumen `size` diberikan dan positif, membaca dan mengembalikan paling banyak `size` karakter (mode teks) atau `size` byte (mode biner) dari posisi saat ini. Jika `size` tidak diberikan atau negatif, membaca **seluruh sisa file** dari posisi saat ini hingga akhir file (EOF - End Of File).
    *   **Hati-hati:** Menggunakan `read()` tanpa `size` pada file yang **sangat besar** dapat menghabiskan banyak memori sistem, karena seluruh isi file dimuat ke dalam memori sekaligus.

    ```python
    file_novel = "novel_panjang.txt"
    print(f"\nMembaca '{file_novel}' dengan read():")
    try:
        with open(file_novel, "r", encoding="utf-8") as f:
            # Baca 50 karakter pertama
            awal_novel = f.read(50)
            print(f"--- 50 Karakter Pertama --- \n{awal_novel}\n" + "-"*25)

            # Baca sisa file (bisa sangat besar!)
            sisa_novel = f.read()
            print(f"--- Sisa Novel ({len(sisa_novel)} karakter) ---")
            # Biasanya tidak dicetak semua jika besar
            print(sisa_novel[:100] + "...") # Cetak 100 karakter pertama dari sisa

            # Coba baca lagi setelah akhir file -> mengembalikan string kosong
            baca_lagi = f.read()
            print(f"\nHasil baca setelah EOF: '{baca_lagi}' (kosong)")

    except FileNotFoundError:
        print(f"Error: File '{file_novel}' tidak ditemukan.")
    ```

2.  **`readline(size=-1)`:**
    *   Membaca dan mengembalikan **satu baris** teks dari file, mulai dari posisi saat ini hingga dan termasuk karakter newline (`\n`) berikutnya (jika ada).
    *   Jika akhir file (EOF) tercapai dan tidak ada lagi baris yang bisa dibaca, mengembalikan **string kosong (`''`)**. Ini cara umum untuk mendeteksi akhir file saat membaca baris per baris dalam loop `while`.
    *   Jika argumen `size` positif diberikan, membaca paling banyak `size` karakter dari baris tersebut.

    ```python
    file_konfig = "settings.conf"
    print(f"\nMembaca '{file_konfig}' dengan readline():")
    try:
        with open(file_konfig, "r", encoding="utf-8") as f:
            print("--- Membaca baris per baris ---")
            baris_num = 1
            while True:
                baris = f.readline() # Baca satu baris
                if not baris: # Jika string kosong, berarti akhir file
                    print("--- Akhir File ---")
                    break # Keluar dari loop while
                # Proses baris (misal, hilangkan newline di akhir & spasi)
                print(f"Baris {baris_num}: {baris.strip()}")
                baris_num += 1
    except FileNotFoundError:
        print(f"Error: File '{file_konfig}' tidak ditemukan.")
    ```

3.  **`readlines()`:**
    *   Membaca **semua baris** yang tersisa dari file (dari posisi saat ini hingga EOF) dan mengembalikannya sebagai sebuah **list**, di mana setiap elemen dalam list adalah string yang mewakili satu baris (dan **masih menyertakan** karakter newline `\n` di akhir setiap baris).
    *   **Hati-hati:** Seperti `read()`, ini dapat memuat **seluruh isi file** ke dalam memori jika file sangat besar. Tidak disarankan untuk file besar.

    ```python
    file_daftar = "daftar_item.txt"
    print(f"\nMembaca '{file_daftar}' dengan readlines():")
    try:
        with open(file_daftar, "r", encoding="utf-8") as f:
            semua_baris_list = f.readlines()
            print(f"Hasil readlines() (tipe: {type(semua_baris_list)}):")
            print(semua_baris_list)

            # Memproses list baris
            print("\n--- Memproses list hasil readlines ---")
            for i, baris in enumerate(semua_baris_list):
                print(f"Item {i+1}: {baris.strip()}") # Hilangkan newline
    except FileNotFoundError:
        print(f"Error: File '{file_daftar}' tidak ditemukan.")
    ```

4.  **Iterasi Langsung atas Objek File (Cara Paling Pythonic & Efisien Memori):**
    *   Ini adalah cara yang paling **direkomendasikan** untuk membaca file teks **baris per baris**, terutama untuk file besar.
    *   Anda dapat menggunakan objek file langsung dalam loop `for`. Python secara otomatis akan membaca file satu baris pada satu waktu dan memberikan string baris tersebut (termasuk `\n`) ke variabel loop Anda. Ini **sangat efisien memori** karena tidak memuat seluruh file sekaligus.

    ```python
    file_log = "access.log"
    print(f"\nMembaca '{file_log}' dengan iterasi langsung:")
    try:
        with open(file_log, "r", encoding="utf-8") as f_log:
            print("--- Memproses log baris per baris ---")
            nomor_baris = 0
            for baris in f_log: # Iterasi langsung pada objek file 'f_log'
                nomor_baris += 1
                # Proses setiap baris
                # Contoh: Cari baris yang mengandung '404'
                if " 404 " in baris:
                    print(f"Baris {nomor_baris} (Error 404): {baris.strip()}")
            print(f"--- Selesai memproses {nomor_baris} baris ---")
    except FileNotFoundError:
        print(f"Error: File '{file_log}' tidak ditemukan.")
    except Exception as e:
        print(f"Error lain: {e}")
    ```
    Metode iterasi langsung ini biasanya merupakan pilihan terbaik untuk membaca file teks baris demi baris di Python.

### Menulis ke File

Untuk menulis ke file, Anda harus membukanya dalam mode yang mengizinkan penulisan (misalnya `'w'`, `'a'`, `'x'`, atau mode update `'+'`).

1.  **`write(string)`:**
    *   Menulis string yang diberikan ke file pada posisi penunjuk saat ini.
    *   **Penting:** Metode `write()` **tidak menambahkan karakter newline (`\n`) secara otomatis** di akhir string. Anda perlu menambahkannya secara eksplisit jika Anda ingin setiap `write()` menghasilkan baris baru.
    *   Mengembalikan jumlah karakter yang berhasil ditulis.

    ```python
    file_catatan = "catatan_harian.txt"
    print(f"\nMenulis ke '{file_catatan}' dengan write():")
    try:
        # Mode 'w' akan menimpa file jika sudah ada
        with open(file_catatan, "w", encoding="utf-8") as f:
            f.write("Catatan Hari Ini\n") # Tambahkan \n untuk baris baru
            f.write("================\n")
            f.write("Pagi: Meeting proyek A.\n")
            f.write("Siang: Makan siang dan coding.\n")
            f.write("Sore: Olahraga.") # Baris ini tidak akan diakhiri newline
            f.write(" Malam: Belajar Python.\n") # \n ditambahkan di sini

        print(f"Berhasil menulis ke '{file_catatan}'.")

        # Contoh menambahkan dengan mode 'a'
        with open(file_catatan, "a", encoding="utf-8") as f:
            f.write("\nTambahan: Jangan lupa beli susu!") # Tambah di baris baru

        print("Berhasil menambahkan ke file.")

    except IOError as e:
        print(f"Error menulis file: {e}")
    ```

2.  **`writelines(list_of_strings)`:**
    *   Menulis setiap string dari *iterable* (seperti list atau tuple) ke file secara berurutan.
    *   Sama seperti `write()`, **tidak menambahkan newline secara otomatis** antar elemen iterable. Anda harus memastikan string-string di dalam iterable sudah menyertakan karakter `\n` jika diperlukan.
    *   Biasanya lebih efisien daripada memanggil `write()` berulang kali dalam loop Python untuk menulis banyak baris dari list.

    ```python
    file_data = "data_angka.txt"
    list_angka_str = [str(i) + "\n" for i in range(1, 6)] # Buat list ['1\n', '2\n', ...]
    print(f"\nMenulis list {list_angka_str} ke '{file_data}' dengan writelines():")
    try:
        with open(file_data, "w", encoding="utf-8") as f:
            f.writelines(list_angka_str)
        print(f"Berhasil menulis list ke '{file_data}'.")
    except IOError as e:
        print(f"Error menulis file: {e}")
    ```

Ingat perbedaan utama antara mode `'w'` (write) dan `'a'` (append):
*   `'w'` (write): Memulai dari awal file. Jika file sudah ada, **isinya akan hilang (ditimpa)**.
*   `'a'` (append): Memulai dari akhir file. Jika file sudah ada, **data baru ditambahkan setelah isi yang lama**. Isi lama tetap ada.

### Bekerja dengan Path File (`os.path`, `pathlib`)

Seringkali Anda perlu memanipulasi path file (nama dan lokasi file/direktori di sistem file) sebelum membukanya, seperti menggabungkan nama direktori dan nama file, memeriksa keberadaan file, atau membuat direktori. Python menyediakan dua modul utama untuk ini:

1.  **Modul `os.path` (Tradisional):** Bagian dari modul `os`, berisi fungsi-fungsi yang beroperasi pada path file yang direpresentasikan sebagai **string**. Ini adalah cara klasik, tetapi kadang bisa sedikit kurang intuitif.
    *   `os.path.join(path1, path2, ...)`: Cara **terbaik dan aman** untuk menggabungkan satu atau lebih komponen path menjadi satu path string tunggal. Otomatis menggunakan pemisah direktori yang benar untuk sistem operasi (`/` di Linux/macOS, `\` di Windows). **Selalu gunakan ini** daripada menggabungkan string path secara manual dengan `+` dan `/` atau `\`.
    *   `os.path.exists(path)`: Mengembalikan `True` jika `path` (file atau direktori) ada, `False` jika tidak.
    *   `os.path.isfile(path)`: Mengembalikan `True` jika `path` ada dan merupakan file reguler.
    *   `os.path.isdir(path)`: Mengembalikan `True` jika `path` ada dan merupakan direktori.
    *   `os.path.basename(path)`: Mengembalikan nama file atau direktori terakhir dari path (misal, `file.txt` dari `/home/user/file.txt`).
    *   `os.path.dirname(path)`: Mengembalikan nama direktori yang berisi path (misal, `/home/user` dari `/home/user/file.txt`).
    *   `os.path.abspath(path)`: Mengembalikan path absolut dari `path` (misal, `/home/user/dokumen` dari `dokumen` jika direktori saat ini adalah `/home/user`).
    *   `os.path.splitext(path)`: Memisahkan path menjadi tuple `(root, ext)`, di mana `ext` adalah ekstensi file (termasuk titiknya).
    *   `os.getcwd()`: (Dari modul `os`) Mendapatkan direktori kerja saat ini (current working directory).
    *   `os.makedirs(path, exist_ok=False)`: (Dari modul `os`) Membuat direktori `path`. Akan membuat direktori induk jika perlu (seperti `mkdir -p`). Jika `exist_ok=True`, tidak akan error jika direktori sudah ada. Jika `False` (default), akan error jika sudah ada.
    *   `os.listdir(path)`: (Dari modul `os`) Mengembalikan list berisi nama-nama file dan direktori (sebagai string) yang ada di dalam direktori `path`.

    ```python
    import os

    nama_file_laporan = "laporan_bulanan.txt"
    dir_tujuan = "hasil_output"
    sub_dir = "januari"

    # Membuat path lengkap dengan aman
    path_sub_dir = os.path.join(dir_tujuan, sub_dir)
    path_lengkap_file = os.path.join(path_sub_dir, nama_file_laporan)

    print(f"\n--- Menggunakan os.path ---")
    print(f"Direktori Tujuan: {dir_tujuan}")
    print(f"Sub Direktori: {sub_dir}")
    print(f"Nama File: {nama_file_laporan}")
    print(f"Path Sub Direktori (join): {path_sub_dir}") # hasil_output/januari atau hasil_output\januari
    print(f"Path Lengkap File (join): {path_lengkap_file}")

    # Membuat direktori jika belum ada
    if not os.path.exists(path_sub_dir):
        print(f"Membuat direktori: {path_sub_dir}")
        os.makedirs(path_sub_dir, exist_ok=True) # exist_ok=True aman
    else:
        print(f"Direktori {path_sub_dir} sudah ada.")

    # Contoh menulis ke file dalam direktori tersebut
    try:
        with open(path_lengkap_file, "w", encoding="utf-8") as f:
            f.write("Ini isi laporan bulan Januari.\n")
        print(f"Berhasil menulis ke {path_lengkap_file}")
    except IOError as e:
        print(f"Gagal menulis file: {e}")

    # Cek properti path
    if os.path.exists(path_lengkap_file):
        print(f"\n'{path_lengkap_file}' ditemukan.")
        print(f"  Apakah file? {os.path.isfile(path_lengkap_file)}") # True
        print(f"  Apakah direktori? {os.path.isdir(path_lengkap_file)}") # False
        print(f"  Nama file (basename): {os.path.basename(path_lengkap_file)}") # laporan_bulanan.txt
        print(f"  Nama direktori (dirname): {os.path.dirname(path_lengkap_file)}") # hasil_output/januari
        nama_akar, ekstensi = os.path.splitext(path_lengkap_file)
        print(f"  Nama akar: {nama_akar}, Ekstensi: {ekstensi}") # .txt
    ```

2.  **Modul `pathlib` (Modern, Object-Oriented - Direkomendasikan):** Diperkenalkan di Python 3.4, `pathlib` menyediakan cara yang lebih modern, intuitif, dan berorientasi objek untuk bekerja dengan path file system. Anda bekerja dengan objek `Path` daripada string biasa. Objek `Path` memiliki banyak metode dan properti yang berguna, membuat kode manipulasi path seringkali lebih ringkas dan ekspresif.

    *   Membuat objek `Path`: `p = Path("nama/path/string")` atau `p = Path(var1, var2, ...)`
    *   Menggabungkan path: Gunakan operator slash (`/`). `new_path = path_obj / "subfolder" / "file.txt"` (lebih intuitif dari `os.path.join`).
    *   Properti: `.exists()`, `.is_file()`, `.is_dir()`, `.name` (basename), `.parent` (dirname), `.stem` (nama file tanpa ekstensi), `.suffix` (ekstensi file termasuk titik), `.resolve()` (path absolut), `.absolute()` (path absolut).
    *   Metode:
        *   `mkdir(parents=False, exist_ok=False)`: Membuat direktori. `parents=True` membuat direktori induk jika perlu. `exist_ok=True` tidak error jika sudah ada.
        *   `iterdir()`: Menghasilkan iterator untuk item (file/direktori) di dalam direktori `Path` ini.
        *   `glob(pattern)`: Mencari file/direktori yang cocok dengan pola (misal `*.txt`).
        *   `read_text(encoding=None, errors=None)`: Cara ringkas membaca seluruh isi file teks (menangani open, read, close).
        *   `write_text(data, encoding=None, errors=None)`: Cara ringkas menulis string ke file teks (menangani open, write, close).
        *   `read_bytes()`: Membaca seluruh file biner.
        *   `write_bytes(data)`: Menulis data bytes ke file biner.
        *   `rename(target)`: Mengganti nama atau memindahkan file/direktori.
        *   `unlink(missing_ok=False)`: Menghapus file. `missing_ok=True` tidak error jika file tidak ada.
        *   `rmdir()`: Menghapus direktori kosong.

    ```python
    from pathlib import Path
    import datetime

    nama_file_laporan = "laporan_pathlib.txt"
    # Membuat objek Path
    dir_tujuan = Path("hasil_pathlib")
    sub_dir = Path("februari")

    # Menggabungkan path dengan operator /
    path_sub_dir = dir_tujuan / sub_dir
    path_lengkap_file = path_sub_dir / nama_file_laporan

    print(f"\n--- Menggunakan pathlib ---")
    print(f"Path Sub Direktori (objek): {path_sub_dir}")
    print(f"Path Lengkap File (objek): {path_lengkap_file}")
    print(f"Tipe path_lengkap_file: {type(path_lengkap_file)}") # <class 'pathlib.PosixPath'> atau <class 'pathlib.WindowsPath'>

    # Membuat direktori (lebih ringkas)
    # mkdir() pada Path object
    print(f"Membuat direktori (jika belum ada): {path_sub_dir}")
    path_sub_dir.mkdir(parents=True, exist_ok=True)

    # Menulis ke file dengan mudah (menangani open/close)
    try:
        isi_laporan = f"Laporan bulan Februari.\nDibuat pada: {datetime.datetime.now()}\n"
        karakter_ditulis = path_lengkap_file.write_text(isi_laporan, encoding="utf-8")
        print(f"Berhasil menulis {karakter_ditulis} karakter ke {path_lengkap_file}")
    except IOError as e:
        print(f"Gagal menulis (pathlib): {e}")

    # Membaca teks dari file dengan mudah
    try:
        konten_dibaca = path_lengkap_file.read_text(encoding="utf-8")
        print(f"\nIsi dibaca dari {path_lengkap_file}:\n{konten_dibaca}")
    except FileNotFoundError:
        print(f"Error: {path_lengkap_file} tidak ditemukan saat membaca.")
    except IOError as e:
        print(f"Gagal membaca (pathlib): {e}")

    # Cek properti Path
    if path_lengkap_file.exists():
        print(f"\nProperti '{path_lengkap_file}':")
        print(f"  Apakah file? {path_lengkap_file.is_file()}") # True
        print(f"  Apakah direktori? {path_lengkap_file.is_dir()}") # False
        print(f"  Nama file: {path_lengkap_file.name}") # laporan_pathlib.txt
        print(f"  Direktori induk: {path_lengkap_file.parent}") # hasil_pathlib/februari
        print(f"  Nama file tanpa ekstensi: {path_lengkap_file.stem}") # laporan_pathlib
        print(f"  Ekstensi: {path_lengkap_file.suffix}") # .txt
        print(f"  Path absolut: {path_lengkap_file.resolve()}")

    # Iterasi isi direktori
    print(f"\nIsi direktori {dir_tujuan}:")
    for item in dir_tujuan.iterdir():
        jenis = "Direktori" if item.is_dir() else "File"
        print(f"- {item.name} ({jenis})")
    ```

    **`pathlib` umumnya lebih disukai** untuk kode Python modern karena API-nya yang berorientasi objek, lebih intuitif (terutama operator `/`), dan seringkali membuat kode manipulasi path menjadi lebih bersih dan mudah dibaca dibandingkan `os.path`.

### Bekerja dengan Format File Umum

Selain file teks biasa (`.txt`) atau file biner (`.jpg`, `.zip`), Anda akan sering berhadapan dengan format file terstruktur yang digunakan untuk pertukaran data, seperti CSV dan JSON. Python Standard Library menyediakan modul khusus untuk memudahkan pekerjaan dengan format-format ini.

1.  **CSV (Comma Separated Values) (`csv` module):**
    Format CSV adalah cara umum untuk menyimpan data tabel (seperti spreadsheet) dalam file teks biasa. Setiap baris mewakili satu record data, dan nilai-nilai dalam baris dipisahkan oleh karakter pemisah (delimiter), yang paling umum adalah koma (`,`), tetapi bisa juga titik koma (`;`), tab (`\t`), atau lainnya. Baris pertama seringkali berisi nama kolom (header).

    Modul `csv` membantu membaca dan menulis file CSV dengan benar, menangani masalah seperti nilai yang mengandung koma atau karakter newline (biasanya dengan mengapit nilai tersebut dalam tanda kutip).

    ```python
    import csv
    import os

    nama_file_csv = "data_mahasiswa.csv"
    dir_csv = Path("data_output_csv")
    path_csv = dir_csv / nama_file_csv

    # Membuat direktori
    dir_csv.mkdir(exist_ok=True)

    # Data contoh untuk ditulis
    data_untuk_csv = [
        ['NIM', 'Nama', 'IPK', 'Kota Asal'], # Baris Header
        ['101', 'Budi', '3.75', 'Jakarta'],
        ['102', 'Ani', '3.90', 'Bandung,"Jawa Barat"'], # Nilai berisi koma
        ['103', 'Citra', '3.55', 'Surabaya']
    ]

    # --- Menulis ke file CSV ---
    print(f"\nMenulis data ke '{path_csv}'...")
    try:
        # 'newline=""' penting untuk mencegah baris kosong ekstra di Windows
        with open(path_csv, 'w', newline='', encoding='utf-8') as file_csv:
            # Membuat objek writer
            # writer = csv.writer(file_csv) # Default delimiter koma
            writer = csv.writer(file_csv, delimiter=';', quotechar='"', quoting=csv.QUOTE_MINIMAL)
            # delimiter=';' -> gunakan titik koma sebagai pemisah
            # quotechar='"' -> gunakan kutip ganda untuk mengapit
            # quoting=csv.QUOTE_MINIMAL -> hanya kutip jika perlu (misal ada delimiter/quotechar di nilai)

            # Menulis semua baris data sekaligus
            writer.writerows(data_untuk_csv)

            # Atau menulis baris per baris
            # writer.writerow(['NIM', 'Nama', 'IPK']) # Header
            # writer.writerow(['101', 'Budi', 3.75])
            # writer.writerow(['102', 'Ani', 3.90])

        print(f"Berhasil menulis data ke {path_csv}")
    except IOError as e:
        print(f"Gagal menulis CSV: {e}")
    except csv.Error as e:
        print(f"CSV Error saat menulis: {e}")


    # --- Membaca dari file CSV ---
    print(f"\nMembaca data dari '{path_csv}'...")
    data_dibaca_csv = []
    try:
        with open(path_csv, 'r', newline='', encoding='utf-8') as file_csv:
            # Membuat objek reader (sesuaikan delimiter jika saat tulis diubah)
            reader = csv.reader(file_csv, delimiter=';', quotechar='"')

            # Membaca header (jika ada)
            try:
                header = next(reader) # Baca baris pertama sebagai header
                print(f"Header CSV: {header}")
            except StopIteration:
                print("File CSV kosong.")
                header = []

            # Iterasi sisa baris data
            print("Data:")
            for baris in reader: # Setiap 'baris' adalah list of strings
                print(f"  {baris}")
                data_dibaca_csv.append(baris)

    except FileNotFoundError:
        print(f"Error: File '{path_csv}' tidak ditemukan.")
    except csv.Error as e:
        print(f"CSV Error saat membaca: {e}")
    except Exception as e:
        print(f"Gagal membaca CSV: {e}")


    # --- Membaca CSV sebagai dictionary (DictReader) ---
    # Berguna jika file punya header, setiap baris jadi dict {header: nilai}
    print(f"\nMembaca '{path_csv}' sebagai Dictionary...")
    data_dict_csv = []
    try:
        with open(path_csv, 'r', newline='', encoding='utf-8') as file_csv:
            # Membuat DictReader (otomatis pakai baris pertama sbg kunci)
            # Sesuaikan delimiter jika perlu
            reader = csv.DictReader(file_csv, delimiter=';', quotechar='"')

            print("Data (sebagai dict):")
            for row_dict in reader: # Setiap row_dict adalah dictionary
                print(f"  {row_dict}")
                # Anda bisa akses nilai pakai kunci header
                print(f"    Nama: {row_dict['Nama']}, IPK: {row_dict['IPK']}")
                data_dict_csv.append(row_dict)

    except FileNotFoundError:
        print(f"Error: File '{path_csv}' tidak ditemukan.")
    except Exception as e:
        print(f"Gagal membaca CSV (DictReader): {e}")

    ```

2.  **JSON (JavaScript Object Notation) (`json` module):**
    JSON adalah format pertukaran data berbasis teks yang ringan, mudah dibaca manusia, dan mudah diproses mesin. Sangat populer digunakan dalam API web dan file konfigurasi. Strukturnya mirip dengan objek JavaScript dan sangat mudah dipetakan ke struktur data Python (dan sebaliknya).

    *   Objek JSON (`{...}`) -> Dictionary Python (`dict`)
    *   Array JSON (`[...]`) -> List Python (`list`)
    *   String JSON (`"..."`) -> String Python (`str`)
    *   Angka JSON (`123`, `3.14`, `-5e2`) -> Angka Python (`int`, `float`)
    *   Boolean JSON (`true`, `false`) -> Boolean Python (`True`, `False`)
    *   Null JSON (`null`) -> None Python (`None`)

    Modul `json` menyediakan fungsi utama:
    *   `json.dump(obj, fp, indent=None, ...)`: Menulis (serialize) objek Python `obj` ke file-like object `fp` (yang dibuka dalam mode tulis teks) sebagai string JSON. `indent` (misal `4`) digunakan untuk *pretty-printing* (membuat format JSON lebih rapi dengan indentasi).
    *   `json.dumps(obj, indent=None, ...)`: Mengembalikan (serialize) objek Python `obj` sebagai **string** JSON (dump string).
    *   `json.load(fp)`: Membaca (deserialize) string JSON dari file-like object `fp` (yang dibuka dalam mode baca teks) dan mengembalikannya sebagai objek Python yang sesuai.
    *   `json.loads(s)`: Membaca (deserialize) string JSON `s` dan mengembalikannya sebagai objek Python (load string).

    ```python
    import json
    from pathlib import Path

    nama_file_json = "data_produk.json"
    dir_json = Path("data_output_json")
    path_json = dir_json / nama_file_json

    # Membuat direktori
    dir_json.mkdir(exist_ok=True)

    # Data Python (contoh: dictionary kompleks)
    data_produk_py = {
        "productId": "P001-XYZ",
        "namaProduk": "Laptop Gaming Super",
        "harga": 25500000.50,
        "tersedia": True,
        "tags": ["gaming", "laptop", "high-end", None], # List bisa berisi None
        "spesifikasi": { # Dictionary bersarang
            "cpu": "Intel Core i9 Gen 13",
            "ramGB": 32,
            "storage": {
                "tipe": "NVMe SSD",
                "kapasitasGB": 1024
            },
            "fitur": ["RGB Keyboard", "Layar 144Hz"] # List dalam dict
        },
        "rating": None # Nilai bisa None
    }

    # --- Menulis objek Python ke file JSON (Serialization) ---
    print(f"\nMenulis data Python ke '{path_json}'...")
    try:
        with open(path_json, 'w', encoding='utf-8') as f_json:
            # json.dump(objek_python, file_objek, ...)
            # indent=4 membuat output JSON lebih mudah dibaca manusia
            json.dump(data_produk_py, f_json, indent=4, ensure_ascii=False)
            # ensure_ascii=False penting jika data Anda mungkin punya karakter non-ASCII
        print(f"Berhasil menulis data ke {path_json}")
    except IOError as e:
        print(f"Gagal menulis JSON ke file: {e}")
    except TypeError as e:
        print(f"Gagal serialize JSON (tipe data tidak didukung?): {e}")

    # --- Membaca data dari file JSON ke objek Python (Deserialization) ---
    print(f"\nMembaca data dari '{path_json}'...")
    data_dibaca_py = None
    try:
        with open(path_json, 'r', encoding='utf-8') as f_json:
            # json.load(file_objek)
            data_dibaca_py = json.load(f_json)

        print(f"Berhasil membaca data dari JSON. Tipe data: {type(data_dibaca_py)}")
        # Sekarang data_dibaca_py adalah dictionary Python
        if data_dibaca_py:
            print(f"Nama Produk: {data_dibaca_py['namaProduk']}")
            print(f"CPU: {data_dibaca_py['spesifikasi']['cpu']}")
            print(f"Tag kedua: {data_dibaca_py['tags'][1]}")
            print(f"Tipe Storage: {data_dibaca_py.get('spesifikasi',{}).get('storage',{}).get('tipe', 'N/A')}")

    except FileNotFoundError:
        print(f"Error: File '{path_json}' tidak ditemukan.")
    except json.JSONDecodeError as e:
        # Terjadi jika format file JSON tidak valid
        print(f"Error: Format JSON tidak valid dalam file: {e}")
    except Exception as e:
        print(f"Gagal membaca JSON dari file: {e}")

    # --- Konversi antara objek Python dan STRING JSON ---
    print("\n--- Konversi ke/dari String JSON ---")
    # Objek Python -> String JSON (json.dumps)
    try:
        json_string = json.dumps(data_produk_py, indent=2, ensure_ascii=False)
        print("Data Produk sebagai String JSON:")
        print(json_string)
    except TypeError as e:
        print(f"Gagal dumps ke string JSON: {e}")

    # String JSON -> Objek Python (json.loads)
    json_string_baru = '{"kota": "Yogyakarta", "provinsi": "DIY", "populasi": 422731, "aktif": true, "area_kode": null}'
    try:
        data_kota_py = json.loads(json_string_baru)
        print("\nObjek Python dari String JSON baru:")
        print(data_kota_py)
        print(f"Kota: {data_kota_py['kota']}, Aktif: {data_kota_py['aktif']}")
    except json.JSONDecodeError as e:
        print(f"Gagal loads dari string JSON: {e}")
    ```

## 9. Penanganan Error dan Exceptions

Saat menulis program, kesalahan (error) tidak dapat dihindari. Python memiliki mekanisme yang kuat untuk menangani error yang terjadi saat runtime (selama program berjalan), yang dikenal sebagai **exceptions**. Menangani exceptions dengan benar membuat program Anda lebih tangguh (robust) dan tidak mudah crash, serta dapat memberikan umpan balik yang berguna kepada pengguna atau melakukan tindakan pemulihan.

### Syntax Errors vs Exceptions

Penting untuk membedakan dua jenis error utama:

1.  **Syntax Errors (Kesalahan Sintaks):** Terjadi ketika kode Anda tidak mengikuti aturan tata bahasa (sintaks) Python. Interpreter Python tidak dapat memahami atau mem-parsing kode tersebut. Program **tidak akan bisa dijalankan sama sekali** sampai kesalahan sintaks diperbaiki.
    ```python
    # Contoh Syntax Error (lupa titik dua setelah if)
    # angka = 10
    # if angka > 5
    #   print("Lebih besar")
    # SyntaxError: expected ':'

    # Contoh Syntax Error (indentasi salah)
    # def fungsi_salah():
    # print("Indentasi salah")
    # IndentationError: expected an indented block
    ```
2.  **Exceptions (Pengecualian):** Terjadi **selama eksekusi program** (runtime) meskipun sintaks kodenya sudah benar. Exceptions muncul ketika terjadi sesuatu yang tidak terduga atau operasi yang tidak valid, seperti mencoba membagi dengan nol, mengakses indeks list yang tidak ada, atau membuka file yang tidak ditemukan. Jika exception tidak ditangani, program akan berhenti (crash) dan menampilkan *traceback* (jejak eksekusi yang menunjukkan di mana error terjadi).

    ```python
    # Contoh Exception (berpotensi terjadi saat runtime)
    try:
      hasil = 10 / 0 # ZeroDivisionError
    except ZeroDivisionError:
      print("Exception: Tidak bisa membagi dengan nol!")

    try:
      list_ku = [1, 2, 3]
      print(list_ku[5]) # IndexError
    except IndexError:
      print("Exception: Indeks di luar jangkauan!")
    ```
Bagian ini fokus pada penanganan *exceptions*.

### Exceptions Umum

Python memiliki banyak jenis exception bawaan. Beberapa yang paling umum Anda temui:

*   `TypeError`: Operasi atau fungsi diterapkan pada objek dengan tipe yang tidak sesuai (misal, `len(123)` atau `"usia: " + 25`).
*   `ValueError`: Fungsi menerima argumen dengan tipe yang benar, tetapi nilainya tidak sesuai (misal, `int("halo")`).
*   `NameError`: Mencoba menggunakan variabel atau nama fungsi yang belum didefinisikan.
*   `IndexError`: Mencoba mengakses indeks di luar jangkauan pada urutan (list, tuple, string).
*   `KeyError`: Mencoba mengakses kunci yang tidak ada dalam dictionary.
*   `FileNotFoundError`: Mencoba membuka file yang tidak ada dalam mode baca.
*   `ZeroDivisionError`: Mencoba melakukan pembagian atau modulo dengan nol.
*   `AttributeError`: Mencoba mengakses atribut atau metode yang tidak ada pada suatu objek (misal, `list_ku.appendx(1)` - harusnya `append`).
*   `ImportError`: Gagal mengimpor modul (bisa karena tidak ditemukan atau ada error di dalam modul saat diimpor).
*   `IOError` (dan subclass seperti `PermissionError`): Error terkait operasi Input/Output, termasuk masalah izin file.
*   `MemoryError`: Program kehabisan memori.
*   `RecursionError`: Melebihi batas kedalaman rekursi.

### Blok `try...except`

Cara utama untuk menangani exceptions adalah menggunakan blok `try...except`.

**Sintaks Dasar:**

```python
try:
    # Kode yang berpotensi menimbulkan exception
    # Letakkan operasi yang "berisiko" di sini
    kode_yang_mungkin_error()
except NamaExceptionTertentu:
    # Kode yang dijalankan HANYA JIKA exception
    # 'NamaExceptionTertentu' terjadi di blok try
    print("Terjadi exception spesifik!")
    # Lakukan tindakan penanganan, log error, beri pesan, dll.
except ExceptionLain:
    # Blok except lain untuk exception berbeda
    print("Terjadi exception lain!")
# ... bisa ada blok except lain ...
```

**Alur Kerja:**
1.  Kode di dalam blok `try` dieksekusi baris per baris.
2.  Jika **tidak ada exception** terjadi selama eksekusi blok `try`, maka semua blok `except` akan **dilewati**, dan eksekusi dilanjutkan setelah seluruh blok `try...except`.
3.  Jika **terjadi exception** di dalam blok `try`, eksekusi di blok `try` **langsung berhenti** pada titik terjadinya error.
4.  Python kemudian mencari blok `except` yang cocok dengan tipe exception yang terjadi. Pencarian dilakukan dari atas ke bawah.
5.  Jika ditemukan `except` yang cocok, kode di dalam blok `except` tersebut **dieksekusi**. Setelah blok `except` selesai, eksekusi dilanjutkan setelah seluruh blok `try...except`.
6.  Jika **tidak ada `except` yang cocok** yang ditemukan, exception tersebut tidak tertangani (unhandled exception). Program akan berhenti dan menampilkan traceback (perilaku default jika tidak ada `try...except` sama sekali).

### Menangkap Exceptions Spesifik

Sangat disarankan untuk menangkap exception **sespesifik mungkin** daripada menggunakan `except` kosong (`except:`) atau `except Exception:`.

**Mengapa?**
*   **Lebih Jelas:** Anda tahu persis error apa yang Anda tangani.
*   **Tidak Menyembunyikan Bug:** Menangkap `Exception` atau `except:` kosong dapat secara tidak sengaja menangkap error yang tidak Anda antisipasi (seperti `NameError` karena typo, atau bahkan `KeyboardInterrupt` dari Ctrl+C), membuat debugging lebih sulit.
*   **Penanganan Berbeda:** Memungkinkan Anda memberikan penanganan yang berbeda untuk jenis error yang berbeda.

```python
def bagi_dua_angka(a, b):
  try:
    a_int = int(a)
    b_int = int(b)
    hasil = a_int / b_int
    print(f"Hasil {a_int} / {b_int} = {hasil}")
  except ValueError:
    # Menangani jika konversi int() gagal
    print("Error: Input harus berupa angka integer!")
  except ZeroDivisionError:
    # Menangani jika pembagian dengan nol
    print("Error: Tidak bisa membagi dengan nol!")
  except Exception as e:
    # Menangkap exception lain yang tidak terduga (kurang spesifik)
    # 'as e' menyimpan objek exception ke variabel 'e'
    print(f"Terjadi error tak terduga: {e}")
    print(f"Tipe error: {type(e)}")

bagi_dua_angka("10", "2")   # Sukses
bagi_dua_angka("sepuluh", "2") # ValueError
bagi_dua_angka("10", "0")   # ZeroDivisionError
# Jika ada error lain, misal NameError di dalam try, akan ditangkap 'except Exception'
```

Anda dapat menyimpan objek exception yang tertangkap ke dalam variabel menggunakan `as nama_variabel` (misal `except ValueError as ve:`). Objek ini berisi informasi lebih detail tentang error.

### Menangkap Multiple Exceptions

Ada dua cara untuk menangani beberapa jenis exception dengan logika yang sama:

1.  **Tuple dalam satu `except`:**
    ```python
    angka_str = input("Masukkan angka atau tekan Enter: ")
    try:
        angka = int(angka_str)
        hasil_kebalikan = 1 / angka
        print(f"Kebalikan dari {angka} adalah {hasil_kebalikan}")
    except (ValueError, ZeroDivisionError) as e:
        # Menangani ValueError (jika input bukan int)
        # ATAU ZeroDivisionError (jika input 0)
        print(f"Input tidak valid atau nol: {e}")
    ```
2.  **Beberapa blok `except`:** (Seperti contoh `bagi_dua_angka` di atas) Gunakan ini jika Anda memerlukan logika penanganan yang berbeda untuk setiap jenis exception.

### Klausa `else`

Blok `else` opsional dapat ditambahkan setelah semua blok `except`. Kode di dalam `else` akan dieksekusi **hanya jika blok `try` selesai tanpa menimbulkan exception apa pun**.

Ini berguna untuk meletakkan kode yang seharusnya hanya berjalan jika operasi "berisiko" di `try` berhasil.

```python
file_path = "mungkin_ada.txt"
try:
    print(f"\nMencoba membuka '{file_path}'...")
    f = open(file_path, "r", encoding="utf-8")
except FileNotFoundError:
    print("File tidak ditemukan. Membuat file baru.")
    # Mungkin logika untuk membuat file default di sini
except Exception as e:
    print(f"Error lain saat membuka: {e}")
else:
    # Blok ini HANYA jalan jika try berhasil (file ditemukan & bisa dibuka)
    print("File berhasil dibuka! Membaca konten...")
    with f: # Gunakan with di sini untuk menutup otomatis
        konten = f.read()
        print(f"Isi file:\n{konten[:50]}...")
    print("Selesai memproses file.")
```

### Klausa `finally`

Blok `finally` opsional akan **selalu dieksekusi** setelah blok `try`, `except`, dan `else`, terlepas dari apa yang terjadi:
*   Apakah exception terjadi atau tidak.
*   Apakah exception yang terjadi ditangkap atau tidak.
*   Apakah blok `try`, `except`, atau `else` diakhiri dengan `return`, `break`, atau `continue`.

`finally` sangat penting untuk **tindakan pembersihan (cleanup)** yang harus selalu dilakukan, seperti menutup file (meskipun `with` lebih baik untuk ini), menutup koneksi jaringan/database, melepaskan kunci (lock), dll.

```python
koneksi_db = None # Anggap ini objek koneksi database
try:
    print("\nMencoba membuka koneksi database...")
    # Anggap kode ini bisa error (misal, server down)
    koneksi_db = "Koneksi Berhasil Dibuka" # Simulasi
    print(koneksi_db)

    # Anggap operasi query bisa error
    query_hasil = 10 / 1 # Operasi sukses
    # query_hasil = 10 / 0 # Operasi gagal (ZeroDivisionError)
    print(f"Hasil query: {query_hasil}")

except ZeroDivisionError:
    print("Error dalam operasi database!")

finally:
    # Blok ini akan SELALU dijalankan
    print("Blok finally dieksekusi.")
    if koneksi_db:
        print("Menutup koneksi database...")
        # Kode untuk menutup koneksi_db.close()
        koneksi_db = None # Reset variabel
    else:
        print("Tidak ada koneksi aktif untuk ditutup.")
```

**Urutan Eksekusi Lengkap:** `try` -> (jika error) `except` -> (jika no error) `else` -> `finally`.

### Membangkitkan Exceptions (`raise`)

Anda dapat secara sengaja membangkitkan (memunculkan) exception menggunakan pernyataan `raise`. Ini berguna ketika:
*   Anda mendeteksi kondisi error dalam kode Anda (misalnya, input tidak valid dari pengguna).
*   Anda ingin mengubah tipe exception yang ditangkap menjadi tipe lain yang lebih spesifik untuk aplikasi Anda.
*   Anda ingin meneruskan (re-raise) exception yang baru saja ditangkap setelah melakukan beberapa tindakan logging atau cleanup.

```python
def validasi_umur(umur):
  """Memvalidasi umur, raise ValueError jika tidak valid."""
  try:
      umur_int = int(umur)
      if umur_int < 0:
          # Membangkitkan ValueError secara manual
          raise ValueError("Umur tidak boleh negatif.")
      elif umur_int > 120:
          raise ValueError("Umur terlalu tinggi, tidak realistis.")
      else:
          print(f"Umur {umur_int} valid.")
          return umur_int
  except ValueError as ve: # Menangkap ValueError dari int() atau dari raise
      print(f"Error Validasi: {ve}")
      # Bisa juga re-raise exception setelah logging
      # print("Mencatat error validasi umur...")
      # raise # Re-raise exception asli (ve)
      return None # Atau kembalikan nilai penanda

validasi_umur("25")      # Valid
validasi_umur("-5")     # Error Validasi: Umur tidak boleh negatif.
validasi_umur("tua")    # Error Validasi: invalid literal for int() with base 10: 'tua'
validasi_umur("200")    # Error Validasi: Umur terlalu tinggi, tidak realistis.

# Re-raise contoh (kurang umum tapi bisa)
def proses_data_sensitif(data):
    try:
        # ... operasi yang mungkin KeyError ...
        nilai = data['kunci_rahasia']
        print("Proses berhasil")
    except KeyError:
        print("Log: Akses kunci sensitif gagal.")
        # Ubah ke exception yang lebih umum atau spesifik aplikasi
        raise RuntimeError("Gagal memproses data sensitif karena kunci hilang.")

try:
    proses_data_sensitif({})
except RuntimeError as re:
    print(f"Ditangkap di luar: {re}")
```

### Membuat Custom Exceptions

Untuk error yang sangat spesifik pada logika aplikasi Anda, seringkali lebih baik membuat kelas exception kustom Anda sendiri. Ini membuat penanganan error lebih terstruktur dan jelas. Cukup buat kelas baru yang mewarisi dari kelas `Exception` bawaan (atau subclass exception lain yang lebih relevan).

```python
# Mendefinisikan exception kustom
class SaldoTidakCukupError(Exception):
  """Exception kustom yang dibangkitkan saat saldo tidak mencukupi."""
  def __init__(self, saldo_sekarang, jumlah_diminta):
    self.saldo_sekarang = saldo_sekarang
    self.jumlah_diminta = jumlah_diminta
    # Pesan error standar
    message = f"Saldo tidak cukup. Saldo saat ini: {saldo_sekarang}, diminta: {jumlah_diminta}"
    # Panggil __init__ dari superclass (Exception) dengan pesan
    super().__init__(message)

# Fungsi yang mungkin membangkitkan exception kustom
def tarik_tunai(saldo, jumlah):
  print(f"\nMencoba tarik {jumlah} dari saldo {saldo}")
  if jumlah <= 0:
    raise ValueError("Jumlah penarikan harus positif.")
  if jumlah > saldo:
    # Bangkitkan exception kustom kita
    raise SaldoTidakCukupError(saldo, jumlah)
  else:
    saldo_baru = saldo - jumlah
    print(f"Penarikan berhasil. Saldo baru: {saldo_baru}")
    return saldo_baru

# Menangani exception kustom
saldo_akun = 500
try:
  saldo_akun = tarik_tunai(saldo_akun, 200) # Berhasil
  saldo_akun = tarik_tunai(saldo_akun, 400) # Gagal (SaldoTidakCukupError)
  saldo_akun = tarik_tunai(saldo_akun, 100) # Baris ini tidak akan jalan
except SaldoTidakCukupError as stce:
  print(f"Gagal tarik tunai: {stce}")
  print(f"  Detail - Saldo: {stce.saldo_sekarang}, Diminta: {stce.jumlah_diminta}")
except ValueError as ve:
  print(f"Input tidak valid: {ve}")
```

### Assertion (`assert`)

Pernyataan `assert` digunakan sebagai alat bantu debugging untuk memeriksa kondisi yang *seharusnya* selalu benar dalam program Anda. Jika kondisi setelah `assert` dievaluasi menjadi `False`, maka `AssertionError` akan dibangkitkan.

**Sintaks:** `assert kondisi, pesan_error_opsional`

```python
def hitung_diskon(harga, persentase):
  """Menghitung harga setelah diskon."""
  # Assert digunakan untuk memeriksa kondisi internal/logika programmer
  # Bukan untuk validasi input pengguna (gunakan if/raise untuk itu)
  assert 0 <= persentase <= 1, "Persentase diskon harus antara 0 dan 1"

  harga_diskon = harga * (1 - persentase)
  # Contoh assert lain: harga diskon tidak boleh negatif
  assert harga_diskon >= 0, "Harga setelah diskon tidak boleh negatif"
  return harga_diskon

try:
  print(f"Diskon 100, 10%: {hitung_diskon(100, 0.1)}")
  # print(f"Diskon 50, 110%: {hitung_diskon(50, 1.1)}") # AssertionError: Persentase...
  # Jika ada bug logika yg membuat harga negatif:
  # print(f"Diskon -50, 10%: {hitung_diskon(-50, 0.1)}") # AssertionError: Harga...
except AssertionError as ae:
  print(f"Assertion Error: {ae}")
```

**Kapan Menggunakan `assert`:**
*   Memeriksa kondisi pra/pasca dalam fungsi (invariants).
*   Memeriksa tipe atau nilai argumen internal yang seharusnya sudah divalidasi sebelumnya.
*   Sebagai penanda kondisi yang "tidak mungkin terjadi" (jika terjadi, berarti ada bug).

**Kapan TIDAK Menggunakan `assert`:**
*   Untuk validasi data input dari pengguna atau sumber eksternal (file, jaringan). Gunakan `if/elif/else` dan `raise ValueError/TypeError` dll., karena assertion dapat dinonaktifkan.
*   Untuk error yang diharapkan terjadi dalam operasi normal (seperti `FileNotFoundError`). Gunakan `try/except`.

**Menonaktifkan Assertions:** Ketika menjalankan Python dengan opsi `-O` (Optimize), semua pernyataan `assert` akan diabaikan dan tidak dieksekusi. Ini berarti Anda tidak boleh mengandalkan `assert` untuk logika program yang krusial.

---

## 10. Pemrograman Berorientasi Objek (Object-Oriented Programming - OOP)

Pemrograman Berorientasi Objek (OOP) adalah paradigma pemrograman yang populer dan kuat yang mengorganisir perangkat lunak di sekitar **objek**, bukan hanya fungsi dan logika. Objek menggabungkan **data (atribut)** dan **perilaku (metode)** yang beroperasi pada data tersebut menjadi satu unit. Python adalah bahasa yang mendukung OOP secara ekstensif.

### Pendahuluan OOP

Konsep utama dalam OOP meliputi:

*   **Kelas (Class):** Blueprint atau cetakan untuk membuat objek. Mendefinisikan atribut (variabel) dan metode (fungsi) yang akan dimiliki oleh objek dari kelas tersebut.
*   **Objek (Object/Instance):** Instansiasi nyata dari sebuah kelas. Setiap objek memiliki state (nilai atributnya) sendiri tetapi berbagi struktur dan perilaku yang sama (metode) seperti yang didefinisikan oleh kelasnya.
*   **Atribut (Attribute):** Data atau variabel yang terkait dengan kelas atau objek. Menyimpan state objek.
*   **Metode (Method):** Fungsi yang didefinisikan di dalam kelas. Beroperasi pada data (atribut) objek. Mendefinisikan perilaku objek.
*   **Prinsip Utama:** Enkapsulasi, Pewarisan, Polimorfisme, Abstraksi (akan dibahas lebih lanjut).

OOP membantu membuat kode yang:
*   **Modular:** Objek mandiri dan dapat dikelola secara terpisah.
*   **Reusable:** Kelas dapat digunakan kembali untuk membuat banyak objek atau diwarisi oleh kelas lain.
*   **Mudah Dipelihara:** Perubahan dalam satu kelas cenderung tidak mempengaruhi bagian lain dari program secara drastis (jika dirancang dengan baik).
*   **Lebih Dekat ke Dunia Nyata:** Memungkinkan pemodelan entitas dunia nyata (mobil, pengguna, rekening bank) sebagai objek dalam kode.

### Kelas dan Objek

#### Mendefinisikan Kelas di Python

Gunakan kata kunci `class` diikuti nama kelas (konvensi `CamelCase`) dan titik dua `:`. Badan kelas diindentasi.

```python
# Mendefinisikan kelas sederhana 'Kucing'
class Kucing:
  """Blueprint untuk objek kucing."""

  # Class Attribute (dibagi oleh semua instance Kucing)
  spesies = "Felis catus"

  # Metode __init__ (Konstruktor) - dipanggil saat objek dibuat
  def __init__(self, nama_kucing, warna_kucing, umur_kucing=0):
    """Menginisialisasi objek Kucing baru."""
    # Instance Attributes (unik untuk setiap objek kucing)
    self.nama = nama_kucing
    self.warna = warna_kucing
    self.umur = umur_kucing
    self.lapar = True # Contoh atribut instance dengan nilai default
    print(f"Seekor kucing bernama '{self.nama}' ({self.warna}) telah lahir!")

  # Metode Instance (perilaku objek kucing)
  def bersuara(self):
    """Membuat kucing bersuara."""
    print(f"{self.nama} berkata: Meooow!")

  def makan(self):
    """Memberi makan kucing."""
    if self.lapar:
      print(f"{self.nama} sedang makan...")
      self.lapar = False
    else:
      print(f"{self.nama} tidak lapar sekarang.")

  def info(self):
    """Menampilkan informasi tentang kucing."""
    status_lapar = "lapar" if self.lapar else "kenyang"
    print(f"--- Info Kucing ---")
    print(f"Nama: {self.nama}")
    print(f"Warna: {self.warna}")
    print(f"Umur: {self.umur} tahun")
    print(f"Spesies: {self.spesies}") # Akses class attribute
    print(f"Status: {status_lapar}")
    print(f"--------------------")

# Membuat Objek (Instansiasi) dari kelas Kucing
kucing1 = Kucing("Oyen", "Oranye", 2) # Memanggil __init__
kucing2 = Kucing("Milo", "Coklat Belang") # Umur pakai default 0

# Mengakses atribut objek
print(f"\nNama kucing pertama: {kucing1.nama}") # Output: Oyen
print(f"Warna kucing kedua: {kucing2.warna}") # Output: Coklat Belang
print(f"Apakah kucing1 lapar? {kucing1.lapar}") # Output: True

# Mengakses class attribute (bisa dari instance atau kelas)
print(f"Spesies kucing1: {kucing1.spesies}") # Output: Felis catus
print(f"Spesies Kucing (kelas): {Kucing.spesies}") # Output: Felis catus

# Memanggil metode objek
print("\nAksi Kucing:")
kucing1.bersuara() # Output: Oyen berkata: Meooow!
kucing2.bersuara() # Output: Milo berkata: Meooow!

kucing1.makan()    # Output: Oyen sedang makan...
kucing1.makan()    # Output: Oyen tidak lapar sekarang.

# Menampilkan info objek
kucing1.info()
kucing2.info()
```

### Atribut (Instance vs Class Attributes)

*   **Instance Attributes:**
    *   Milik **setiap objek individu**.
    *   Nilainya bisa **berbeda** untuk setiap objek.
    *   Didefinisikan di dalam metode `__init__` (atau metode instance lain) menggunakan `self.nama_atribut = nilai`.
    *   Contoh di atas: `self.nama`, `self.warna`, `self.umur`, `self.lapar`.
*   **Class Attributes:**
    *   Milik **kelas itu sendiri**, bukan objek individu.
    *   Nilainya **dibagi (shared)** oleh semua objek (instance) dari kelas tersebut.
    *   Didefinisikan langsung di dalam blok `class`, di luar metode apa pun.
    *   Jika Anda mengubah class attribute melalui nama kelas (`NamaKelas.atribut = nilai_baru`), perubahan itu akan terlihat oleh semua instance yang belum meng-override atribut tersebut secara lokal.
    *   Jika Anda menugaskan nilai ke `self.nama_atribut_kelas = nilai_baru` di dalam instance, Anda membuat *instance attribute* baru dengan nama yang sama, yang akan menaungi (shadow) class attribute untuk instance tersebut saja.
    *   Contoh di atas: `spesies = "Felis catus"`.

```python
class Mobil:
    # Class attribute
    jumlah_roda = 4
    pabrikan = "Umum" # Default pabrikan

    def __init__(self, warna, merk):
        # Instance attributes
        self.warna = warna
        self.merk = merk

mobil1 = Mobil("Merah", "Toyota")
mobil2 = Mobil("Biru", "Honda")

print(f"\nMobil 1: Warna={mobil1.warna}, Merk={mobil1.merk}, Roda={mobil1.jumlah_roda}, Pabrikan={mobil1.pabrikan}")
print(f"Mobil 2: Warna={mobil2.warna}, Merk={mobil2.merk}, Roda={mobil2.jumlah_roda}, Pabrikan={mobil2.pabrikan}")

# Mengubah class attribute via nama kelas
Mobil.pabrikan = "Pabrik Mobil Kustom"
print("\n--- Setelah mengubah Mobil.pabrikan ---")
print(f"Mobil 1 Pabrikan: {mobil1.pabrikan}") # Berubah
print(f"Mobil 2 Pabrikan: {mobil2.pabrikan}") # Berubah

# Membuat instance attribute yang menaungi class attribute
mobil1.jumlah_roda = 3 # Ini membuat atribut INSTANCE 'jumlah_roda' hanya untuk mobil1
print("\n--- Setelah mobil1.jumlah_roda = 3 ---")
print(f"Mobil 1 Roda: {mobil1.jumlah_roda}") # 3 (dari instance attribute)
print(f"Mobil 2 Roda: {mobil2.jumlah_roda}") # 4 (masih dari class attribute)
print(f"Mobil.jumlah_roda: {Mobil.jumlah_roda}") # 4 (class attribute asli tidak berubah)
```

### Metode

#### Metode `__init__` (Konstruktor)

Metode spesial `__init__` adalah **konstruktor** kelas di Python. Ia dipanggil secara otomatis **ketika Anda membuat instance baru** dari sebuah kelas (`objek = NamaKelas(...)`). Tugas utamanya adalah **menginisialisasi state awal objek** dengan menetapkan nilai ke atribut instance (`self.nama_atribut`). Argumen yang Anda berikan saat membuat objek (setelah nama kelas) akan diteruskan ke `__init__` (setelah parameter `self`).

#### Parameter `self`

Parameter pertama dari setiap **metode instance** (termasuk `__init__`) secara konvensi dinamai `self`. Anda bisa memberinya nama lain, tetapi `self` adalah standar yang sangat kuat diikuti. `self` merujuk pada **objek instance itu sendiri** yang sedang memanggil metode tersebut. Melalui `self`, metode dapat:
*   Mengakses atau memodifikasi **atribut instance** lain (`self.nama`, `self.warna`).
*   Memanggil **metode instance** lain (`self.metode_lain()`).
*   Mengakses **class attributes** (`self.spesies` atau `NamaKelas.spesies`).

Python secara otomatis meneruskan instance sebagai argumen pertama (`self`) ketika Anda memanggil metode pada sebuah objek (`objek.metode(argumen_lain)`), jadi Anda tidak perlu menyertakannya secara manual saat pemanggilan.

#### Metode Instance

Ini adalah jenis metode yang paling umum. Mereka terikat pada instance objek dan beroperasi pada data (atribut) instance tersebut melalui parameter `self`. Contoh: `bersuara()`, `makan()`, `info()` pada kelas `Kucing`.

#### Metode Kelas (`@classmethod`)

Metode kelas terikat pada **kelas itu sendiri**, bukan pada instance spesifik. Mereka menerima **kelas (`cls`)** sebagai argumen pertama, bukan instance (`self`). Untuk menandainya, gunakan decorator `@classmethod`.

**Kasus penggunaan umum:**
*   **Factory Methods (Metode Pabrik):** Membuat instance objek dengan cara alternatif atau dari sumber data yang berbeda (misalnya, membuat objek `Tanggal` dari string `YYYY-MM-DD`).
*   **Mengakses atau Memodifikasi Class Attributes:** Karena menerima `cls`, mereka dapat berinteraksi dengan atribut kelas secara langsung.

```python
import datetime

class Pengguna:
    jumlah_pengguna_aktif = 0 # Class attribute

    def __init__(self, nama, tgl_lahir_str):
        self.nama = nama
        # Konversi tanggal lahir dari string
        tahun, bulan, tanggal = map(int, tgl_lahir_str.split('-'))
        self.tgl_lahir = datetime.date(tahun, bulan, tanggal)
        Pengguna.jumlah_pengguna_aktif += 1 # Akses class attribute saat init

    def info(self):
        print(f"Nama: {self.nama}, Tgl Lahir: {self.tgl_lahir}")

    @classmethod
    def dari_timestamp(cls, nama, timestamp):
        """Factory method: Membuat Pengguna dari Unix timestamp."""
        tgl_lahir = datetime.date.fromtimestamp(timestamp)
        tgl_lahir_str = tgl_lahir.strftime('%Y-%m-%d')
        # Memanggil __init__ secara tidak langsung via cls()
        # 'cls' di sini merujuk ke kelas Pengguna
        print(f"Membuat pengguna '{nama}' dari timestamp via @classmethod...")
        return cls(nama, tgl_lahir_str) # Sama seperti Pengguna(nama, tgl_lahir_str)

    @classmethod
    def get_jumlah_pengguna(cls):
        """Mengembalikan nilai class attribute."""
        return cls.jumlah_pengguna_aktif

# Membuat instance secara normal
user1 = Pengguna("Andi", "1995-03-15")

# Membuat instance menggunakan factory method @classmethod
# Misal timestamp untuk 1 Jan 2000
ts_2000 = 946684800
user2 = Pengguna.dari_timestamp("Beti", ts_2000)

user1.info()
user2.info()

# Mengakses class attribute via @classmethod
print(f"\nJumlah pengguna aktif (via @classmethod): {Pengguna.get_jumlah_pengguna()}") # Output: 2
```

#### Metode Statis (`@staticmethod`)

Metode statis tidak terikat pada instance (`self`) maupun kelas (`cls`). Mereka pada dasarnya adalah **fungsi biasa** yang ditempatkan di dalam namespace kelas, biasanya karena memiliki hubungan logis dengan kelas tersebut, tetapi tidak bergantung pada state instance atau kelas. Gunakan decorator `@staticmethod`.

**Kapan digunakan?**
*   Ketika Anda memiliki fungsi utilitas yang relevan dengan kelas tetapi tidak perlu mengakses data instance atau kelas.
*   Untuk mengorganisir fungsi terkait di bawah namespace kelas.

```python
class Kalkulator:
    @staticmethod
    def tambah(x, y):
        """Metode statis, tidak butuh self atau cls."""
        return x + y

    @staticmethod
    def kurang(x, y):
        return x - y

    def __init__(self, nilai_awal=0):
        self.hasil_sementara = nilai_awal # Instance attribute

    def kali(self, x): # Instance method
        self.hasil_sementara *= x
        return self.hasil_sementara

# Memanggil metode statis (bisa dari kelas atau instance)
hasil_tambah = Kalkulator.tambah(5, 3)
print(f"\nHasil tambah (statis): {hasil_tambah}") # Output: 8

calc_obj = Kalkulator(10)
hasil_kurang = calc_obj.kurang(10, 4) # Bisa juga dipanggil dari instance
print(f"Hasil kurang (statis via instance): {hasil_kurang}") # Output: 6

hasil_kali = calc_obj.kali(5) # Memanggil instance method
print(f"Hasil kali (instance): {hasil_kali}") # Output: 50
```

### Prinsip Utama OOP

Empat pilar utama OOP memberikan struktur dan manfaat paradigma ini:

#### 1. Enkapsulasi (Encapsulation)

*   **Konsep:** Menggabungkan data (atribut) dan metode (perilaku) yang beroperasi pada data tersebut ke dalam satu unit (kelas). Tujuannya adalah untuk **menyembunyikan detail implementasi internal** objek dari dunia luar dan hanya mengekspos antarmuka (metode publik) yang diperlukan untuk berinteraksi dengannya. Ini melindungi integritas data objek (state) agar tidak diubah secara sembarangan dari luar.
*   **Implementasi di Python:**
    *   **Kontrol Akses (Konvensi):** Python tidak memiliki kata kunci `private` atau `protected` yang ketat seperti Java/C++. Namun, ada konvensi yang kuat:
        *   **Nama tanpa underscore (misal `nama`):** Dianggap **publik**, dapat diakses dari mana saja.
        *   **Nama diawali satu underscore (misal `_saldo`):** Dianggap **"protected"** (konvensi). Menandakan bahwa ini adalah bagian internal kelas dan *sebaiknya* tidak diakses langsung dari luar kelas, meskipun secara teknis masih bisa. Dimaksudkan untuk digunakan di dalam kelas itu sendiri atau subclass-nya.
        *   **Nama diawali dua underscore (misal `__nomor_rekening`):** Memicu **Name Mangling**. Python secara otomatis mengubah nama ini menjadi `_NamaKelas__namaAtribut` (misal `_RekeningBank__nomor_rekening`). Ini membuatnya lebih sulit (tapi tidak mustahil) untuk diakses dari luar dan mencegah bentrokan nama secara tidak sengaja di subclass. Dianggap **"private"** (konvensi).
    *   **Properti (`@property`, `@setter`, `@deleter`):** Cara Pythonic untuk mengimplementasikan enkapsulasi dengan mengontrol bagaimana atribut diakses atau dimodifikasi. Memungkinkan Anda menjalankan logika (validasi, perhitungan) saat atribut dibaca, ditulis, atau dihapus, sambil tetap memberikan sintaks akses yang sederhana seperti atribut biasa.

```python
class RekeningBank:
    def __init__(self, pemilik, saldo_awal=0):
        self.pemilik = pemilik # Publik
        self._saldo = saldo_awal # Protected (konvensi)
        self.__nomor_rekening = self._generate_nomor() # Private (name mangling)
        self._log_transaksi = [] # Protected

    def _generate_nomor(self):
        # Logika internal untuk generate nomor rekening (anggap saja)
        import random
        return random.randint(10000, 99999)

    def setor(self, jumlah):
        if jumlah > 0:
            self._saldo += jumlah
            self._log_transaksi.append(f"Setor: +{jumlah}")
            print(f"Setor {jumlah} berhasil.")
        else:
            print("Jumlah setor harus positif.")

    def tarik(self, jumlah):
        if jumlah <= 0:
            print("Jumlah tarik harus positif.")
        elif jumlah > self._saldo:
            print("Saldo tidak cukup.")
        else:
            self._saldo -= jumlah
            self._log_transaksi.append(f"Tarik: -{jumlah}")
            print(f"Tarik {jumlah} berhasil.")

    # Menggunakan @property untuk akses saldo (read-only)
    @property
    def saldo(self):
        """Getter untuk saldo (hanya bisa dibaca)."""
        print("(Mengakses saldo via property)")
        return self._saldo

    # Tidak ada @saldo.setter, jadi saldo tidak bisa diubah langsung dari luar
    # rekening._saldo = 1000000 # Sebaiknya dihindari
    # rekening.saldo = 1000000 # Akan error (AttributeError: can't set attribute)

    def tampilkan_log(self):
        print(f"\n--- Log Transaksi untuk {self.pemilik} ---")
        if not self._log_transaksi:
            print("Tidak ada transaksi.")
        else:
            for log in self._log_transaksi:
                print(log)

    def _metode_internal(self):
        # Contoh metode internal/protected
        print("Ini metode internal.")

    def get_nomor_rekening_tersembunyi(self):
        # Cara mengakses atribut 'private' (jika perlu, tapi jarang)
        return self.__nomor_rekening


rek1 = RekeningBank("Andi", 500)
rek1.setor(200)
rek1.tarik(100)
# rek1.tarik(700) # Output: Saldo tidak cukup.

# Mengakses atribut publik
print(f"\nPemilik Rekening: {rek1.pemilik}")

# Mengakses saldo via property (getter)
print(f"Saldo saat ini: {rek1.saldo}") # Memanggil metode saldo() di balik layar

# Mencoba akses protected (bisa, tapi sebaiknya tidak)
# print(f"Saldo (akses langsung _saldo): {rek1._saldo}")
# rek1._metode_internal() # Bisa dipanggil

# Mencoba akses private (gagal dengan nama asli)
# print(rek1.__nomor_rekening) # AttributeError
# Akses via name mangling (bisa, tapi sangat tidak disarankan)
# print(f"Nomor Rekening (mangled): {rek1._RekeningBank__nomor_rekening}")
print(f"Nomor Rekening (via metode): {rek1.get_nomor_rekening_tersembunyi()}")

rek1.tampilkan_log()
```

#### 2. Pewarisan (Inheritance)

*   **Konsep:** Mekanisme di mana sebuah kelas baru (**subclass** atau **derived class**) dapat "mewarisi" atribut dan metode dari kelas yang sudah ada (**superclass** atau **base class**). Subclass secara otomatis mendapatkan semua fitur dari superclassnya dan dapat **menambahkan fitur baru** atau **mengubah (override)** perilaku yang diwarisi. Ini mempromosikan **code reuse** dan menciptakan hierarki kelas ("is-a" relationship, misal "Kucing *is a* Hewan").
*   **Implementasi di Python:**
    *   **Sintaks:** `class SubKelas(SuperKelas): ...`
    *   **Meng-override Metode:** Definisikan metode dengan nama yang sama di subclass. Metode di subclass akan digunakan untuk instance subclass tersebut.
    *   **Fungsi `super()`:** Digunakan di dalam subclass untuk memanggil metode dari **superclass**. Sangat penting, terutama dalam `__init__` subclass untuk memastikan inisialisasi superclass juga dijalankan, dan dalam metode yang di-override untuk *menambah* fungsionalitas superclass, bukan hanya menggantinya.
    *   **Pewarisan Ganda (Multiple Inheritance):** Python mengizinkan subclass mewarisi dari *lebih dari satu* superclass: `class SubKelas(Super1, Super2): ...`. Ini bisa sangat kuat tetapi juga kompleks karena potensi masalah seperti "Diamond Problem" (ambiguitas jika kedua superclass punya metode dengan nama sama). Python menggunakan **Method Resolution Order (MRO)** (algoritma C3) untuk menentukan urutan pencarian metode dalam kasus pewarisan ganda. Gunakan dengan hati-hati.

```python
# Superclass
class Hewan:
    def __init__(self, nama):
        self.nama = nama
        print(f"Seekor hewan bernama '{self.nama}' dibuat.")

    def makan(self):
        print(f"{self.nama} sedang makan.")

    def bersuara(self):
        print(f"{self.nama} mengeluarkan suara generik.")

# Subclass Kucing mewarisi dari Hewan
class Kucing(Hewan): # Mewarisi dari Hewan
    def __init__(self, nama, warna):
        # Panggil __init__ dari superclass (Hewan) untuk inisialisasi nama
        super().__init__(nama)
        # Tambahkan atribut spesifik Kucing
        self.warna = warna
        print(f"-> Dan ini adalah seekor kucing berwarna {self.warna}.")

    # Override metode bersuara
    def bersuara(self):
        print(f"{self.nama} (kucing) berkata: Meooow!")

    # Tambahkan metode spesifik Kucing
    def mengejar_tikus(self):
        print(f"{self.nama} sedang mengejar tikus!")

# Subclass Anjing mewarisi dari Hewan
class Anjing(Hewan):
    def __init__(self, nama, ras):
        super().__init__(nama)
        self.ras = ras
        print(f"-> Dan ini adalah seekor anjing ras {self.ras}.")

    # Override metode bersuara
    def bersuara(self):
        print(f"{self.nama} (anjing) berkata: Guk! Guk!")

    # Override metode makan untuk menambah detail
    def makan(self):
        super().makan() # Panggil metode makan dari Hewan
        print(f"-> {self.nama} (anjing) makan dengan lahap.")

# Membuat instance
hewan_umum = Hewan("Generik")
oyen = Kucing("Oyen", "Oranye")
doggo = Anjing("Doggo", "Golden Retriever")

print("\nAksi Hewan:")
hewan_umum.makan()
hewan_umum.bersuara()

print("\nAksi Oyen (Kucing):")
oyen.makan()       # Metode makan diwarisi dari Hewan
oyen.bersuara()    # Metode bersuara di-override oleh Kucing
oyen.mengejar_tikus() # Metode spesifik Kucing

print("\nAksi Doggo (Anjing):")
doggo.makan()      # Metode makan di-override (memanggil super().makan())
doggo.bersuara()   # Metode bersuara di-override oleh Anjing
# doggo.mengejar_tikus() # AttributeError: Anjing tidak punya metode ini

# Mengecek tipe dan hubungan inheritance
print(f"\nApakah oyen instance Kucing? {isinstance(oyen, Kucing)}") # True
print(f"Apakah oyen instance Hewan? {isinstance(oyen, Hewan)}") # True (karena Kucing mewarisi Hewan)
print(f"Apakah hewan_umum instance Kucing? {isinstance(hewan_umum, Kucing)}") # False
print(f"Apakah Kucing subclass dari Hewan? {issubclass(Kucing, Hewan)}") # True
print(f"Apakah Hewan subclass dari Kucing? {issubclass(Hewan, Kucing)}") # False
```

#### 3. Polimorfisme (Polymorphism)

*   **Konsep:** Berasal dari bahasa Yunani yang berarti "banyak bentuk". Dalam OOP, polimorfisme berarti kemampuan objek dari kelas yang berbeda untuk merespons **pesan (pemanggilan metode) yang sama** dengan cara (implementasi) yang berbeda, sesuai dengan tipenya masing-masing. Ini memungkinkan penulisan kode yang lebih generik dan fleksibel, yang dapat bekerja dengan berbagai jenis objek tanpa perlu mengetahui tipe spesifiknya, selama objek tersebut menyediakan antarmuka (metode) yang diharapkan.
*   **Implementasi di Python:**
    *   **Duck Typing:** Cara polimorfisme yang paling umum di Python. Fokusnya bukan pada *tipe* objek (kelasnya apa atau mewarisi dari mana), melainkan pada *kemampuan* atau *perilaku* objek (metode apa saja yang dimilikinya). Jika sebuah objek memiliki metode yang diperlukan oleh suatu kode, kode tersebut dapat bekerja dengan objek itu, terlepas dari kelas asalnya. "If it walks like a duck and quacks like a duck, then it must be a duck."
    *   **Polimorfisme dengan Inheritance (Method Overriding):** Seperti yang terlihat di contoh inheritance, ketika subclass meng-override metode superclass, pemanggilan metode yang sama pada objek superclass dan subclass akan menghasilkan perilaku yang berbeda. Ini adalah bentuk polimorfisme yang lebih terstruktur berdasarkan hierarki kelas.

```python
# Contoh Duck Typing
class Bebek:
    def bersuara(self):
        print("Bebek: Kwek! Kwek!")
    def berjalan(self):
        print("Bebek berjalan menggemaskan.")

class Manusia:
    def bersuara(self):
        print("Manusia: Halo!")
    def berjalan(self):
        print("Manusia berjalan tegak.")

class MobilMainan:
    def bersuara(self):
        print("Mobil Mainan: Ngiung... Ngiung...")
    # Tidak punya metode berjalan

# Fungsi yang bekerja dengan objek APA PUN yang punya metode 'bersuara' dan 'berjalan'
def aksi_objek(obj):
    print(f"\n--- Aksi untuk objek tipe {type(obj).__name__} ---")
    try:
        obj.bersuara()
        obj.berjalan()
    except AttributeError as e:
        print(f"Objek ini tidak bisa melakukan semua aksi: {e}")

bebek = Bebek()
andi = Manusia()
mainan = MobilMainan()

aksi_objek(bebek) # Sukses
aksi_objek(andi)  # Sukses
aksi_objek(mainan)# Gagal di berjalan() karena tidak ada metode itu

# Contoh Polimorfisme dengan Inheritance
# Kita sudah punya kelas Hewan, Kucing, Anjing sebelumnya

# Fungsi generik yang bekerja dengan Hewan (atau subclassnya)
def interaksi_hewan(hewan_peliharaan):
    print(f"\n--- Berinteraksi dengan {hewan_peliharaan.nama} ---")
    hewan_peliharaan.makan()
    hewan_peliharaan.bersuara() # Perilaku berbeda tergantung objek (Kucing/Anjing)

interaksi_hewan(oyen)  # Memanggil makan() Hewan, bersuara() Kucing
interaksi_hewan(doggo) # Memanggil makan() Anjing, bersuara() Anjing
```

#### 4. Abstraksi (Abstraction)

*   **Konsep:** Menyembunyikan detail implementasi yang kompleks dan hanya menampilkan fitur atau fungsionalitas esensial kepada pengguna (atau kode lain). Fokus pada **apa** yang dilakukan objek, bukan **bagaimana** ia melakukannya. Ini membantu mengurangi kompleksitas dan memudahkan interaksi dengan objek. Enkapsulasi adalah salah satu cara mencapai abstraksi. Cara lain adalah melalui **kelas abstrak**.
*   **Implementasi di Python:**
    *   **Kelas Abstrak (Abstract Base Classes - ABCs):** Disediakan oleh modul `abc`. ABC mendefinisikan *antarmuka (interface)* atau kontrak yang harus dipenuhi oleh subclass konkret. ABC bisa memiliki metode biasa (dengan implementasi) dan **metode abstrak** (tanpa implementasi, ditandai dengan decorator `@abc.abstractmethod`).
    *   Anda **tidak bisa** membuat instance langsung dari ABC jika ia memiliki metode abstrak yang belum diimplementasikan.
    *   Subclass **wajib** meng-override (menyediakan implementasi) semua metode abstrak yang diwarisi dari ABC agar bisa diinstansiasi.
    *   ABCs berguna untuk memastikan bahwa sekelompok kelas terkait memiliki struktur atau perilaku dasar yang sama.

```python
import abc # Modul untuk Abstract Base Classes

# Mendefinisikan Kelas Abstrak
class Bentuk(abc.ABC): # Mewarisi dari abc.ABC
    def __init__(self, nama):
        self.nama = nama

    @abc.abstractmethod # Menandai metode ini sebagai abstrak
    def hitung_luas(self):
        """Metode abstrak: Subclass HARUS mengimplementasikan ini."""
        pass # Tidak ada implementasi di kelas abstrak

    @abc.abstractmethod
    def tampilkan_info(self):
        """Metode abstrak lain."""
        pass

    def get_nama(self): # Metode biasa (konkret) dalam kelas abstrak
        return self.nama

# Mencoba membuat instance dari kelas abstrak (akan error)
# bentuk_abstrak = Bentuk("Abstrak") # TypeError: Can't instantiate abstract class Bentuk ...

# Subclass Konkret yang mengimplementasikan metode abstrak
class Persegi(Bentuk):
    def __init__(self, nama, sisi):
        super().__init__(nama)
        self.sisi = sisi

    # Implementasi metode abstrak hitung_luas
    def hitung_luas(self):
        return self.sisi * self.sisi

    # Implementasi metode abstrak tampilkan_info
    def tampilkan_info(self):
        print(f"Bentuk: {self.get_nama()} (Persegi)")
        print(f"Sisi: {self.sisi}")
        print(f"Luas: {self.hitung_luas()}")

class Lingkaran(Bentuk):
    def __init__(self, nama, radius):
        super().__init__(nama)
        self.radius = radius

    def hitung_luas(self):
        import math
        return math.pi * self.radius**2

    def tampilkan_info(self):
        print(f"Bentuk: {self.get_nama()} (Lingkaran)")
        print(f"Radius: {self.radius}")
        print(f"Luas: {self.hitung_luas():.2f}")

# Membuat instance dari subclass konkret (bisa dilakukan)
persegi1 = Persegi("Kotak Merah", 5)
lingkaran1 = Lingkaran("Roda Biru", 7)

print("\n--- Info Bentuk ---")
persegi1.tampilkan_info()
print("-" * 15)
lingkaran1.tampilkan_info()

# Fungsi yang dapat bekerja dengan objek Bentuk APAPUN (polimorfisme)
def cetak_luas_bentuk(objek_bentuk):
    # Memastikan objek adalah instance dari Bentuk (opsional tapi baik)
    if isinstance(objek_bentuk, Bentuk):
        print(f"\nMenghitung luas untuk {objek_bentuk.get_nama()}: {objek_bentuk.hitung_luas():.2f}")
    else:
        print("Objek bukan merupakan turunan dari Bentuk.")

cetak_luas_bentuk(persegi1)
cetak_luas_bentuk(lingkaran1)
```

### Metode Khusus (Dunder/Magic Methods)

Metode dengan nama diawali dan diakhiri dua underscore (misalnya `__init__`, `__str__`) disebut *dunder methods* (double underscore) atau *magic methods*. Metode ini bukan untuk dipanggil langsung oleh Anda (kecuali `__init__` via `super()`), melainkan dipanggil secara otomatis oleh Python sebagai respons terhadap operasi atau fungsi bawaan tertentu. Mereka memungkinkan objek Anda berperilaku seperti tipe data bawaan dan terintegrasi mulus dengan sintaks Python.

Beberapa dunder method penting:

*   **`__init__(self, ...)`:** Konstruktor objek, dipanggil saat instansiasi.
*   **`__str__(self)`:** Dipanggil oleh fungsi `str()` dan `print()`. Harus mengembalikan **representasi string yang *user-friendly*** dari objek. Jika `__str__` tidak ada, Python akan fallback ke `__repr__`.
*   **`__repr__(self)`:** Dipanggil oleh fungsi `repr()` dan ditampilkan di interpreter interaktif saat Anda mengetik nama objek. Harus mengembalikan **representasi string yang *unambiguous*** dari objek, idealnya string yang bisa dievaluasi Python untuk membuat ulang objek (misal, `NamaKelas(arg1='nilai1')`). Jika `__repr__` tidak ada, representasi default (misal `<__main__.NamaKelas object at 0x...>)` akan digunakan. **Penting untuk selalu mengimplementasikan `__repr__` yang baik.**
*   **`__len__(self)`:** Dipanggil oleh fungsi `len()`. Harus mengembalikan panjang (integer) dari objek (misalnya, jumlah item dalam koleksi).
*   **`__eq__(self, other)`:** Dipanggil oleh operator kesetaraan `==`. Harus mengembalikan `True` jika objek `self` dianggap sama dengan objek `other`, `False` sebaliknya. Jika tidak diimplementasikan, `==` akan membandingkan identitas objek (sama dengan `is`).
*   **Metode Perbandingan Lain:** `__ne__(self, other)` (`!=`), `__lt__(self, other)` (`<`), `__le__(self, other)` (`<=`), `__gt__(self, other)` (`>`), `__ge__(self, other)` (`>=`). Memungkinkan objek diurutkan atau dibandingkan.
*   **Metode Operator Aritmatika:** `__add__(self, other)` (`+`), `__sub__(self, other)` (`-`), `__mul__(self, other)` (`*`), `__truediv__(self, other)` (`/`), dll. Memungkinkan operator aritmatika digunakan pada objek Anda.
*   **Metode Akses Item:** `__getitem__(self, key)` (untuk `obj[key]`), `__setitem__(self, key, value)` (untuk `obj[key] = value`), `__delitem__(self, key)` (untuk `del obj[key]`). Memungkinkan objek berperilaku seperti sequence atau mapping.
*   **`__call__(self, ...)`:** Memungkinkan instance objek dipanggil seolah-olah ia adalah fungsi (`objek(arg1, arg2)`).

```python
class Buku:
    def __init__(self, judul, penulis, tahun):
        self.judul = judul
        self.penulis = penulis
        self.tahun = tahun

    def __str__(self):
        # Representasi user-friendly
        return f'"{self.judul}" oleh {self.penulis} ({self.tahun})'

    def __repr__(self):
        # Representasi developer-friendly, idealnya bisa dievaluasi
        # Menggunakan repr() internal untuk string agar kutipnya benar
        return f"Buku(judul={repr(self.judul)}, penulis={repr(self.penulis)}, tahun={self.tahun})"

    def __eq__(self, other):
        # Membandingkan kesamaan berdasarkan atribut
        if not isinstance(other, Buku):
            return NotImplemented # Penting untuk tipe lain
        return (self.judul == other.judul and
                self.penulis == other.penulis and
                self.tahun == other.tahun)

    def __len__(self):
        # Contoh: panjang buku adalah jumlah karakter judul
        return len(self.judul)

# Membuat instance
buku1 = Buku("Belajar Python OOP", "Guido van Rossum", 2023)
buku2 = Buku("Data Science Lanjut", "Wes McKinney", 2022)
buku3 = Buku("Belajar Python OOP", "Guido van Rossum", 2023) # Sama dengan buku1

print("\n--- Dunder Methods ---")
# Dipanggil oleh print() -> menggunakan __str__
print(buku1)
print(buku2)

# Dipanggil di interpreter atau oleh repr() -> menggunakan __repr__
print(repr(buku1))
print([buku1, buku2]) # List menggunakan repr() untuk elemennya

# Dipanggil oleh len() -> menggunakan __len__
print(f"Panjang judul buku 1: {len(buku1)}")

# Dipanggil oleh == -> menggunakan __eq__
print(f"Apakah buku1 == buku2? {buku1 == buku2}") # False
print(f"Apakah buku1 == buku3? {buku1 == buku3}") # True
print(f"Apakah buku1 == 'teks'? {buku1 == 'teks'}") # False (karena check isinstance di __eq__)
```

### Data Classes (`@dataclass`) - Python 3.7+

Modul `dataclasses` menyediakan decorator `@dataclass` yang sangat menyederhanakan pembuatan kelas yang tujuan utamanya adalah untuk menyimpan data (mirip struct di bahasa lain). Secara otomatis ia akan men-generate metode-metode dunder umum seperti `__init__`, `__repr__`, `__eq__` (dan opsional `__lt__`, `__le__`, dll. jika `order=True`) berdasarkan *type hints* yang Anda definisikan untuk atribut kelas.

```python
from dataclasses import dataclass, field # Import field juga jika perlu default factory

@dataclass(order=True) # order=True akan generate __lt__, __le__, dll.
class InventarisItem:
    """Kelas untuk menyimpan item inventaris (menggunakan dataclass)."""
    nama: str # Type hint wajib untuk atribut yang diinginkan
    unit_harga: float
    kuantitas: int = 0 # Bisa beri nilai default biasa
    # Untuk default mutable, gunakan field(default_factory=...)
    tags: list[str] = field(default_factory=list)
    # Atribut ini akan diurutkan berdasarkan nama, lalu unit_harga (sesuai urutan definisi)
    sort_index: int = field(init=False, repr=False) # Contoh field khusus

    # __post_init__ dipanggil setelah __init__ otomatis
    def __post_init__(self):
        # Hitung nilai sort_index setelah inisialisasi
        self.sort_index = self.kuantitas
        print(f"Item '{self.nama}' diinisialisasi (post_init).")
        # Bisa juga lakukan validasi di sini

    # Anda masih bisa menambah metode lain
    def total_nilai(self) -> float:
        return self.unit_harga * self.kuantitas

# Membuat instance (lebih ringkas, __init__ otomatis)
item1 = InventarisItem("Pensil", 2000.0, 50, tags=["alat tulis"])
item2 = InventarisItem("Buku", 5000.0, tags=["alat tulis", "bacaan"]) # kuantitas default 0
item3 = InventarisItem("Pensil", 1800.0, 20) # Harga beda

print("\n--- Data Classes ---")
# __repr__ otomatis dihasilkan dan cukup bagus
print(item1)
print(item2)

# __eq__ otomatis dihasilkan
print(f"Apakah item1 == item3? {item1 == item3}") # False (harga beda)

# Metode biasa tetap bisa dipanggil
print(f"Total nilai item1: {item1.total_nilai()}")
print(f"Total nilai item2: {item2.total_nilai()}")

# Perbandingan (karena order=True)
print(f"Apakah item2 < item1? {item2 < item1}") # True (Buku < Pensil secara alfabet)

# Default factory untuk list
print(f"Tags item 1: {item1.tags}")
print(f"Tags item 2: {item2.tags}") # List baru, bukan shared
item2.tags.append("baru")
print(f"Tags item 1 setelah item 2 diubah: {item1.tags}") # Tidak terpengaruh
```
`@dataclass` sangat berguna untuk mengurangi kode boilerplate saat membuat kelas data sederhana.

---

## 11. Topik Menengah

Setelah menguasai dasar-dasar dan OOP, mari kita jelajahi beberapa konsep Python yang lebih menengah yang dapat membuat kode Anda lebih kuat, efisien, dan elegan.

### List/Set/Dictionary Comprehensions (Lebih Dalam)

Kita sudah melihat dasar-dasarnya. Mari lihat beberapa penggunaan yang sedikit lebih kompleks:

*   **Comprehension Bersarang:** Membuat struktur data bersarang atau memproses iterable bersarang.
*   **Kondisional dalam Ekspresi:** Menggunakan ekspresi `if-else` (ternary operator) di bagian *ekspresi* comprehension.

```python
# Comprehension Bersarang: Membuat matriks 3x3
matriks = [[(baris, kolom) for kolom in range(3)] for baris in range(3)]
print(f"\nMatriks 3x3 dibuat dengan comprehension:\n{matriks}")

# Nested comprehension untuk 'flatten' list of lists (sudah dicontohkan sebelumnya)
list_nested = [[1, 2], [3, 4, 5], [6]]
list_flat = [item for sublist in list_nested for item in sublist]
print(f"Flatten list: {list_flat}") # [1, 2, 3, 4, 5, 6]

# Kondisional dalam Ekspresi: Kategorikan angka ganjil/genap
angka = range(1, 7)
kategori = ["genap" if x % 2 == 0 else "ganjil" for x in angka]
print(f"Kategori angka {list(angka)}: {kategori}") # ['ganjil', 'genap', 'ganjil', 'genap', 'ganjil', 'genap']

# Dictionary comprehension dengan kondisional di nilai
dict_asli = {'a': 1, 'b': 2, 'c': 3, 'd': 4}
dict_kuadrat_genap = {k: v**2 if v % 2 == 0 else v for k, v in dict_asli.items()}
print(f"Dict kuadrat genap: {dict_kuadrat_genap}") # {'a': 1, 'b': 4, 'c': 3, 'd': 16}
```

### Generator Expressions

Sangat mirip dengan list comprehension secara sintaks, tetapi menggunakan **kurung biasa `()`** bukan kurung siku `[]`. Perbedaan utamanya adalah:

*   **List Comprehension:** Mengevaluasi seluruh ekspresi dan membuat **list lengkap di memori** secara langsung.
*   **Generator Expression:** Membuat objek **iterator (generator)**. Nilai dihasilkan **satu per satu (lazy evaluation)** hanya ketika diminta (misalnya, saat iterasi dalam loop `for` atau saat `next()` dipanggil).

**Keuntungan Generator Expression:**
*   **Efisien Memori:** Sangat berguna untuk sekuens data yang sangat besar, karena tidak perlu menyimpan semua elemen di memori sekaligus.
*   **Lazy Evaluation:** Perhitungan hanya dilakukan saat nilai dibutuhkan.

```python
# List comprehension (membuat list penuh di memori)
list_comp = [x * 2 for x in range(1000000)] # Bisa makan banyak memori
# print(f"Ukuran list_comp (contoh): {sys.getsizeof(list_comp)}")

# Generator expression (membuat iterator)
gen_expr = (x * 2 for x in range(1000000)) # Sangat hemat memori
# print(f"Ukuran gen_expr (contoh): {sys.getsizeof(gen_expr)}") # Jauh lebih kecil

print(f"\nTipe gen_expr: {type(gen_expr)}") # <class 'generator'>

# Nilai baru dihasilkan saat iterasi
print("Iterasi pertama dari generator expression (ambil 5):")
count = 0
for nilai in gen_expr:
    print(nilai, end=" ")
    count += 1
    if count >= 5:
        break # Output: 0 2 4 6 8
print()

# Melanjutkan iterasi (iterator mengingat posisinya)
print("Iterasi kedua dari generator expression (ambil 5 lagi):")
count = 0
for nilai in gen_expr: # Melanjutkan dari tempat berhenti sebelumnya
    print(nilai, end=" ")
    count += 1
    if count >= 5:
        break # Output: 10 12 14 16 18
print()

# Generator expression sering digunakan sebagai argumen fungsi
total = sum(x**2 for x in range(1, 11)) # Tidak perlu list sementara
print(f"\nJumlah kuadrat 1-10 (pakai gen expr): {total}")
```
Gunakan generator expression jika Anda tidak memerlukan list lengkap sekaligus, terutama untuk data besar atau stream data.

### Fungsi Generator (`yield`)

Cara lain untuk membuat iterator adalah dengan menggunakan **fungsi generator**. Ini adalah fungsi biasa yang menggunakan kata kunci `yield` setidaknya satu kali di dalam badannya.

*   Ketika fungsi generator dipanggil, ia **tidak langsung menjalankan kode** di dalamnya. Sebaliknya, ia **mengembalikan objek iterator (generator)**.
*   Setiap kali `yield ekspresi` dieksekusi, fungsi **berhenti sementara (pauses)** pada titik itu dan **mengirimkan nilai `ekspresi`** kembali ke pemanggil (kode yang sedang mengiterasi generator).
*   State (variabel lokal) fungsi generator **dipertahankan** antara pemanggilan `yield`.
*   Ketika iterator diminta nilai berikutnya (misalnya oleh loop `for` atau `next()`), eksekusi fungsi generator **dilanjutkan tepat setelah `yield` terakhir** sampai `yield` berikutnya ditemui, atau sampai fungsi berakhir (secara normal atau via `return`), atau sampai `StopIteration` dibangkitkan.

```python
def hitung_mundur_gen(n):
    """Fungsi generator untuk hitung mundur."""
    print(f"-> Generator dimulai untuk hitung mundur dari {n}")
    while n > 0:
        print(f"  >> Yielding {n}")
        yield n # Berhenti sementara, kirim n
        print(f"  << Resuming setelah yield {n}")
        n -= 1
    print("-> Generator selesai.")
    # return "Selesai!" # return dalam generator akan jadi nilai StopIteration

# Panggil fungsi -> dapatkan objek generator
penghitung = hitung_mundur_gen(3)
print(f"Objek generator dibuat: {penghitung}")

# Iterasi menggunakan loop for (cara umum)
print("\nIterasi dengan for loop:")
for angka in penghitung:
    print(f"  Diterima dari generator: {angka}")

# Membuat generator baru (karena yg lama sudah habis)
penghitung2 = hitung_mundur_gen(2)
print("\nIterasi manual dengan next():")
try:
    print(f"  Manual next() 1: {next(penghitung2)}")
    print(f"  Manual next() 2: {next(penghitung2)}")
    print(f"  Manual next() 3: {next(penghitung2)}") # Akan StopIteration
except StopIteration as si:
    print(f"  StopIteration terjadi!") # Generator selesai

# Contoh: Generator untuk membaca file besar baris per baris (meskipun iterasi langsung lebih umum)
def baca_baris_gen(nama_file):
    try:
        with open(nama_file, "r", encoding="utf-8") as f:
            for baris in f:
                yield baris.strip() # Hilangkan newline saat yield
    except FileNotFoundError:
        print(f"Error: File {nama_file} tidak ditemukan di generator.")
        # Bisa juga raise di sini
    except Exception as e:
        print(f"Error lain di generator: {e}")

print("\nMembaca file via generator function:")
for baris_log in baca_baris_gen("access.log"): # Anggap file ini ada
     if len(baris_log) > 80: # Proses baris
         print(f"  Log panjang: {baris_log[:80]}...")
```

#### Keuntungan Menggunakan Generator

Sama seperti generator expression:
*   **Efisien Memori:** Ideal untuk sekuens data besar atau tak terbatas (infinite sequences).
*   **Lazy Evaluation:** Kode hanya berjalan saat nilai dibutuhkan.
*   **Kode Lebih Bersih:** Untuk logika pembuatan iterator yang kompleks, fungsi generator seringkali lebih mudah dibaca daripada membuat kelas iterator manual dengan `__iter__` dan `__next__`.
*   **Bisa Mewakili Stream Data:** Cocok untuk memproses data yang datang secara bertahap (misal dari jaringan atau sensor).

### Decorators (`@`)

Decorator adalah fitur Python yang sangat kuat yang memungkinkan Anda untuk **memodifikasi atau membungkus (wrap)** fungsi atau metode lain secara dinamis. Decorator menyediakan cara bersih untuk menambahkan fungsionalitas tambahan (seperti logging, timing, pemeriksaan izin, caching) ke fungsi yang sudah ada tanpa mengubah kode asli fungsi tersebut secara langsung.

Sintaks `@nama_decorator` yang diletakkan sebelum definisi fungsi (`def`) adalah *syntactic sugar* (gula sintaksis) untuk:

```python
@nama_decorator
def fungsi_saya():
  pass

# adalah sama dengan:
def fungsi_saya():
  pass
fungsi_saya = nama_decorator(fungsi_saya)
```

Decorator pada dasarnya adalah **fungsi tingkat tinggi (higher-order function)**:
*   Menerima fungsi lain sebagai argumen.
*   Biasanya mendefinisikan fungsi baru di dalamnya (wrapper function) yang menambahkan perilaku sebelum dan/atau sesudah memanggil fungsi asli.
*   Mengembalikan fungsi baru (wrapper) tersebut.

#### Memahami Decorator (Konsep Inti)

1.  **Fungsi adalah Objek First-Class:** Di Python, fungsi dapat ditugaskan ke variabel, diteruskan sebagai argumen ke fungsi lain, dan dikembalikan dari fungsi lain.
2.  **Fungsi Bersarang (Nested Functions):** Anda dapat mendefinisikan fungsi di dalam fungsi lain. Fungsi dalam hanya dapat diakses dari dalam fungsi luar (kecuali dikembalikan).
3.  **Closure:** Fungsi dalam dapat "mengingat" variabel dari scope fungsi luar (enclosing scope) tempat ia didefinisikan, bahkan setelah fungsi luar selesai dieksekusi.

#### Membuat Decorator Sederhana

```python
import time
import functools # Penting untuk functools.wraps

# 1. Decorator Function
def decorator_timer(fungsi_asli):
    """Decorator untuk mengukur waktu eksekusi sebuah fungsi."""
    @functools.wraps(fungsi_asli) # 4. Penting: Salin metadata fungsi asli
    def wrapper(*args, **kwargs): # 3. Wrapper function (terima argumen fleksibel)
        waktu_mulai = time.perf_counter()
        print(f"--- Memulai eksekusi '{fungsi_asli.__name__}' ---")
        hasil = fungsi_asli(*args, **kwargs) # Panggil fungsi asli dengan argumennya
        waktu_selesai = time.perf_counter()
        durasi = waktu_selesai - waktu_mulai
        print(f"--- Selesai '{fungsi_asli.__name__}' dalam {durasi:.4f} detik ---")
        return hasil # Kembalikan hasil dari fungsi asli
    return wrapper # 2. Kembalikan wrapper function

# Menggunakan decorator
@decorator_timer
def proses_data_lama(n):
    """Fungsi contoh yang butuh waktu."""
    print(f"Memproses {n} iterasi...")
    total = 0
    for i in range(n):
        total += i**0.5 # Operasi agak lambat
    print("Proses data selesai.")
    return total

@decorator_timer
def sapa(nama, pesan="Halo"):
    """Fungsi sapaan sederhana."""
    print(f"{pesan}, {nama}!")
    return f"Sapaan untuk {nama}"

# Memanggil fungsi yang sudah didekorasi
print("\nMemanggil fungsi yang didekorasi:")
hasil_proses = proses_data_lama(1000000) # decorator_timer akan otomatis aktif
# print(f"Hasil akhir proses data: {hasil_proses}") # Hasil tetap dikembalikan

hasil_sapa = sapa("Dunia", pesan="Selamat Pagi")
print(f"Hasil dari fungsi sapa: {hasil_sapa}")

# Melihat metadata fungsi (setelah menggunakan @wraps)
print(f"\nNama fungsi proses_data_lama: {proses_data_lama.__name__}") # Tetap proses_data_lama
print(f"Docstring proses_data_lama: {proses_data_lama.__doc__}") # Docstring asli terjaga
```

#### Decorator dengan Argumen

Terkadang Anda ingin decorator itu sendiri menerima argumen untuk mengonfigurasi perilakunya. Ini memerlukan **satu lapisan fungsi tambahan**.

```python
# Decorator Factory: Fungsi yang MENGEMBALIKAN decorator
def ulangi(jumlah):
    """Decorator Factory: Membuat decorator yang mengulang fungsi beberapa kali."""
    def decorator_ulangi(fungsi_asli): # Ini adalah decorator sebenarnya
        @functools.wraps(fungsi_asli)
        def wrapper(*args, **kwargs):
            print(f"--- Mengulang '{fungsi_asli.__name__}' {jumlah} kali ---")
            hasil_terakhir = None
            for i in range(jumlah):
                print(f"  Iterasi {i+1}:")
                hasil_terakhir = fungsi_asli(*args, **kwargs)
            print("--- Selesai pengulangan ---")
            return hasil_terakhir # Kembalikan hasil dari pemanggilan terakhir
        return wrapper
    return decorator_ulangi # Kembalikan decorator

# Menggunakan decorator dengan argumen
@ulangi(jumlah=3) # Panggil factory 'ulangi' untuk dapatkan decorator
def bip():
    print("  Bip!")

@ulangi(1) # Ulangi sekali
def tepuk_tangan():
    print("  Prok prok prok!")

print("\nMemanggil fungsi dengan decorator berargumen:")
bip()
tepuk_tangan()
```
Alurnya: `ulangi(3)` dipanggil -> mengembalikan `decorator_ulangi` -> `decorator_ulangi(bip)` dipanggil -> mengembalikan `wrapper` -> `bip` sekarang merujuk ke `wrapper`.

#### `functools.wraps`

Seperti terlihat di contoh, menggunakan `@functools.wraps(fungsi_asli)` di dalam definisi `wrapper` sangat penting. Tanpanya, fungsi yang didekorasi (`proses_data_lama`, `sapa`) akan kehilangan metadata aslinya (seperti `__name__`, `__doc__`, signature) dan malah mengambil metadata dari fungsi `wrapper`. `@wraps` menyalin metadata penting ini dari `fungsi_asli` ke `wrapper`, sehingga fungsi yang didekorasi tetap terlihat seperti aslinya bagi tools introspeksi dan debugger.

### Context Managers (`with` statement dan `contextlib`)

Context manager adalah objek yang mendefinisikan *konteks runtime* yang akan dieksekusi di sekitar sebuah blok kode (blok `with`). Tujuan utamanya adalah untuk **mengelola sumber daya** secara otomatis, memastikan bahwa sumber daya tersebut **di-setup** dengan benar sebelum blok `with` dijalankan dan **di-teardown (dibersihkan)** dengan benar setelah blok `with` selesai, *bahkan jika terjadi error*.

Kasus penggunaan paling umum adalah `with open(...)` untuk file, yang menjamin `file.close()` dipanggil. Contoh lain: mengunci dan membuka kunci (locks) dalam multithreading, membuka dan menutup koneksi database/jaringan, mengelola transaksi.

Pernyataan `with` bekerja dengan objek yang mengimplementasikan **protokol context manager**, yaitu memiliki metode:
*   `__enter__(self)`: Dieksekusi **sebelum** memasuki blok `with`. Nilai yang dikembalikan oleh metode ini (jika ada) akan ditugaskan ke variabel setelah `as` (jika ada). Bertugas melakukan setup sumber daya.
*   `__exit__(self, exc_type, exc_val, exc_tb)`: Dieksekusi **setelah** keluar dari blok `with`. Bertugas melakukan teardown/cleanup sumber daya. Menerima tiga argumen yang berisi informasi tentang exception jika terjadi di dalam blok `with` (`None` jika tidak ada exception). Jika `__exit__` mengembalikan `True`, exception tersebut dianggap telah ditangani (suppressed). Jika mengembalikan `False` atau `None` (default), exception akan diteruskan keluar setelah `__exit__` selesai.

#### Membuat Context Manager Sendiri

Ada dua cara utama:

1.  **Menggunakan Kelas:** Definisikan kelas dengan metode `__enter__` dan `__exit__`.

    ```python
    import time

    class TimerContext:
        """Context Manager sederhana untuk mengukur waktu blok kode."""
        def __enter__(self):
            print("-> Memulai timer...")
            self.start_time = time.perf_counter()
            # Kembalikan self agar bisa diakses via 'as' (opsional)
            return self

        def __exit__(self, exc_type, exc_val, exc_tb):
            self.end_time = time.perf_counter()
            duration = self.end_time - self.start_time
            print(f"<- Timer selesai. Durasi: {duration:.4f} detik.")
            # Jika ada exception, exc_type, exc_val, exc_tb akan berisi info
            if exc_type:
                print(f"!! Exception terjadi di dalam blok 'with': {exc_type.__name__}: {exc_val}")
            # Return False (atau None) agar exception (jika ada) tetap diteruskan
            return False

    # Menggunakan context manager kelas
    print("\nMenggunakan TimerContext:")
    with TimerContext() as timer: # __enter__ dipanggil, hasilnya ke 'timer'
        print("  Melakukan pekerjaan...")
        time.sleep(0.5) # Simulasi pekerjaan
        print("  Pekerjaan selesai.")
    # __exit__ otomatis dipanggil di sini

    print("\nMencoba TimerContext dengan error:")
    try:
        with TimerContext():
            print("  Melakukan pekerjaan yang akan error...")
            hasil = 10 / 0 # Akan raise ZeroDivisionError
            print("  Baris ini tidak akan jalan.")
    except ZeroDivisionError:
        print(">> Exception ZeroDivisionError ditangkap di luar 'with'.")
    # __exit__ tetap dipanggil sebelum exception ditangkap di luar
    ```

2.  **Menggunakan `contextlib.contextmanager`:** Cara yang lebih ringkas menggunakan fungsi generator dan decorator `@contextlib.contextmanager`. Kode **sebelum `yield`** berfungsi sebagai `__enter__`, nilai yang di-`yield` akan ditugaskan ke variabel `as` (jika ada), dan kode **setelah `yield`** berfungsi sebagai `__exit__`. Penanganan exception harus dilakukan secara manual di dalam generator menggunakan `try...finally`.

    ```python
    import contextlib

    @contextlib.contextmanager
    def timer_context_gen():
        """Context Manager timer menggunakan generator."""
        print("-> (Gen) Memulai timer...")
        start_time = time.perf_counter()
        try:
            yield # Titik jeda, blok 'with' dieksekusi di sini
                # Tidak ada nilai yield, jadi 'as' tidak akan mendapat apa-apa
        finally:
            # Kode ini dijamin jalan setelah blok 'with' selesai (seperti finally)
            end_time = time.perf_counter()
            duration = end_time - start_time
            print(f"<- (Gen) Timer selesai. Durasi: {duration:.4f} detik.")

    # Menggunakan context manager generator
    print("\nMenggunakan timer_context_gen:")
    with timer_context_gen():
        print("  Melakukan pekerjaan (generator)...")
        time.sleep(0.6)
        print("  Pekerjaan (generator) selesai.")
    ```
    Versi generator seringkali lebih ringkas untuk context manager sederhana.

### Regular Expressions (`re` modul)

Ekspresi reguler (regex) adalah bahasa mini yang sangat kuat untuk **mencocokkan pola (pattern)** dalam string. Sangat berguna untuk:
*   Validasi input (misalnya, format email, nomor telepon).
*   Mencari dan mengekstrak data spesifik dari teks yang tidak terstruktur.
*   Mengganti bagian dari string berdasarkan pola.

Modul `re` di Python menyediakan fungsi untuk bekerja dengan regex.

#### Pola Dasar (Beberapa Metakarakter Umum)

*   `.` (Titik): Cocok dengan karakter **apa pun** (kecuali newline secara default).
*   `^`: Cocok dengan **awal** string (atau awal baris dalam mode multiline).
*   `$`: Cocok dengan **akhir** string (atau akhir baris dalam mode multiline).
*   `*`: Cocok dengan **nol atau lebih** kemunculan dari karakter/grup sebelumnya.
*   `+`: Cocok dengan **satu atau lebih** kemunculan dari karakter/grup sebelumnya.
*   `?`: Cocok dengan **nol atau satu** kemunculan dari karakter/grup sebelumnya (membuatnya opsional). Juga digunakan untuk matching *non-greedy*.
*   `{n}`: Cocok dengan **tepat n** kemunculan.
*   `{n,}`: Cocok dengan **n atau lebih** kemunculan.
*   `{n,m}`: Cocok dengan **minimal n, maksimal m** kemunculan.
*   `[...]`: Mendefinisikan **set karakter**. Cocok dengan **satu** karakter apa pun di dalam kurung. Misal `[abc]` cocok 'a', 'b', atau 'c'. `[a-z]` cocok huruf kecil, `[0-9]` cocok digit. `[^...]` mencocokkan karakter yang *tidak* ada dalam set.
*   `(...)`: **Mengelompokkan** bagian dari pola dan **menangkap (capture)** teks yang cocok dengan grup tersebut.
*   `|`: Berfungsi sebagai **OR**. Cocok dengan pola di sebelah kiri ATAU pola di sebelah kanan.
*   `\`: **Escape character**. Digunakan untuk mencocokkan metakarakter secara harfiah (misal `\.` untuk titik) atau untuk sekuens khusus.
*   **Sekuens Khusus:**
    *   `\d`: Cocok dengan digit desimal (`[0-9]`).
    *   `\D`: Cocok dengan non-digit.
    *   `\w`: Cocok dengan karakter "word" (alphanumeric + underscore: `[a-zA-Z0-9_]`).
    *   `\W`: Cocok dengan karakter non-word.
    *   `\s`: Cocok dengan karakter whitespace (spasi, tab, newline, dll.).
    *   `\S`: Cocok dengan karakter non-whitespace.
    *   `\b`: Cocok dengan batas kata (word boundary). Posisi antara karakter word dan non-word, atau awal/akhir string jika berbatasan dengan word.
    *   `\A`: Cocok hanya di awal string (mirip `^` tapi tidak terpengaruh mode multiline).
    *   `\Z`: Cocok hanya di akhir string (mirip `$` tapi tidak terpengaruh mode multiline).

#### Fungsi Utama (`match()`, `search()`, `findall()`, `sub()`)

*   `re.match(pattern, string, flags=0)`: Mencoba mencocokkan `pattern` **hanya di awal `string`**. Mengembalikan objek *match* jika cocok, `None` jika tidak.
*   `re.search(pattern, string, flags=0)`: Mencari kecocokan `pattern` **di mana saja** dalam `string` (mencari kemunculan pertama). Mengembalikan objek *match* jika cocok, `None` jika tidak. **Lebih umum digunakan daripada `match`**.
*   `re.findall(pattern, string, flags=0)`: Menemukan **semua** kemunculan `pattern` yang tidak tumpang tindih dalam `string` dan mengembalikannya sebagai **list string**. Jika ada grup tangkapan dalam pattern, mengembalikan list tuple (satu tuple per match, berisi teks yang ditangkap oleh setiap grup).
*   `re.sub(pattern, replacement, string, count=0, flags=0)`: Mengganti (substitute) semua kemunculan `pattern` dalam `string` dengan `replacement`. `replacement` bisa berupa string (bisa merujuk grup tangkapan via `\1`, `\2`, dll.) atau fungsi. Mengembalikan string baru hasil penggantian. `count` membatasi jumlah penggantian.
*   `re.split(pattern, string, maxsplit=0, flags=0)`: Memecah `string` berdasarkan kemunculan `pattern`.
*   `re.compile(pattern, flags=0)`: Mengompilasi pola regex menjadi objek pola regex. **Sangat direkomendasikan jika Anda akan menggunakan pola yang sama berulang kali**, karena lebih efisien. Objek pola yang dikompilasi memiliki metode yang sama (`.match()`, `.search()`, `.findall()`, `.sub()`, dll.).

**Objek Match:** Dikembalikan oleh `match()` dan `search()`. Memiliki metode seperti:
*   `.group(0)` atau `.group()`: Mengembalikan seluruh string yang cocok.
*   `.group(n)`: Mengembalikan string yang ditangkap oleh grup ke-n (dimulai dari 1).
*   `.groups()`: Mengembalikan tuple berisi semua string yang ditangkap oleh semua grup.
*   `.start()`: Indeks awal kecocokan.
*   `.end()`: Indeks akhir kecocokan (eksklusif).
*   `.span()`: Tuple `(start, end)`.

```python
import re

teks = "Nomor telepon saya adalah 0812-3456-7890, dan teman saya 0855-9876-5432. Email: user@example.com"

# Contoh 1: Mencari nomor telepon (pola sederhana)
pola_telp = r"\d{4}-\d{4}-\d{4}" # r"" -> raw string, agar \ tidak dianggap escape

# search() - cari di mana saja
match_obj = re.search(pola_telp, teks)
if match_obj:
    print(f"Nomor telepon pertama ditemukan: {match_obj.group(0)}") # group(0) atau group() -> seluruh match
    print(f"  Posisi: {match_obj.span()}")
else:
    print("Nomor telepon tidak ditemukan.")

# findall() - cari semua
semua_telp = re.findall(pola_telp, teks)
print(f"Semua nomor telepon ditemukan: {semua_telp}") # ['0812-3456-7890', '0855-9876-5432']

# Contoh 2: Mengekstrak email (dengan grup)
# Pola email sederhana (tidak sempurna, tapi cukup untuk contoh)
pola_email = r"([\w.-]+)@([\w.-]+)\.([a-zA-Z]{2,})"
# Grup 1: username ([\w.-]+)
# Grup 2: domain name ([\w.-]+)
# Grup 3: top-level domain ([a-zA-Z]{2,})

match_email = re.search(pola_email, teks)
if match_email:
    print(f"\nEmail ditemukan: {match_email.group()}") # Seluruh email
    print(f"  Username: {match_email.group(1)}")   # Grup 1
    print(f"  Domain: {match_email.group(2)}")     # Grup 2
    print(f"  TLD: {match_email.group(3)}")        # Grup 3
    print(f"  Semua grup: {match_email.groups()}") # Tuple ('user', 'example', 'com')

# Contoh 3: Mengganti nomor telepon (sub)
teks_disensor = re.sub(pola_telp, "[NOMOR DISENSOR]", teks)
print(f"\nTeks setelah sensor nomor: {teks_disensor}")

# Contoh 4: Menggunakan compile untuk efisiensi
pola_angka = re.compile(r"\d+") # Kompilasi pola angka
angka_ditemukan = pola_angka.findall("Ada 3 apel dan 15 jeruk di 1 keranjang.")
print(f"\nAngka ditemukan (compile): {angka_ditemukan}") # ['3', '15', '1']
```
Regex bisa sangat kompleks. Gunakan tools online seperti Regex101.com untuk membantu membangun dan menguji pola Anda.

### Type Hinting (PEP 484)

Diperkenalkan di Python 3.5, type hinting memungkinkan Anda menambahkan **anotasi tipe** opsional ke kode Anda (variabel, parameter fungsi, nilai kembali fungsi).

**Penting:** Type hints **tidak mempengaruhi cara Python menjalankan kode**. Python tetap bahasa yang **dinamis secara tipe data** saat runtime. Type hints hanyalah **metadata** yang:
*   **Meningkatkan Keterbacaan:** Memperjelas tipe data apa yang diharapkan oleh fungsi atau disimpan dalam variabel.
*   **Membantu Pengembangan:** Memungkinkan editor kode (IDE) dan alat bantu lainnya memberikan auto-completion yang lebih baik dan mendeteksi potensi error lebih awal.
*   **Memungkinkan Analisis Statis:** Alat seperti **Mypy** dapat memeriksa kode Anda berdasarkan type hints dan melaporkan potensi `TypeError` *sebelum* Anda menjalankan program.

#### Mengapa Menggunakan Type Hinting?

*   Dokumentasi kode yang lebih baik.
*   Menangkap error tipe lebih awal dalam siklus pengembangan.
*   Memudahkan refactoring kode.
*   Meningkatkan kolaborasi tim dengan ekspektasi tipe yang jelas.

#### Sintaks Dasar

*   **Variabel:** `nama_variabel: tipe_data = nilai_awal`
*   **Parameter Fungsi:** `def fungsi(param1: tipe1, param2: tipe2 = default): ...`
*   **Nilai Kembali Fungsi:** `def fungsi(...) -> tipe_kembalian: ...`

```python
nama: str = "Alice"
umur: int = 30
aktif: bool = True
harga: float | None = None # Union type (Python 3.10+) atau Optional[float]

def sapa_lengkap(nama_depan: str, nama_belakang: str, usia: int) -> str:
    """Menyapa dengan nama lengkap dan usia, mengembalikan string sapaan."""
    print(f"Debug: Menerima {nama_depan=}, {nama_belakang=}, {usia=}")
    # Mypy akan mendeteksi jika Anda mencoba menambah string dan int di sini
    # return "Halo, " + nama_depan + " " + nama_belakang + "! Usia Anda: " + usia # TypeError terdeteksi Mypy
    return f"Halo, {nama_depan} {nama_belakang}! Usia Anda: {usia}."

def proses_angka(angka: int | float) -> None: # Menerima int atau float, tidak mengembalikan apa pun
    """Memproses angka (hanya mencetak)."""
    print(f"Memproses angka: {angka * 2}")

# Panggil fungsi
sapaan = sapa_lengkap("Budi", "Santoso", 35)
print(sapaan)
proses_angka(10)
proses_angka(5.5)
# proses_angka("lima") # Mypy akan menandai ini sebagai error tipe

# Contoh type hint untuk variabel tanpa nilai awal
koordinat: tuple[int, int]
# ... kode lain ...
# koordinat = (10, 20)
```

#### Modul `typing`

Untuk type hints yang lebih kompleks (sebelum Python 3.9/3.10 yang memperkenalkan sintaks generik bawaan seperti `list[int]`), Anda perlu mengimpor tipe dari modul `typing`. Modul ini masih sangat relevan untuk tipe yang lebih canggih.

*   `List`, `Tuple`, `Dict`, `Set`: Untuk tipe koleksi generik (misal, `List[str]`, `Dict[str, int]`). Sejak Python 3.9, bisa pakai `list[str]`, `dict[str, int]`.
*   `Union[type1, type2, ...]`: Menunjukkan nilai bisa berupa salah satu dari tipe yang diberikan. Sejak Python 3.10, bisa pakai `type1 | type2`.
*   `Optional[type1]`: Singkatan untuk `Union[type1, None]`. Menunjukkan nilai bisa berupa `type1` atau `None`. Sejak Python 3.10, bisa pakai `type1 | None`.
*   `Any`: Menunjukkan tipe apa saja diizinkan (mengabaikan pemeriksaan tipe). Gunakan seminimal mungkin.
*   `Callable[[arg_type1, arg_type2], return_type]`: Untuk fungsi atau objek lain yang bisa dipanggil.
*   `TypeVar`: Untuk mendefinisikan variabel tipe generik.
*   `Iterable`, `Sequence`, `Mapping`: Tipe abstrak untuk berbagai jenis koleksi.

```python
from typing import List, Dict, Tuple, Optional, Union, Callable, Any

# Sebelum Python 3.9/3.10
def proses_nama(daftar_nama: List[str]) -> int:
    print(f"Memproses {len(daftar_nama)} nama.")
    return len(daftar_nama)

def cari_data(id_data: str) -> Optional[Dict[str, Any]]:
    # Anggap fungsi ini mencari data, bisa ketemu (dict) atau tidak (None)
    if id_data == "valid":
        return {"nama": "Data Valid", "nilai": 100}
    else:
        return None

# Menggunakan Union
def format_output(data: Union[str, int, float]) -> str:
    return f"Output: [{data}]"

# Menggunakan Callable
def jalankan_callback(callback: Callable[[int], str], nilai: int):
    hasil_cb = callback(nilai)
    print(f"Hasil callback: {hasil_cb}")

def cb_contoh(x: int) -> str:
    return f"Nilai dikali 2 adalah {x*2}"

jalankan_callback(cb_contoh, 5)

# Menggunakan tipe generik bawaan (Python 3.9+)
def hitung_total(harga: list[float]) -> float:
    return sum(harga)

def get_config(kunci: str) -> str | None: # Python 3.10+
    # ...
    return "nilai" # atau None
```

### Partial Functions (`functools.partial`)

`functools.partial` adalah alat yang berguna untuk membuat **versi baru dari sebuah fungsi** dengan **sebagian argumennya sudah ditetapkan (pre-filled)**. Fungsi baru ini (objek partial) berperilaku seperti fungsi asli tetapi dengan beberapa argumen sudah "terpasang".

Ini berguna ketika Anda ingin meneruskan fungsi sebagai argumen ke fungsi lain (misal, sebagai callback), tetapi fungsi target memerlukan fungsi dengan signature (jumlah/jenis argumen) yang berbeda, atau Anda ingin menyederhanakan pemanggilan fungsi yang sering dipanggil dengan argumen yang sama.

```python
import functools

def power(base, exponent):
  """Menghitung base pangkat exponent."""
  return base ** exponent

# Membuat fungsi baru 'kuadrat' dari 'power' dengan exponent=2
kuadrat = functools.partial(power, exponent=2)

# Membuat fungsi baru 'kubik' dari 'power' dengan exponent=3
kubik = functools.partial(power, exponent=3)

# Membuat fungsi baru 'dua_pangkat' dengan base=2
dua_pangkat = functools.partial(power, 2) # Argumen positional pertama (base) diisi

print(f"\n--- Partial Functions ---")
print(f"Kuadrat dari 5: {kuadrat(5)}") # Hanya perlu beri argumen 'base' -> 25
print(f"Kubik dari 3: {kubik(3)}")   # Hanya perlu beri argumen 'base' -> 27
print(f"Dua pangkat 10: {dua_pangkat(10)}") # Hanya perlu beri argumen 'exponent' -> 1024

# Contoh: Callback dengan argumen berbeda
def proses_event(event_data, callback):
    print(f"\nMemproses event: {event_data}")
    # Callback hanya diharapkan menerima satu argumen (hasil)
    hasil_proses = f"Processed: {event_data.upper()}"
    callback(hasil_proses)

def log_hasil(hasil, level="INFO"): # Fungsi log butuh 'level'
    print(f"[{level}] Hasil diterima: {hasil}")

# Tidak bisa langsung: proses_event("data penting", log_hasil) -> TypeError
# Karena log_hasil butuh argumen 'level'

# Solusi: Gunakan partial untuk membuat callback baru dengan 'level' terpasang
log_info = functools.partial(log_hasil, level="INFO")
log_warning = functools.partial(log_hasil, level="WARNING")

proses_event("data penting", log_info)
proses_event("kesalahan kecil", log_warning)
```

### Enumerations (`enum` modul)

Enumeration (Enum) adalah tipe data khusus yang terdiri dari **sekumpulan nama simbolik (anggota) yang terikat pada nilai unik dan konstan**. Modul `enum` menyediakan kelas dasar `Enum` untuk membuat enumerasi.

**Mengapa Menggunakan Enum?**
*   **Keterbacaan:** Mengganti "magic numbers" atau string literal dengan nama yang bermakna, membuat kode lebih mudah dipahami.
*   **Mencegah Error:** Membatasi nilai yang mungkin untuk suatu variabel ke set anggota enum yang valid, mengurangi risiko typo atau nilai yang tidak valid.
*   **Perbandingan Identitas:** Anggota enum dapat dibandingkan dengan aman menggunakan `is` atau `==`.
*   **Representasi String:** Enum memiliki representasi string default yang informatif.

```python
import enum

# Membuat Enum
class Warna(enum.Enum):
    MERAH = 1 # Nama = nilai
    KUNING = 2
    HIJAU = 3
    BIRU = 4
    # Anda bisa punya nilai duplikat, tapi nama harus unik
    # MERAH_LAIN = 1 # Ini akan menjadi alias untuk MERAH

# Mengakses anggota Enum
warna_lampu = Warna.MERAH
print(f"\n--- Enumerations ---")
print(f"Warna lampu saat ini: {warna_lampu}") # Output: Warna.MERAH
print(f"Nama anggota: {warna_lampu.name}")   # Output: MERAH
print(f"Nilai anggota: {warna_lampu.value}")  # Output: 1

# Iterasi melalui anggota Enum
print("Anggota Warna Enum:")
for warna in Warna:
    print(f"- {warna.name} = {warna.value} ({warna})")

# Perbandingan
if warna_lampu is Warna.MERAH:
    print("Lampu sedang MERAH.")
elif warna_lampu == Warna.HIJAU: # == juga berfungsi
    print("Lampu sedang HIJAU.")

# Mendapatkan anggota dari nilai (jika unik)
warna_dari_nilai_2 = Warna(2)
print(f"Warna dari nilai 2: {warna_dari_nilai_2}") # Output: Warna.KUNING

# Contoh penggunaan dalam fungsi
def deskripsi_warna(warna_input: Warna):
    if not isinstance(warna_input, Warna):
        raise TypeError("Input harus berupa instance Warna Enum")

    if warna_input == Warna.MERAH:
        return "Berhenti!"
    elif warna_input == Warna.KUNING:
        return "Hati-hati!"
    elif warna_input == Warna.HIJAU:
        return "Jalan!"
    else:
        return "Warna tidak dikenal." # Seharusnya tidak terjadi jika pakai Enum

print(f"Deskripsi {Warna.HIJAU}: {deskripsi_warna(Warna.HIJAU)}")
# print(deskripsi_warna("MERAH")) # Akan TypeError

# Enum lain dengan nilai string atau auto()
class Status(enum.Enum):
    PENDING = "pending"
    PROSES = "processing"
    SELESAI = "completed"
    GAGAL = "failed"

class KodeError(enum.Enum):
    OK = enum.auto() # Nilai otomatis (biasanya mulai dari 1)
    TIMEOUT = enum.auto()
    INVALID_REQUEST = enum.auto()
    SERVER_ERROR = enum.auto()

print(f"\nStatus PENDING: {Status.PENDING}, Nilai: {Status.PENDING.value}")
print(f"Kode Error TIMEOUT: {KodeError.TIMEOUT}, Nilai: {KodeError.TIMEOUT.value}") # Output: 2
```
Enum sangat berguna untuk merepresentasikan state, kategori, pilihan, atau konstanta bernama lainnya dalam program Anda.

---

## 12. Pengenalan Pustaka Populer

Ekosistem Python kaya dengan pustaka (library) pihak ketiga yang memperluas kemampuannya secara signifikan. Berikut adalah pengenalan singkat ke beberapa pustaka paling populer di berbagai domain. Menguasai pustaka yang relevan dengan bidang Anda adalah kunci untuk menjadi produktif dengan Python.

### Ilmu Data dan Analisis:

*   **NumPy (Numerical Python):**
    *   **Tujuan:** Pustaka fundamental untuk komputasi numerik di Python.
    *   **Fitur Utama:** Menyediakan objek array multi-dimensi (`ndarray`) yang sangat efisien, fungsi matematika tingkat tinggi untuk beroperasi pada array ini (operasi linear algebra, transformasi Fourier, statistik dasar, random number). Dasar bagi banyak pustaka data science lainnya.
    *   **Contoh:** `import numpy as np; arr = np.array([1, 2, 3]); print(arr * 2)`
*   **Pandas:**
    *   **Tujuan:** Pustaka utama untuk manipulasi dan analisis data.
    *   **Fitur Utama:** Menyediakan struktur data tingkat tinggi dan fleksibel: `Series` (1D array berlabel) dan `DataFrame` (2D tabel data berlabel seperti spreadsheet). Memudahkan pembacaan data dari berbagai format (CSV, Excel, SQL, JSON), pembersihan data (handling missing values), transformasi, penggabungan (merging/joining), pengelompokan (grouping), agregasi, dan analisis data tabular. Sangat terintegrasi dengan NumPy dan Matplotlib.
    *   **Contoh:** `import pandas as pd; df = pd.read_csv("data.csv"); print(df.head())`
*   **Matplotlib:**
    *   **Tujuan:** Pustaka dasar dan paling banyak digunakan untuk membuat visualisasi data statis, animatif, dan interaktif di Python.
    *   **Fitur Utama:** Menyediakan API berorientasi objek dan API berbasis state (mirip MATLAB) untuk membuat berbagai jenis plot (line plot, scatter plot, bar chart, histogram, pie chart, dll.). Sangat dapat disesuaikan. Menjadi dasar bagi banyak pustaka visualisasi lainnya.
    *   **Contoh:** `import matplotlib.pyplot as plt; plt.plot([1, 2, 3], [4, 1, 5]); plt.show()`
*   **Seaborn:**
    *   **Tujuan:** Pustaka visualisasi data berbasis Matplotlib yang menyediakan antarmuka tingkat tinggi untuk menggambar plot statistik yang menarik dan informatif.
    *   **Fitur Utama:** Memudahkan pembuatan plot statistik kompleks (seperti distribution plots, categorical plots, regression plots, matrix plots) dengan kode yang lebih sedikit. Memiliki tema default yang estetis. Bekerja sangat baik dengan Pandas DataFrames.
    *   **Contoh:** `import seaborn as sns; data = sns.load_dataset("tips"); sns.scatterplot(data=data, x="total_bill", y="tip"); plt.show()`

### Pengembangan Web (Backend):

*   **Flask:**
    *   **Tujuan:** Kerangka kerja web mikro (microframework). Disebut "mikro" karena intinya kecil dan tidak memaksakan banyak struktur atau dependensi eksternal.
    *   **Fitur Utama:** Memberikan dasar-dasar routing (memetakan URL ke fungsi Python), request handling, templating (biasanya dengan Jinja2), dan manajemen sesi. Sangat fleksibel, mudah dipelajari untuk proyek kecil hingga menengah, dan memungkinkan Anda memilih komponen tambahan (seperti ORM, form validation) sesuai kebutuhan.
    *   **Contoh:**
        ```python
        # from flask import Flask
        # app = Flask(__name__)
        # @app.route('/')
        # def hello(): return "Halo, Dunia Flask!"
        # if __name__ == '__main__': app.run()
        ```
*   **Django:**
    *   **Tujuan:** Kerangka kerja web tingkat tinggi (high-level framework) yang mengikuti filosofi "batteries-included".
    *   **Fitur Utama:** Menyediakan hampir semua yang Anda butuhkan untuk membangun aplikasi web kompleks secara out-of-the-box: ORM (Object-Relational Mapper) yang kuat, sistem migrasi database, panel admin otomatis, sistem routing, templating engine, autentikasi pengguna, form handling, security features (CSRF, XSS protection), dll. Lebih beropini (opinionated) tentang struktur proyek tetapi mempromosikan pengembangan cepat (Rapid Application Development). Cocok untuk proyek besar dan kompleks.
    *   **Struktur:** Biasanya melibatkan pembuatan "apps" Django yang modular.

### Permintaan HTTP:

*   **Requests:**
    *   **Tujuan:** Membuat permintaan HTTP (GET, POST, PUT, DELETE, dll.) menjadi sangat mudah dan manusiawi.
    *   **Fitur Utama:** Menyederhanakan interaksi dengan API web atau pengambilan konten web. Mengelola detail HTTP seperti koneksi, pengiriman data (JSON, form), penanganan header, cookie, autentikasi, verifikasi SSL, dan penanganan respons (status code, content) dengan API yang sangat intuitif. Jauh lebih mudah digunakan daripada modul `urllib` bawaan untuk sebagian besar kasus penggunaan.
    *   **Contoh:** `import requests; response = requests.get('https://api.github.com'); print(response.status_code); print(response.json())`

### Web Scraping:

*   **Beautiful Soup 4 (bs4):**
    *   **Tujuan:** Pustaka untuk menarik (parsing) data dari file HTML dan XML.
    *   **Fitur Utama:** Mengubah dokumen HTML/XML yang mungkin berantakan menjadi struktur pohon (parse tree) yang dapat dinavigasi dengan mudah. Menyediakan cara idiomatik untuk mencari, menavigasi, dan memodifikasi parse tree menggunakan tag HTML/XML, atribut, dan teks. Bekerja bersama pustaka seperti `requests` (untuk mengunduh halaman web) dan parser seperti `html.parser` (bawaan) atau `lxml`.
    *   **Contoh:** `from bs4 import BeautifulSoup; soup = BeautifulSoup(html_doc, 'html.parser'); print(soup.title.string)`
*   **Scrapy:**
    *   **Tujuan:** Kerangka kerja (framework) yang lengkap untuk web crawling dan scraping.
    *   **Fitur Utama:** Menyediakan arsitektur yang kuat untuk membangun "spider" (bot) yang dapat menjelajahi situs web secara otomatis, mengekstrak data terstruktur (items), dan menyimpannya dalam berbagai format. Menangani banyak aspek kompleks seperti request scheduling, concurrency, user-agent spoofing, proxy handling, dan mengikuti `robots.txt`. Lebih kompleks daripada Requests+BeautifulSoup tetapi jauh lebih kuat untuk tugas scraping skala besar.

### Pengujian (Testing):

*   **unittest:**
    *   **Tujuan:** Kerangka kerja pengujian unit (unit testing) yang **bawaan** Python.
    *   **Fitur Utama:** Terinspirasi dari xUnit (JUnit). Menyediakan kelas dasar (`unittest.TestCase`) dengan metode assertion (`assertEqual`, `assertTrue`, `assertRaises`, dll.), mekanisme test discovery, test fixtures (setup/teardown), dan test runner untuk mengorganisir dan menjalankan tes. Sedikit lebih banyak boilerplate code dibandingkan pytest.
*   **pytest:**
    *   **Tujuan:** Kerangka kerja pengujian yang sangat populer dan kuat, sering dianggap lebih mudah digunakan dan lebih Pythonic daripada `unittest`.
    *   **Fitur Utama:** Menggunakan fungsi tes biasa (bukan kelas `TestCase`), assertion `assert` bawaan Python (dengan introspeksi cerdas untuk pesan error yang detail), sistem fixtures yang sangat fleksibel (menggunakan decorator `@pytest.fixture`), test discovery yang kuat, banyak plugin, dan output yang berwarna/informatif. Seringkali membutuhkan lebih sedikit kode untuk menulis tes yang sama dibandingkan `unittest`.

---

**\*Catatan:** Ini hanya pengenalan singkat, setiap pustaka memerlukan pembelajaran lebih lanjut\*. Dokumentasi resmi masing-masing pustaka adalah sumber terbaik. Memilih pustaka yang tepat tergantung pada kebutuhan spesifik proyek Anda.

---

## 13. Praktik Terbaik dan Gaya Kode

Menulis kode Python yang berfungsi saja tidak cukup. Kode yang baik juga harus **mudah dibaca, dipahami, dipelihara, dan konsisten**. Mengikuti praktik terbaik dan panduan gaya kode (style guide) sangat penting, terutama saat bekerja dalam tim atau pada proyek jangka panjang.

### PEP 8 - Panduan Gaya Kode Python

**PEP 8 (Python Enhancement Proposal 8)** adalah **panduan gaya kode resmi** untuk kode Python di pustaka standar. Ini adalah dokumen yang sangat penting dan diadopsi secara luas oleh komunitas Python. Mengikuti PEP 8 membuat kode Anda terlihat profesional dan konsisten dengan kode Python lainnya.

Beberapa poin utama PEP 8:

*   **Indentasi:** Gunakan **4 spasi** per level indentasi. **Jangan gunakan tab**, atau jika harus (misalnya karena codebase lama), jangan campur aduk tab dan spasi. Editor kode modern biasanya dapat dikonfigurasi untuk otomatis mengubah tab menjadi 4 spasi.
*   **Panjang Baris Maksimum:** Batasi semua baris hingga **maksimal 79 karakter**. Untuk docstrings atau komentar, batasi hingga 72 karakter. Ini meningkatkan keterbacaan, terutama pada layar yang lebih kecil atau saat menampilkan beberapa file berdampingan. Gunakan pemisah baris implisit Python di dalam tanda kurung `()`, kurung siku `[]`, atau kurung kurawal `{}` untuk memecah baris panjang, atau gunakan backslash `\` (kurang disukai).
*   **Baris Kosong:** Gunakan baris kosong untuk memisahkan fungsi dan kelas tingkat atas (dua baris kosong), metode di dalam kelas (satu baris kosong), dan untuk memisahkan grup logika di dalam fungsi (satu baris kosong, gunakan secukupnya).
*   **Impor (`import`):**
    *   Impor harus selalu berada di bagian atas file, setelah komentar modul dan docstring, dan sebelum konstanta atau variabel global.
    *   Urutkan impor dalam grup: 1. Impor pustaka standar, 2. Impor pustaka pihak ketiga terkait, 3. Impor modul lokal aplikasi Anda. Pisahkan setiap grup dengan baris kosong.
    *   Hindari `import *` (kecuali ada alasan kuat).
    *   Impor absolut lebih disukai daripada impor relatif untuk sebagian besar kasus di luar paket itu sendiri.
*   **Whitespace dalam Ekspresi dan Pernyataan:**
    *   Gunakan spasi di sekitar sebagian besar operator (`=`, `+=`, `==`, `<`, `>`, `in`, `is`, `and`, `or`, `not`).
    *   Jangan gunakan spasi tepat di dalam tanda kurung/siku/kurawal: `spam(ham[1], {eggs: 2})` (benar), `spam( ham[ 1 ], { eggs: 2 } )` (salah).
    *   Jangan gunakan spasi sebelum koma, titik koma, atau titik dua: `if x == 4: print(x, y); x, y = y, x` (benar).
    *   Gunakan spasi setelah koma: `[1, 2, 3]`.
    *   Tidak perlu spasi di sekitar `=` saat digunakan untuk argumen keyword atau nilai parameter default: `def func(arg1, arg2=None): ...` ; `func(1, arg2=2)`.
*   **Komentar:**
    *   Komentar harus berupa kalimat lengkap dan jelas.
    *   Komentar inline (`#` di akhir baris kode) harus digunakan secukupnya dan dipisahkan setidaknya dua spasi dari pernyataan. Jelaskan *mengapa*, bukan *apa* yang dilakukan kode (jika kodenya sudah jelas).
    *   Komentar blok (`#` di baris terpisah sebelum kode) harus sejajar dengan indentasi kode yang dijelaskannya.
    *   Gunakan **docstrings** (string dokumentasi `"""..."""`) untuk mendokumentasikan modul, fungsi, kelas, dan metode publik.
    *   Jaga komentar tetap *up-to-date* saat kode berubah.
*   **Penamaan (Konvensi Penting):**
    *   **Modul:** Nama pendek, huruf kecil semua, bisa pakai underscore jika perlu (`nama_modul.py`).
    *   **Paket:** Nama pendek, huruf kecil semua (`nama_paket/`). Hindari underscore.
    *   **Kelas:** `CamelCase` (atau `CapWords`) (misal `NamaKelasSaya`).
    *   **Exception:** `CamelCase` dan sebaiknya diakhiri `Error` (misal `CustomValueError`).
    *   **Fungsi:** `snake_case` (huruf kecil semua, dipisah underscore) (misal `hitung_total_harga`).
    *   **Variabel:** `snake_case` (misal `nama_pengguna`, `total_sementara`).
    *   **Metode:** `snake_case` (sama seperti fungsi).
    *   **Konstanta:** `UPPER_SNAKE_CASE` (huruf kapital semua, dipisah underscore) (misal `PI = 3.14`, `BATAS_MAKSIMUM = 100`).
    *   **Nama Internal/Protected:** Diawali satu underscore (`_nama_internal`).
    *   **Nama Private (Name Mangling):** Diawali dua underscore (`__nama_private`). Hindari jika tidak benar-benar perlu.
*   **Rekomendasi Pemrograman:**
    *   Bandingkan dengan `None` menggunakan `is` atau `is not` (`if var is None:`), bukan `==`.
    *   Gunakan `isinstance()` untuk memeriksa tipe objek, bukan `type() == ...` (karena `isinstance` menangani inheritance).
    *   Jangan bandingkan boolean dengan `== True` atau `== False` (redundant). Gunakan `if var:` atau `if not var:`.
    *   Untuk sequence (string, list, tuple), gunakan fakta bahwa sequence kosong adalah false: `if not my_list:` lebih baik dari `if len(my_list) == 0:`.

Bacalah [PEP 8](https://peps.python.org/pep-0008/) secara lengkap untuk detailnya. Sebagian besar IDE dan linter dapat membantu Anda memeriksa kepatuhan terhadap PEP 8.

### Menulis Kode yang Pythonic

"Pythonic" mengacu pada penulisan kode yang memanfaatkan fitur-fitur unik dan idiom bahasa Python secara efektif, sehingga menghasilkan kode yang tidak hanya berfungsi tetapi juga bersih, mudah dibaca, dan efisien. Ini seringkali kontras dengan menerjemahkan gaya dari bahasa lain (seperti C atau Java) langsung ke Python.

Beberapa contoh gaya Pythonic:

*   **Memanfaatkan Struktur Data Bawaan:** Gunakan list, tuple, dict, dan set secara tepat sesuai kebutuhan. Misalnya, gunakan set untuk keanggotaan cepat atau keunikan, dict untuk pemetaan kunci-nilai.
*   **Menggunakan Comprehensions dan Generator:** Lebih disukai daripada loop `for` dengan `append()` untuk membuat list/set/dict, atau loop manual untuk iterasi sederhana, karena lebih ringkas dan seringkali lebih cepat. Gunakan generator untuk efisiensi memori.
*   **Iterasi Langsung:** Lakukan iterasi langsung pada iterable (`for item in my_list:`) daripada menggunakan indeks (`for i in range(len(my_list)): item = my_list[i]`), kecuali Anda benar-benar memerlukan indeks (gunakan `enumerate()` jika perlu keduanya).
*   **Tuple Unpacking:** Gunakan unpacking untuk menugaskan nilai dari sequence atau menukar variabel (`a, b = b, a`).
*   **Menggunakan `with` untuk Context Management:** Selalu gunakan `with open(...)` atau context manager lain untuk sumber daya yang perlu cleanup.
*   **Duck Typing:** Andalkan perilaku (metode) objek daripada memeriksa tipenya secara eksplisit jika memungkinkan.
*   **Penanganan Error Pythonic:** Gunakan `try...except` untuk menangani error yang *diharapkan* terjadi (EAFP - Easier to Ask for Forgiveness than Permission), daripada memeriksa kondisi terlebih dahulu (LBYL - Look Before You Leap), terutama jika kondisi error jarang terjadi.
    ```python
    # Kurang Pythonic (LBYL)
    if key in my_dict:
        value = my_dict[key]
        # proses value
    else:
        # handle key tidak ada

    # Lebih Pythonic (EAFP)
    try:
        value = my_dict[key]
        # proses value
    except KeyError:
        # handle key tidak ada

    # Atau pakai get() jika hanya perlu nilai default
    value = my_dict.get(key, default_value)
    if value is not None: # Atau cek jika bukan default_value
        # proses value
    ```
*   **Menghindari Pengulangan Kode (DRY - Don't Repeat Yourself):** Gunakan fungsi, kelas, dan modul untuk mengabstraksi logika yang berulang.
*   **Menulis Kode yang Mudah Dibaca dan Dipelihara:** Prioritaskan kejelasan daripada kecerdasan kode yang berlebihan. Gunakan nama variabel/fungsi yang deskriptif. Tambahkan komentar dan docstring yang berguna. Ikuti PEP 8.

"The Zen of Python" (`import this`) merangkum banyak filosofi di balik kode Pythonic.

### Alat Bantu (Linters dan Formatters)

Menggunakan alat bantu otomatis dapat sangat meningkatkan kualitas dan konsistensi kode Anda:

1.  **Linters (Penganalisis Kode Statis):** Menganalisis kode Anda *tanpa menjalankannya* untuk mendeteksi:
    *   Kesalahan sintaks.
    *   Potensi bug (misalnya, variabel tidak terdefinisi, impor tidak digunakan).
    *   Pelanggaran gaya kode (PEP 8).
    *   Kode yang terlalu kompleks atau "code smells".
    *   **Contoh Populer:**
        *   **Flake8:** Cepat, menggabungkan Pyflakes (cek error logika), Pycodestyle (cek gaya PEP 8), dan McCabe (cek kompleksitas). Sangat umum digunakan.
        *   **Pylint:** Lebih komprehensif dan dapat dikonfigurasi daripada Flake8. Melakukan analisis yang lebih mendalam, memberikan skor kode, dan bisa sangat cerewet (banyak saran), tetapi sangat membantu untuk meningkatkan kualitas kode.
        *   **Mypy:** Linter khusus untuk memeriksa *type hints*.

2.  **Formatters (Pemformat Kode Otomatis):** Mengatur ulang format kode Anda secara otomatis agar sesuai dengan panduan gaya tertentu, menghilangkan perdebatan tentang gaya dan memastikan konsistensi.
    *   **Contoh Populer:**
        *   **Black:** Pemformat yang sangat "beropini" (tidak banyak konfigurasi). Memformat kode dengan gaya yang konsisten (sub-set dari PEP 8). Tujuannya adalah mengakhiri perdebatan tentang format. Sangat populer.
        *   **YAPF (Yet Another Python Formatter):** Dibuat oleh Google. Lebih dapat dikonfigurasi daripada Black, mencoba mencocokkan gaya kode asli sambil membuatnya sesuai PEP 8.
        *   **autopep8:** Fokus hanya memperbaiki pelanggaran PEP 8.

**Cara Menggunakan:**
*   Alat-alat ini biasanya diinstal via `pip` (`pip install flake8 black mypy`).
*   Dapat dijalankan dari baris perintah (`flake8 .`, `black .`, `mypy src/`).
*   Sangat direkomendasikan untuk **mengintegrasikannya dengan editor kode/IDE Anda**. Sebagian besar editor memiliki ekstensi/plugin untuk menjalankan linter/formatter secara otomatis saat menyimpan file atau sebagai bagian dari alur kerja pengembangan Anda.
*   Konfigurasi (misalnya, file `pyproject.toml`, `.flake8`) memungkinkan penyesuaian aturan.

Menggunakan kombinasi linter (seperti Flake8/Pylint + Mypy) dan formatter (seperti Black) adalah praktik standar dalam pengembangan Python modern.

### Manajemen Ketergantungan (Dependency Management)

Proyek Python seringkali bergantung pada pustaka pihak ketiga. Mengelola dependensi ini dengan benar sangat penting untuk reproduktifitas dan kolaborasi.

*   **Lingkungan Virtual (`venv`):** Seperti dibahas sebelumnya, ini adalah **dasar** dari manajemen dependensi yang baik. Isolasi dependensi per proyek.
*   **`requirements.txt`:** Cara standar (dan paling dasar) untuk mencatat dependensi proyek.
  *   Dihasilkan dengan `pip freeze > requirements.txt` di dalam venv aktif.
    *   Berisi daftar paket dan versi **tepat** yang terinstal saat itu. Ini memastikan orang lain (atau Anda di mesin lain) dapat menginstal versi yang sama persis menggunakan `pip install -r requirements.txt`, menghasilkan lingkungan yang dapat direproduksi.
    *   **Kelemahan:** Tidak secara eksplisit memisahkan dependensi level atas (yang Anda impor langsung) dari dependensi transitif (yang dibutuhkan oleh dependensi Anda). Juga tidak mengelola versi Python itu sendiri.
*   **Alat seperti Poetry atau Pipenv (Opsional Lanjutan):** Alat yang lebih modern dan canggih yang mencoba mengatasi beberapa keterbatasan `pip` + `venv` + `requirements.txt`.
    *   **Fitur Umum:**
        *   Mengelola dependensi proyek dan dependensi pengembangan (misal, untuk testing/linting) secara terpisah.
        *   Menggunakan file konfigurasi sentral (misal `pyproject.toml` untuk Poetry, `Pipfile` untuk Pipenv).
        *   Membuat "lock file" (misal `poetry.lock`, `Pipfile.lock`) yang mencatat *pohon dependensi lengkap* dengan versi yang tepat (termasuk dependensi transitif), memastikan build yang lebih deterministik.
        *   Mengelola lingkungan virtual secara otomatis.
        *   Membantu dalam pembuatan dan penerbitan paket Python.
    *   **Kapan Digunakan?** Sangat berguna untuk proyek aplikasi atau library yang lebih besar, terutama saat kolaborasi tim atau kebutuhan build yang konsisten sangat penting. Memiliki kurva belajar yang sedikit lebih tinggi daripada `pip` + `venv`.

### Kontrol Versi dengan Git

Kontrol versi adalah praktik fundamental dalam pengembangan perangkat lunak modern, dan **Git** adalah sistem kontrol versi terdistribusi yang paling populer dan dominan saat ini. Menggunakan Git (biasanya bersama platform hosting seperti GitHub, GitLab, Bitbucket) sangat penting untuk:

*   **Melacak Perubahan:** Menyimpan riwayat lengkap setiap perubahan yang dibuat pada kode Anda. Anda bisa melihat siapa mengubah apa, kapan, dan mengapa.
*   **Kembali ke Versi Sebelumnya:** Jika terjadi kesalahan atau Anda ingin mengembalikan perubahan, mudah untuk kembali ke versi kode yang stabil sebelumnya.
*   **Kolaborasi Tim:** Memungkinkan banyak pengembang bekerja pada basis kode yang sama secara bersamaan tanpa saling menimpa pekerjaan. Git membantu menggabungkan (merge) perubahan dari berbagai kontributor.
*   **Percabangan (Branching):** Membuat "cabang" terpisah dari kode utama untuk mengerjakan fitur baru atau memperbaiki bug tanpa mengganggu versi stabil (biasanya cabang `main` atau `master`). Setelah selesai, cabang dapat digabungkan kembali.
*   **Backup:** Platform hosting Git (seperti GitHub) bertindak sebagai backup terpusat untuk kode Anda.

#### Mengapa Git Penting?

Tanpa kontrol versi, Anda mungkin berakhir dengan banyak salinan file (`script_v1.py`, `script_v2_final.py`, `script_final_banget.py`), sulit melacak perubahan, dan kolaborasi menjadi mimpi buruk. Git menyediakan cara yang terstruktur dan kuat untuk mengelola evolusi kode Anda.

#### Perintah Dasar Git (Pengenalan Singkat)

(Diasumsikan Git sudah terinstal. Jalankan di terminal/command prompt di dalam direktori proyek Anda).

1.  **`git init`**: Menginisialisasi repositori Git baru di direktori saat ini. Membuat direktori `.git` tersembunyi untuk menyimpan riwayat. Lakukan ini hanya sekali per proyek.
2.  **`git status`**: Menampilkan status file di direktori kerja Anda (file mana yang baru, dimodifikasi, atau siap di-commit). Sangat sering digunakan.
3.  **`git add <nama_file>`** atau **`git add .`**: Menambahkan perubahan pada file (atau semua perubahan di direktori saat ini dengan `.`) ke area *staging*. Area staging adalah tempat Anda mempersiapkan perubahan yang akan dimasukkan dalam *commit* berikutnya.
4.  **`git commit -m "Pesan commit yang deskriptif"`**: Menyimpan snapshot permanen dari perubahan yang ada di area staging ke riwayat repositori. **Pesan commit sangat penting**; jelaskan *mengapa* perubahan dibuat, bukan hanya *apa*.
5.  **`git log`**: Menampilkan riwayat commit, dari yang terbaru hingga terlama. Tekan `q` untuk keluar.
6.  **`git branch`**: Menampilkan daftar semua cabang (branch) di repositori Anda. Cabang aktif ditandai dengan `*`.
7.  **`git branch <nama_cabang_baru>`**: Membuat cabang baru.
8.  **`git checkout <nama_cabang>`** atau **`git switch <nama_cabang>`** (lebih baru): Berpindah ke cabang lain. Direktori kerja Anda akan diperbarui sesuai dengan snapshot terakhir di cabang tersebut.
9.  **`git merge <nama_cabang_sumber>`**: Menggabungkan perubahan dari `nama_cabang_sumber` ke cabang Anda saat ini. Mungkin menimbulkan *konflik* jika perubahan pada file yang sama terjadi di kedua cabang, yang perlu diselesaikan manual.
10. **`git remote add origin <url_repositori_remote>`**: Menghubungkan repositori lokal Anda ke repositori remote (misalnya di GitHub). `origin` adalah nama alias standar untuk remote utama. Lakukan sekali per proyek.
11. **`git push origin <nama_cabang>`**: Mengirim commit dari cabang lokal Anda ke repositori remote (`origin`).
12. **`git pull origin <nama_cabang>`**: Mengambil (fetch) perubahan terbaru dari cabang di repositori remote (`origin`) dan mencoba menggabungkannya (merge) ke cabang lokal Anda saat ini.

Ini hanyalah puncak gunung es Git. Ada banyak konsep dan perintah lain (rebase, stash, tag, dll.). Sangat disarankan untuk mempelajari Git lebih dalam melalui tutorial atau buku khusus.

---

## 14. Ide Proyek untuk Latihan

Cara terbaik untuk benar-benar memahami dan menguasai Python adalah dengan **mempraktikkannya melalui proyek**. Mulailah dari yang sederhana dan tingkatkan kompleksitasnya seiring bertambahnya pemahaman Anda. Berikut beberapa ide proyek yang dikategorikan berdasarkan tingkat kesulitan:

### Tingkat Pemula:

Fokus pada dasar-dasar: variabel, tipe data, operator, input/output, kontrol alur (`if`, `for`, `while`), fungsi sederhana, string, dan mungkin list dasar.

1.  **Kalkulator Sederhana:** Program yang meminta dua angka dan satu operator (+, -, \*, /) dari pengguna, lalu menampilkan hasilnya.
2.  **Game Tebak Angka:** Program menghasilkan angka acak, lalu pengguna mencoba menebaknya. Program memberikan petunjuk ("terlalu tinggi", "terlalu rendah") sampai angka berhasil ditebak. Hitung jumlah tebakan.
3.  **Konverter Satuan:** Program untuk mengonversi antar satuan, misalnya:
    *   Suhu (Celcius ke Fahrenheit dan sebaliknya).
    *   Panjang (Meter ke Kaki, Kilometer ke Mil).
    *   Berat (Kilogram ke Pon).
4.  **Generator Kata Sandi Sederhana:** Program yang menghasilkan kata sandi acak dengan panjang tertentu, mungkin dengan opsi untuk menyertakan huruf besar, huruf kecil, angka, dan simbol.
5.  **Batu-Gunting-Kertas:** Implementasi game klasik melawan komputer. Komputer memilih secara acak, pengguna memasukkan pilihannya, lalu program menentukan pemenangnya.

### Tingkat Menengah:

Melibatkan struktur data yang lebih kompleks (list, dict, set, tuple), fungsi yang lebih maju, penanganan file, modul, penanganan error, dan mungkin dasar-dasar OOP.

1.  **Aplikasi Todo List (Simpan ke File):** Program baris perintah (command-line) untuk mengelola daftar tugas. Fitur: tambah tugas, lihat semua tugas, tandai tugas selesai, hapus tugas. Simpan daftar tugas ke file teks, CSV, atau JSON agar data tetap ada saat program ditutup dan dibuka lagi.
2.  **Web Scraper Sederhana:** Menggunakan pustaka `requests` untuk mengunduh halaman web dan `BeautifulSoup4` untuk mengekstrak informasi spesifik, misalnya:
    *   Judul semua artikel berita dari halaman utama situs berita.
    *   Harga produk dari halaman e-commerce sederhana.
    *   Judul dan penulis kutipan dari situs kutipan.
3.  **Pengelola Kontak Sederhana:** Program untuk menyimpan dan mengelola informasi kontak (nama, nomor telepon, email). Simpan data ke file (misal, CSV atau JSON). Fitur: tambah kontak, cari kontak, lihat semua kontak, hapus kontak.
4.  **Jam Pomodoro di Terminal:** Aplikasi timer yang mengimplementasikan Teknik Pomodoro (misalnya, 25 menit kerja, 5 menit istirahat pendek, diulang beberapa kali, lalu istirahat panjang). Berikan notifikasi visual atau suara (opsional) di terminal.
5.  **Penganalisis Teks Sederhana:** Program yang membaca file teks dan menghitung statistik seperti:
    *   Jumlah total kata.
    *   Jumlah kalimat.
    *   Frekuensi setiap kata (berapa kali muncul).
    *   Frekuensi setiap huruf.

### Tingkat Lanjut:

Memanfaatkan OOP secara lebih ekstensif, menggunakan pustaka eksternal/framework, menangani konsep yang lebih kompleks seperti API, database, atau GUI dasar.

1.  **Aplikasi Web Sederhana dengan Flask/Django:** Membuat aplikasi web kecil, misalnya:
    *   Blog sederhana: Pengguna bisa melihat postingan, mungkin menambahkan postingan baru (memerlukan database sederhana seperti SQLite).
    *   URL Shortener: Mengambil URL panjang dan menghasilkan URL pendek yang mengarah ke URL asli.
    *   Aplikasi polling sederhana.
2.  **Bot Otomatisasi:** Membuat bot yang berinteraksi dengan platform lain:
    *   Bot Twitter sederhana yang memposting tweet terjadwal atau merespons mention (menggunakan API Twitter dan library seperti `tweepy`).
    *   Bot Discord sederhana yang merespons perintah di server (menggunakan `discord.py`).
    *   Skrip otomatisasi tugas di komputer Anda (misalnya, merapikan file unduhan, mengganti nama file secara massal).
3.  **Alat Visualisasi Data Kecil:** Mengambil data dari file CSV atau API publik, memprosesnya menggunakan Pandas, dan membuat beberapa plot/grafik menarik menggunakan Matplotlib atau Seaborn. Sajikan hasilnya dalam laporan atau halaman web sederhana.
4.  **Game Sederhana dengan Pygame:** Membuat game 2D sederhana menggunakan pustaka `pygame`, misalnya:
    *   Game Pong.
    *   Game Snake.
    *   Space Invaders sederhana.
5.  **API Sederhana:** Membuat API (Application Programming Interface) sendiri menggunakan Flask atau Django (atau FastAPI) yang menyediakan data (misalnya, dari database atau sumber lain) dalam format JSON sebagai respons terhadap permintaan HTTP.

Pilihlah proyek yang menarik minat Anda! Proses belajar akan lebih menyenangkan jika Anda mengerjakan sesuatu yang Anda sukai. Jangan takut untuk memulai dari yang kecil dan menambahkan fitur secara bertahap. Mencari solusi online (Stack Overflow, dokumentasi) saat Anda mengalami kesulitan adalah bagian normal dari proses belajar.

---

## 15. Topik Lanjutan (Sekilas Pandang)

Setelah Anda merasa nyaman dengan topik-topik menengah, dunia Python masih menawarkan banyak area lanjutan untuk dijelajahi, tergantung pada minat dan jalur karier Anda. Berikut sekilas beberapa di antaranya:

*   **Asynchronous I/O (`asyncio`):** Paradigma pemrograman untuk menangani operasi I/O (seperti jaringan, akses disk) yang memakan waktu tanpa memblokir eksekusi program utama. Menggunakan `async` dan `await` untuk menulis kode konkuren yang efisien, sangat penting untuk aplikasi jaringan berperforma tinggi (server web, bot, klien API).
*   **Multithreading dan Multiprocessing:** Cara lain untuk mencapai konkurensi (menjalankan beberapa tugas seolah-olah bersamaan) atau paralelisme (menjalankan beberapa tugas secara harfiah bersamaan di beberapa inti CPU).
    *   `threading`: Menjalankan beberapa thread dalam satu proses. Terbatas oleh Global Interpreter Lock (GIL) untuk tugas CPU-bound di CPython, tetapi berguna untuk I/O-bound.
    *   `multiprocessing`: Menjalankan beberapa proses terpisah, masing-masing dengan interpreter Python dan memori sendiri. Dapat memanfaatkan beberapa inti CPU secara penuh untuk tugas CPU-bound, tetapi komunikasi antar proses lebih kompleks.
*   **Metaprogramming (Metaclasses):** Teknik tingkat lanjut di mana program dapat memanipulasi dirinya sendiri (atau program lain) sebagai datanya. Metaclasses adalah "kelas dari kelas", memungkinkan Anda mengontrol *bagaimana* kelas dibuat. Digunakan dalam framework kompleks, ORM, atau untuk implementasi pola desain tingkat lanjut. Memiliki kurva belajar yang curam.
*   **Descriptors:** Protokol Python yang memungkinkan Anda menyesuaikan apa yang terjadi ketika atribut objek diakses, diatur, atau dihapus. Mekanisme di balik cara kerja `@property`, `@classmethod`, dan `@staticmethod`. Memungkinkan kontrol yang sangat halus atas akses atribut.
*   **Interaksi dengan C/C++ (`ctypes`, `Cython`, dll.):** Cara untuk mengintegrasikan kode Python dengan kode C atau C++:
    *   `ctypes`: Memuat dan memanggil fungsi dari pustaka C dinamis (DLL/.so) langsung dari Python.
    *   `Cython`: Bahasa superset dari Python yang memungkinkan Anda menambahkan anotasi tipe statis dan dikompilasi menjadi modul ekstensi C yang sangat cepat. Berguna untuk mengoptimalkan bagian kode Python yang kritis performa (CPU-bound).
    *   Python C API: Antarmuka tingkat rendah untuk menulis modul ekstensi C/C++ untuk Python.
*   **Packaging dan Distribusi Kode:** Mempelajari cara mengemas (package) library atau aplikasi Python Anda agar dapat didistribusikan ke pengguna lain (misalnya melalui PyPI) atau di-deploy ke server. Melibatkan alat seperti `setuptools`, `wheel`, dan mungkin `Poetry` atau `flit`, serta memahami struktur file `pyproject.toml`.

Topik-topik ini biasanya dipelajari setelah fondasi yang kuat terbentuk dan seringkali didorong oleh kebutuhan proyek spesifik.

---

## 16. Sumber Belajar Lebih Lanjut

Perjalanan belajar pemrograman adalah proses berkelanjutan. Panduan ini memberikan fondasi yang komprehensif, tetapi selalu ada lebih banyak hal untuk dipelajari. Berikut adalah beberapa sumber daya tambahan yang sangat direkomendasikan:

*   **Dokumentasi Python Resmi:** ([https://docs.python.org/3/](https://docs.python.org/3/))
    *   **Tutorial:** Pengantar resmi yang sangat baik.
    *   **Library Reference:** Referensi lengkap untuk semua modul di pustaka standar.
    *   **Language Reference:** Penjelasan mendalam tentang sintaks dan semantik bahasa Python.
    *   **Python HOWTOs:** Panduan praktis untuk topik-topik spesifik.
    *   Ini adalah sumber **paling akurat dan otoritatif**. Biasakan untuk merujuk ke sini.
*   **Buku Rekomendasi:**
    *   **Untuk Pemula:**
        *   *Python Crash Course* oleh Eric Matthes: Pendekatan berbasis proyek yang sangat populer.
        *   *Automate the Boring Stuff with Python* oleh Al Sweigart (Tersedia gratis online): Fokus pada otomatisasi tugas praktis.
        *   *Head First Python* oleh Paul Barry: Gaya belajar visual dan interaktif.
    *   **Untuk Menengah/Lanjut:**
        *   *Fluent Python* oleh Luciano Ramalho: Pembahasan mendalam tentang fitur inti Python dan cara menulis kode Pythonic. Sangat direkomendasikan setelah menguasai dasar.
        *   *Python Cookbook* oleh David Beazley & Brian K. Jones: Kumpulan resep (solusi) untuk berbagai masalah pemrograman Python.
        *   *Effective Python* oleh Brett Slatkin: Tips praktis untuk menulis kode Python yang lebih baik.
*   **Kursus Online:**
    *   **Coursera:** Menawarkan kursus dan spesialisasi dari universitas ternama (misal, University of Michigan's Python for Everybody).
    *   **edX:** Platform lain dengan kursus dari universitas dan institusi (misal, MITx, HarvardX).
    *   **Udemy:** Pasar kursus online dengan banyak pilihan kursus Python untuk berbagai tingkat dan topik.
    *   **Codecademy:** Platform belajar interaktif dengan jalur karier Python.
    *   **DataCamp:** Fokus pada ilmu data dengan Python dan R, pembelajaran interaktif.
    *   **Google's Python Class:** (Gratis) Materi kuliah dan latihan dari Google.
*   **Platform Latihan Koding:**
    *   **HackerRank:** Latihan pemrograman, persiapan wawancara, kompetisi.
    *   **LeetCode:** Fokus pada soal-soal algoritma dan struktur data, populer untuk persiapan wawancara teknis.
    *   **Codewars:** Latihan "kata" (tantangan pemrograman kecil) dengan berbagai tingkat kesulitan, solusi dapat dibandingkan dengan komunitas.
    *   **Exercism:** (Gratis) Latihan dengan bimbingan mentor (opsional).
*   **Komunitas:**
    *   **Stack Overflow:** Tempat bertanya dan mencari jawaban untuk masalah pemrograman spesifik. Cari sebelum bertanya!
    *   **Reddit:**
        *   `r/learnpython`: Komunitas yang sangat membantu untuk pemula bertanya.
        *   `r/Python`: Diskusi umum tentang Python, berita, proyek.
    *   **Forum Diskusi Lokal/Online:** Cari komunitas Python di daerah Anda atau forum online lainnya. Bertemu dan berdiskusi dengan programmer lain sangat bermanfaat.
    *   **Konferensi Python (PyCon):** Jika memungkinkan, hadiri konferensi PyCon global atau lokal untuk belajar dari para ahli dan bertemu komunitas.

---

## 17. Kesimpulan dan Langkah Selanjutnya

Selamat! Anda telah menyelesaikan panduan komprehensif ini. Anda sekarang memiliki pemahaman yang kuat tentang dasar-dasar hingga konsep menengah dalam pemrograman Python, termasuk sintaks, struktur data, fungsi, OOP, penanganan error, modul, I/O file, dan pengenalan ke beberapa topik serta alat penting lainnya.

Namun, belajar pemrograman adalah sebuah maraton, bukan sprint. Kunci sebenarnya untuk menjadi mahir adalah **konsistensi dan praktik**.

**Langkah Selanjutnya:**

1.  **Terus Berlatih!**
    *   Kerjakan lebih banyak **proyek pribadi**. Pilih sesuatu yang menarik minat Anda. Mulai dari yang kecil, lalu tambahkan kompleksitas secara bertahap.
    *   Selesaikan tantangan koding di platform seperti HackerRank, LeetCode, atau Codewars untuk mengasah kemampuan pemecahan masalah dan algoritma Anda.
    *   Tinjau kembali kode lama Anda. Bisakah Anda membuatnya lebih baik, lebih efisien, atau lebih Pythonic sekarang?
2.  **Berkontribusi pada Proyek Open Source:**
    *   Ini adalah cara yang bagus untuk belajar dari kode orang lain, memahami alur kerja pengembangan nyata (Git, code review, testing), dan membangun portofolio Anda.
    *   Cari proyek di GitHub yang sesuai dengan minat dan tingkat keahlian Anda. Banyak proyek menyambut kontributor baru, bahkan untuk tugas-tugas kecil seperti memperbaiki dokumentasi atau bug sederhana.
3.  **Bangun Portofolio Anda:**
    *   Kumpulkan proyek-proyek terbaik Anda di platform seperti GitHub. Portofolio yang solid adalah aset berharga saat mencari pekerjaan atau menunjukkan keahlian Anda.
    *   Tulis README yang jelas untuk setiap proyek, menjelaskan apa yang dilakukannya, bagaimana menjalankannya, dan teknologi apa yang digunakan.
4.  **Perdalam Area Spesifik:**
    *   Jika Anda tertarik pada pengembangan web, pelajari Flask atau Django lebih dalam.
    *   Jika Anda menyukai data, fokus pada NumPy, Pandas, Matplotlib, Seaborn, dan mungkin Scikit-learn untuk machine learning.
    *   Jika otomatisasi adalah tujuan Anda, eksplorasi lebih lanjut pustaka seperti `requests`, `BeautifulSoup`, `Selenium`, atau `schedule`.
    *   Jika Anda ingin membuat game, selami `pygame`.
5.  **Jangan Pernah Berhenti Belajar:**
    *   Dunia teknologi terus berkembang. Python sendiri terus diperbarui dengan fitur-fitu baru.
    *   Ikuti blog, podcast, atau tokoh berpengaruh di komunitas Python.
    *   Baca buku atau ambil kursus lanjutan tentang topik yang menarik minat Anda.
    *   Teruslah bereksperimen dan mencoba hal-hal baru.

Yang terpenting adalah **jangan menyerah**. Semua programmer pernah menjadi pemula. Hadapi tantangan, rayakan keberhasilan kecil, dan nikmati proses belajar dan menciptakan dengan Python!

**Terima kasih telah menggunakan panduan ini. Semoga sukses dalam perjalanan Python Anda!**
