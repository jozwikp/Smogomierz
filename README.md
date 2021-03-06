# Smogomierz

![Smogomierz1](https://raw.githubusercontent.com/hackerspace-silesia/Smogomierz/master/instrukcje/photos/Smogomierz1.jpg)

Smogomierz to niekomercyjny projekt łatwego w budowie i taniego miernika zanieczyszczeń powietrza. Projekt jest w pełni otwarty i łatwy w modyfikowaniu. 

Smogomierz nie wysyła Twoich danych do żadnego serwisu, jeśli nie wyrazisz na to zgody. Dane pomiarowe z Twojego miernika należą do Ciebie i to od Ciebie zależy co z nimi zrobisz i komu je udostępnisz. Jeśli tylko Ty chcesz mieć dostęp do swoich danych, to masz do tego prawo. Jeśli jednak chcesz się nimi podzielić, to w karcie Konfiguracji panelu Smogomierza masz możliwość wyboru kilku serwisów, do których możesz wysłać dane. Wśród nich znajdziesz między innymi serwis [AirMonitor](http://mapa.airmonitor.pl), [ThingSpeak](https://thingspeak.com), czy bazę danych [InfluxDB](https://www.influxdata.com/time-series-platform/influxdb/). Smogomierz posiada również [wtyczkę Homebridge](https://github.com/bfaliszek/homebridge-smogomierz).

Smogomierz po pierwszym uruchomieniu tworzy własną sieć WiFi o nazwie "Smogomierz-deviceName"(np. "Smogomierz-328017"). Po podłączeniu się z nią, będziesz miał możliwość skonfigurowania połączenia WiFi z własną siecią domową. Z listy dostępnych sieci wybierz swoją własną i podaj do niej hasło. Smogomierz zapisze dane w swojej pamięci wewnętrznej i ponownie się uruchomienie. Dalszą konfigurację wykonasz już przez przeglądarkę internetową wchodząc pod adres Smogomierz-deviceName.local lub IP_Smogomierza(do sprawdzenia na routerze). 

Wkrótce planujemy udostępnić aplikację na Windowsa/macOS/Linuksa, która umożliwi w łatwy sposób wgranie oprogramowania oraz znalezienie adresu IP Twojego miernika!

## Instrukcje

1. [Instrukcja zlutowania wymaganych elementów](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/soldering.md)

2. [Instrukcja przygotowania obudowy oraz podłączenia elektroniki](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/hardware.md)

3. [Instrukcja instalacji/aktualizacji oprogramowania z pliku .bin](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/software-bin.md)

4. [Konfiguracja i ustawienia obsługi zewnętrznych serwisów(AirMonitor, InfluxDB itd.)](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/software-additionals.md)

## Parts / Potrzebne części

Do zbudowania własnego Smogomierza wymagana jest lutownica(wraz z cyną) oraz pistolet do kleju na gorąco, wiertarka, nóż do tapet i śrubokręt do skręcenia obudowy oraz części z poniższej listy.

[Lista potrzebnych części](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/components.md)

Gotowe zestawy części potrzebnych do zbudowania własnego Smogomierza, dostępne są również w sklepie Botland: [Zestaw DIY do budowy miernika smogu](https://botland.com.pl/pl/czujniki-czystosci-powietrza/13434-zestaw-diy-do-budowy-miernika-smogu-czujnik-czystosci-powietrza-pm25-i-pm10.html)

## Zaawansowane

[Instrukcja instalacji oprogramowania wymaganego do kompilacji oprogramowania z repozytorium](https://github.com/hackerspace-silesia/Smogomierz/blob/master/instrukcje/software.md)

### Tested on:

ArdinoIDE 1.8.5 – https://www.arduino.cc/en/main/software

### TODO

- [ ] Nowy design
- [ ] Kropki a nie przecinki przy zmianie współrzędnych w /config
- [ ] Automatyczne aktualizacje oprogramowania mierników
- [ ] Przygotowanie aplikacji Smogomierz-firmware-flasher bazującej na [airrohr-firmware-flasher](https://github.com/hackerspace-silesia/airrohr-firmware-flasher)


