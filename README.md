                                                      Trafiğe Yeni Açılan Yollar Nedeniyle Mesafe Cetveli (14.02.2024)
Proje Özeti:
  Bu projede, Türkiye’deki şehirler arası mesafeleri içeren bir uygulama geliştirdim. C# dilinde yazdığım bu uygulamada, şehirler arası mesafe cetvelini kullanarak çeşitli işlemler gerçekleştirdim.
  Jagged array yapısıyla matris oluşturarak ve algoritmalar kullanarak farklı senaryoları ele aldım.

Proje İçeriği:
1. Uzaklık Matrisi Oluşturma
  Şehirler arası mesafe cetvelini kullanarak jagged array yapısında bir uzaklık matrisi oluşturuldu. İller arası mesafe cetvelini dosyadan okuyarak veya kopyalayarak veriler diziye aktarıldı.
  Her ilin numarasına göre bir dizide tutulması sağlandı (indeksler plaka numarasına karşılık gelecek şekilde).
  10 adet şehir çifti, rastgele seçilerek jagged array üzerinden alınan plaka numaraları ve aralarındaki uzaklık bilgisiyle birlikte ekrana ve rapor dosyasına yazdırıldı.

2. Türkiye'deki Şehirlerin Komşuluk Listesi
  Türkiye’deki şehirlerin birbirine komşu olanlarının listesi internetten veya başka bir kaynaktan alınarak mesafe matrisi üzerinde bu bağlantılar gösterildi.
  Mesafe cetvelinde şehirler arası bağlantı bulunmuyorsa o iki şehir için bağlantı değeri sonsuz (∞) kabul edildi.

3. En Kısa ve En Uzun Farklı Mesafeleri Hesaplama
  Komşu olmayan tüm şehir çiftleri arasındaki en kısa mesafeyi ve en uzun mesafeyi bulmak için Dijkstra algoritması ile şehir merkezlerinden geçerek mesafe hesaplandı.
  Her bir şehir çifti için, şehirler arası uzaklık değerinin şehirler arası farkını hesaplayan bir metot oluşturuldu.
  En küçük ve en büyük farkı sağlayan şehir çiftleri tespit edilerek, bu şehir çiftleri ekrana ve rapor dosyasına yazdırıldı.

4. İzmir ve İlçeleri için Uzaklık Matrisi
  İzmir’e bağlı 30 ilçe için yeni bir uzaklık matrisi oluşturuldu (bu kez jagged array olmayan).
  İlçeler arası mesafe cetveli hazırlanarak, İzmir’e bağlı ilçeler arasındaki mesafeler eklendi.
  Kod içerisine manuel olarak veya dosyadan okuma yöntemi ile veri aktarımı sağlandı.
  Uzaklık matrisi ve ilgili metotlar kullanılarak rapor ekranına yazdırıldı.

5. İzmir ve İlçeleri için Tekrar
  İzmir ve ilçeleri için ilk maddede uygulanan işlemler tekrarlanarak, ilçeler için de rapor ve ekran çıktısı alındı.

Kullanılan Teknolojiler:
  C# (.NET)
  Konsol Uygulaması
  Jagged Array ve Normal Matris Yapısı
  Dijkstra Algoritması
