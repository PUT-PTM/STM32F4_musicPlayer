STM32F4_musicPlayer
===================
#==PL==#

#==:: O Projekcie ::==#

Projekt stworzony przy współpracy Jędrzeja Kruczka i Jakuba Nowakowskiego.
Projekt ten ma za zadanie przekonwertowanie pliku wave na płytce STM32F407 Discovery na tablicę wartości ostwarzanej przez codek i wzmacjniany przez wzmaczniacz z płytki. Plik wave zapisany na karcie SD podłączonej do plytki, z którą komunikuje się przez SPI. Nie mogliśmy skorzystać z SDIO ze względu na konflikt pinów z codekiem. Do pytki podłączony jest czujnik odlegości IR, który działa w zakresie 30 - 150 cm. Czujnik steruje głośnością odtwarzanej muzyki.

#===::Środowisko programistyczne i konfiguracja kompilatora::===#

Projekt ten został stworzony i zbudowany przy użyciu CooCox IDE- stwrzonym z myślą o procesorach ARM oraz przez kompilator GNU GCC.
Zainstaluj kompilator i środowisko programistyczne, wskaż ścierzkę do kompilatora GCC w programie CooCox IDE i rozpocznij pracę ze swoim mikrokontrolerem.

#===::Sterowniki i  oprogramowanie dla STM32F4xx::===#

Oprogramowanie na płytkę STM32F4xx Discovery  jest przesyłane przy użyciu przewodu USB, aby to zrobić należy w środowisku CoIDE wybrać opcję Program Download. Sterowniki do mikrokontlorera oraz przydatne narzędzia możesz znaleźć na stronie producenta.

#===::Building and Running the Code::===#

Budowanie: W środowisku CoIDE wybierz buduj.
Prześlij program na mikrokonroler: Klinkij na przycisk "Program Download" w środowisku CooCox IDE.
Testowanie: Klinkij na przycisk "Debug" w  CooCox IDE.

#===::Główne założenie::===#

Odtwarzanie plików wave i sterowanie głośnością odtwarzanej muzyki za pomocą czytnika odległości IR.

#===::Operacje::===#
1. Odczyt pliku wave z karty SD.
2. Dekodowanie pliku wave do tablicy intów.
3. Odtwarzenie dzwięku przez wyjście mini jack na płytce.
5. Odczytywanie odległości od urządzenia.
6. Sterowanie głośnością ze względu na odległość od urządzenia.




#===::Autorzy::===#

-Jędrzej Kruczek  
-Jakub Nowakowski

