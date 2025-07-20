Power BI Müşteri Raporu
1. İçerik
•	Özet Sayfa: KPI’lar ve satış özetleri
•	Müşteri Perspektifi: Cinsiyet, bölge ve yaş grubu analizleri
2. Veri ve Model
•	Tablolar: Kullanıcılar, Adres, Ürünler, siparis, siparisdetay, Bölgeler
•	Önemli ilişkiler:
o	Kullanıcılar[ID] → siparis[UserID]
o	Adres[ID] → siparis[AddressID]
o	siparis[ID] → siparisdetay[OrderID]
o	Ürünler[ID] → siparisdetay[ItemID]
3. Önemli Ölçüler
•	Toplam Satış Adeti = SUM(siparisdetay[Amount])
•	Toplam Ciro = SUM(siparis[TotalPrice])
•	Tekil Müşteri Sayısı = DISTINCTCOUNT(siparis[UserID])
•	Kadın Müşteri Sayısı / Erkek Müşteri Sayısı
•	Yaş Grubuna Göre Satış, Bölgelere Göre Müşteri Sayısı, vb.
4. Kullanım
1.	powerbı_proje_musteri_raporu.pbix dosyasını Power BI Desktop’ta aç
2.	Refresh ile verileri güncelle
