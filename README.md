# 🎨 Real-Time JavaScript Syntax Highlighter with GUI

## ✨ Proje Tanımı

Bu proje, JavaScript benzeri bir sözdizimine sahip kodları *gerçek zamanlı olarak analiz edip renklendiren (syntax highlighting)* ve *hataları tespit eden* etkileşimli bir web uygulamasıdır. Proje; *lexical analiz, **parser (sözdizimi çözümleyici), **hata kontrol mekanizması* ve *kullanıcı dostu GUI* bileşenlerini tamamen *kütüphane kullanmadan* kendi içerisinde barındırır.

[Projeyi canlı  denemek için tıklayabilirsiniz](https://asmbrk.github.io/Js_Syntax_Highlighter/)


---

## 🧩 Özellikler

- ✔ *Gerçek zamanlı sözdizimi vurgulama*
- ✔ *Top-Down recursive parser*
- ✔ *Regex tabanlı token tanıma*
- ✔ *Kapanmamış parantez, string, blok gibi hataları tespit eder*
- ✔ *Yanlış yazılmış anahtar kelimeleri algılar*
- ✔ **Eksik ;, else {}, } gibi yapıları uyarır**
- ✔ *Modern ve sade GUI tasarımı*
- ✔ *En az 5 farklı token tipi için renklendirme*

---

## 🔬 Teknik Bilgiler

### 🧠 Lexical Analysis (Tokenizer)
- *Yöntem:* Regex tabanlı token tanımları
- *Token Türleri:*
  - keyword → if, else, return, function, var, let, const, vb.
  - number → Tam ve ondalıklı sayılar
  - string → Tek, çift ve backtick tırnaklı metinler
  - identifier → Değişken ve fonksiyon isimleri
  - operator → +, -, *, /, =, ==, vb.
  - punctuation → (), {}, ;, , vb.
  - comment → Tek satırlık yorumlar //
  - boolean, null → true, false, null, undefined

     ![Oyun Ekranı](images/ss1.jpg)

### 📚 Syntax Analysis (Parser)
- *Yaklaşım:* Recursive descent parser (Top-down)
- *Desteklenen Yapılar:*
  - Değişken tanımlama (let, var, const)
  - Fonksiyon tanımı ve çağrısı
  - if, else, while, for blokları
  - return, break, continue deyimleri
- *Hatalı ifadeler*: detaylı biçimde işlenir ve kullanıcıya açıklanır

    ![Oyun Ekranı](images/ss2.jpg)

### 💡 Hata Denetimi
- Parantez dengesi ( (), {} )
- Kapanmamış string tespiti
- Yanlış yazılmış anahtar kelimeler (örn. retrun)
- Tanımsız değişken kullanımı
- Eksik noktalı virgül ;
- if, for, while gibi blok ifadelerinde eksik {} kontrolü

  ![Oyun Ekranı](images/ss3.jpg)
      

### 🖼 GUI Özellikleri
- HTML + CSS ile sade, modern bir düzen
- contenteditable alanı sayesinde kod yazımı
- Gerçek zamanlı renkli vurgulama
- Hatalar kullanıcıya altta kutu içerisinde gösterilir



[Proje raporuna ulaşmak için tıklayabilirsiniz](https://github.com/AsmBrk/Js_Syntax_Highlighter/blob/main/RAPOR.pdf)

[Proje için yazdığım makaleyi okumak için tıklayabilirsiniz](https://medium.com/@03asmbrk1907/javascript-syntax-highlighter-087df1f112b4)

[Projenin demo videosunu izlemek için tıklayabilirsiniz](https://www.youtube.com/watch?v=GGvk0aUdXzc)
