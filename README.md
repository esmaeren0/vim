#Nano
Nano, terminal tabanlı kolay bir metin editörüdür.
echo "--------------------------------------------"
echo "| Kısayol         | Açıklama               |"
echo "--------------------------------------------"
echo "| Ctrl + O        | Dosyayı kaydet         |"
echo "| Ctrl + X        | Çıkış                  |"
echo "| Ctrl + R        | Dosya ekle             |"
echo "| Ctrl + W        | Dosya içinde arama     |"
echo "| Ctrl + K        | Satırı kes             |"
echo "| Ctrl + U        | Satırı yapıştır        |"
echo "| Ctrl + G        | Yardım menüsünü aç     |"
echo "| Ctrl + C        | Satır ve sütun bilgisi |"
echo "--------------------------------------------"
# VIM
Vim using

 
KOMUTLAR
-------------------------------------------------------------------------------------------------------------------
1. Vim Nedir ve Nasıl Açılır: vim dosya_adı komutu ile Vim başlatılır. Veya vim ile dosya açılmadan boş  başlatılır.
--------------------------------------------------------------------------------------------------------------------
2. Modlar
- Normal Mode: varsayılan mod
- Insert Mode: i, a, o gibi komutlarla girilir. Yazı yazılır.
- Visual Mode: (v tuşu), V ile satır seçme
  - Command mod: (: tuşuyla girilir) , dosya kaydetme,çıkış
  ----------------------------------------------------------------------------------------------------------------
3. Insert Mode’a Geçiş

- i: İmlecin soluna yazar
- a: İmlecin sağına yazar
- I: Satır başına yazar
- A: Satır sonuna yazar
- o: Alt satıra boş satır açar
- O: Üst satıra boş satır açar

------------------------------------------------------------------------------  
4. Kaydetme & Çıkma

- (:w) Kaydet
- (:q)  Çık
- (:wq) veya (ZZ:) Kaydet ve çık
- (:q!) Kaydetmeden çık
-----------------------------------------------------------------------------------  
5. Temel Hareket Komutları

- h, j, k, l: Sol, aşağı, yukarı, sağ (opsiyonel)
- 0: Satır başına geçilir
- ^: Satırın ilk karakterine geiçilir
- $: Satır sonuna gidilir
- gg: Dosya başına gidilir
- G: Dosya sonuna gidilir
- nG: sayısı girilen satıra gidilir

 ------------------------------------------------------------------------------------- 
6. Silme İşlemleri (Delete)

- x: Bir karakter sil
- dd: Satır sil
- dw: Kelime sil
- d$: Satır sonuna kadar sil
------------------------------------------------------------------------------------
  
7. Geri Alma & Yeniden Yapma

- u: Geri al (undo)
- Ctrl + r: İleri al (redo)
 -------------------------------------------------------------------------------------- 
8. Kopyalama ve Yapıştırma (Yank & Paste)
  
- yy: Satırı kopyala
- p: İmleçten sonra yapıştır
- P: İmleçten önce yapıştır
------------------------------------------------------------------------------------
9. Visual Mode
- v: Karakter seçimi
- V: Satır seçimi
- Ctrl + v: Blok (column) seçimi
- Seçim sonrası y, d, p, : ile işlem yapılabilir

 --------------------------------------------------------------------------------------- 
10. Arama & Değiştirme

- /kelime: Aşağı doğru ara
- ?kelime: Yukarı doğru ara
- n: Sonraki sonucu bul
- :%s/eski/yenisi/g: Tüm dosyada değiştir
 --------------------------------------------------------------------------------------- 
11. Satırları Sıralama
- Görsel modla satırları seç, ardından :sort komutunu yaz
 ----------------------------------------------------------------------------------------- 
12. Buffer (Ara Bellek) Kavramı

- Buffer = Açık dosya
- :ls veya :buffers: Açık buffer'ları listele
- :b1, :b2 gibi komutlarla geçiş yapılır
 ------------------------------------------------------------------------------------------- 
13. Yeni Buffer Açmak
    
- :e dosya.txt: Yeni dosya açar (yeni buffer olur)
- :enew: Boş buffer açar
 ---------------------------------------------------------------------------------------------- 
14. Bufferlar Arası Geçiş
    
- :bnext veya :bn: Sonraki buffer
- :bprev veya :bp: Önceki buffer
- :bd: Buffer sil (kapama)
-----------------------------------------------------------------------------------------------  
15. Bufferları Birleştirmek	İki buffer’ın içeriğini tek dosyada görmek için:
    
- Bir dosyayı açtıktan sonra diğer dosyanın içeriğini eklemek için :read dosya.txt kullanılabilir
 ------------------------------------------------------------------------------------------------- 
16. Vim’de Terminal Komutları Çalıştırma
- :!komut: Dış terminal komutu çalıştırır
Örnek: :!ls, :!date
----------------------------------------------------------------------------------------------
17. Bölünmüş Pencereler (Splits)
- :split dosya.txt veya :sp: Yatay böl
- :vsplit dosya.txt veya :vsp: Dikey böl
- Ctrl + w, w: Pencereler arasında geçiş
- Ctrl + w, h/j/k/l: Yönlü geçiş
- :q: Alt pencereyi kapat
 -------------------------------------------------------------------------------------------- 
18. Tek Dosyayı Bölme	Aynı dosyayı bölünmüş pencerelerde göstermek için:
- :split veya :vsplit (dosya adı olmadan)
---------------------------------------------------------------------------------------------  
19. Yardım Alma
- :help komut: Komut hakkında yardım al
Örnek: :help :wq, :help visual-mode
-----------------------------------------------------------------------------------------------
21. Vim'den Çıkış (Zor Durumlar)
     - Esc tuşuna birkaç kez bas, sonra :q! veya :qa! ile tümünden çık
