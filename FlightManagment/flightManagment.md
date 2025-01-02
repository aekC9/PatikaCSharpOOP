## 1.Ana Aktörler:
 - Havayolu Şirketi (Airline)
 - Uçak (Aircraft)
 - Pilot
 - Uçuş
 - Havaalanı (Airport)
## 2.Sınıflar ve ilişkiler:
### 2.1.Airline (Havayolu Şirketi)
 - ### Nitlekikler:
    - `string AirlineID` (Havayolu kimliği)
    - `string Name` (Havyolua adı)
    - `List<Aircraft> Fleet` (Filo - Sahip olduğu uçaklar)
    - `List<Pilot> Pilots` (Çalıştırdığı pilotlar)
### 2.2.Aircraft (Uçak)
 - ### Nitlekikler:
    - `string AircraftID` (Uçak kimliği)
    - `string Type` (Uçak tipi)
    - `bool IsOperational` (Uçak çalışır durumda mı?)
    - `int RequiredPilots` (Gereken pilot sayısı)
 - ### İlişki:
    - Bir uçak bir havayolu şirketine aittir.
### 2.3.Pilot
 - ### Nitlekikler:
    - `string PilotID` (Pilot kimliği)
    - `string Name` (Pilot adı)
    - `int ExperienceLevel` (Deneyim seviyesi)
 - ### İlişki:
    - Bir pilot, bir havayolu şirketine bağlıdır.
### 2.4.Flight (Uçuş)
 - ### Nitlekikler:
    - `string FlightID` (Uçuş kimliği)
    - `Airport DepartureAirport` (Kalkış havaalanı)
    - `Airport ArrivalAirport` (Varış havaalanı)
    - `DateTime DepartureTime` (Kalkış saati)
    - `DateTime ArrivalTime` (Varış saati)
 - ### İlişkiler:
    - Bir uçuş, bir uçak tarafından gerçekleştirilir.
    - Her uçuşta bir kaptan ve bir yardımcı pilot bulunur.
### 2.5.Airport (Havaalanı)
 - ### Nitlekikler:
    - `string AirportID` (Havaalanı kimliği)
    - `string Name` (Havaalanı adı)
 -  ### İlişki:
    - Havaalanı uçuşlarını kalkış ve iniş yerledridir.

![Sınıf Diyragramı:](sinifdiyagrami.png) 
