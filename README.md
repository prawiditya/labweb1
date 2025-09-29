**Nama : PRAWIDITYA SAHRUL AKBAR**
**NIM : 312410146**
**Kelas : TI.24.A1**

**Hasil Output**

<img width="1920" height="1080" alt="Screenshot 2025-09-29 105128" src="https://github.com/user-attachments/assets/8ec78175-8d10-4cac-a125-343351bd6225" />


# Pertemuan 3 - Pemrograman Web

Proyek ini berisi latihan dasar **HTML** dan **CSS** pada mata kuliah **Pemrograman Web** di **Universitas Pelita Bangsa**.  
Tujuan utamanya adalah memahami penggunaan **CSS Internal**, **CSS Inline**, dan simulasi **CSS Eksternal** dalam satu halaman web.

---

## Struktur File
- `pertemuan 3.html` → File utama berisi contoh penggunaan HTML & CSS dasar.

---

## Materi yang Dipelajari
1. **CSS Internal**  
   Menggunakan tag `<style>` di dalam file HTML.
   
2. **Inline CSS**  
   Menambahkan atribut `style` langsung pada elemen HTML, contoh:
   ```html
   <p style="text-align: center; color: #ccd8e4;">...</p>
3. **CSS Eksternal (Simulasi)**
Disimulasikan menggunakan block <style> kedua, meskipun seharusnya dipisah dalam file .css.

4. **Selector CSS**

ID Selector → #intro

Class Selector → .button, .btn-primary

Tag Selector → h1, nav, p

**Penjelasan Code**
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
    
    <!-- CSS Internal -->
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        
        header {
            min-height: 80px;
            border-bottom: 1px solid #77CCEF;
            background-color: white;
        }
        
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
            margin: 0;
        }
        
        h1 i {
            color: #6d6a6b;
        }
        
        #intro {
            background: #418fb1;
            border: 1px solid #099249;
            min-height: 100px;
            padding: 10px;
            margin: 20px;
            border-radius: 5px;
        }
        
        #intro h1 {
            text-align: left;
            border: 0;
            color: #fff;
            padding: 10px 0;
        }
        
        #intro p {
            color: white;
            line-height: 1.5;
        }
        
        .button {
            padding: 15px 20px;
            background: #bebcbd;
            color: #fff;
            display: inline-block;
            margin: 10px;
            text-decoration: none;
            border-radius: 4px;
        }
        
        .btn-primary {
            background: #E42A42;
        }
        
        .btn-primary:hover {
            background: #c21830;
        }
    </style>
    
    <!-- CSS Eksternal (disimulasikan dalam style tag) -->
    <style>
        /* Simulasi CSS Eksternal */
        nav {
            background: #20A759;
            color: #fff;
            padding: 10px;
        }
        
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
            display: inline-block;
        }
        
        nav .active,
        nav a:hover {
            background: #08E8BA;
        }
    </style>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    
    <!-- CSS ID Selector -->
    <div id="intro">
        <h1>Hello World</h1>
        <!-- Inline CSS pada paragraf -->
        <p style="text-align: center; color: #ccd8e4;">
            Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. 
            Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.
        </p>
        <!-- CSS Class Selector -->
        <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
    </div>
</body>
</html>
```
