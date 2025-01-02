## Sınıf ve İlişkiler
### 1.Sınıflar
     1. **Building**:Bina genel özelliklerini içerir.
     2. **Floor**:Her bir katın özelliklerini temsil eder.
     3. **Elevator**:Asansörlerin özelliklerini ve işlevlerini temsil eder.
     4. **ElevatorControlPanel**:Asansörün iç kontrol panelini modellemek için kullanılır.
     5. **CallButton**:Katlarda yer alan çağrı düğmelerini temsil eder.
     6. **Passenger**:Yolcu nesnelerini temsil eder.
     7. **Clock**:Simülasyonun zamanını takip eder.
     8. **RandomNumberGenerator**:Rastgele yolcu ve kat bilgilerini üretir.
     
## Sınıf Diyagramı
![Elevator Diyagram](elevatorDiyagram.png)

## Açıklamalar
  ### 1.Building:
       - Binanın asansörleri(elevators) ve katları(floors) içerir.
       - Trafik yönetimi işlevlerini içerir
  ### 2.Floor:
       - Kat numarası(floorNumber) ve çağrı düğmelerini(callButtons) içerir.
       - Varış zili ve ışığı kontrol edilir.
  ### 3.Elevator:
       - Kapasite, mevcut kat, hareket yönü gibi temel özelliklere sahiptir.
       - `move()`,`stop()`,`openDoor()`,`closeDoor()` gibi temel işlevlerine sahiptir.
  ### 4.ElevatorControlPanel:
       - Asansör içindeki kontrol panelidir ve hedef düğmelerini içerir.
  ### 5.CallButton:
       - Katlarda bulunan çağrı düğmeleridir ve baıldığında ilgili asansörü çağırır.
  ### 6.Passenger:
       - Yolcu nesnesidir, her bir yolcunun başlangıç ve hedef kat bilgisi mevcuttur.
  ### 7.Clock:
       - Simülasyonun zamanını takiğ eder ve olayları zaman damgası ile kaydeder.
  ### 8.RandomNumberGenerator:
       - Rastgele sayılar üreterek yolcu oluşturur ve katları belirler.
