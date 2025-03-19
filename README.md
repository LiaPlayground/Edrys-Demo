<!--
language: de
narrator: Deutsch Female
-->


# Experimente mit edrys-Lite

Ein Experiment in edrys-Lite ist eine interaktive, digitale Lernumgebung, in der die Schülerinnen und Schüler in Echtzeit zusammenarbeiten und auf Hardware zugreifen können.

## Idee

    --{{0}}--
Stellen sie sich vor, sie hätten ein Arbeitsblatt und ein Experiment, das sie mit ihren Schülern durchführen möchten. Sie könnten das Arbeitsblatt kopieren und an alle Schüler verteilen, die dann einzeln oder in kleinen Gruppen das Experiment durchführen.

      {{1}}
- __Arbeitsblatt als einfache Datei:__

      --{{1}}--
  In edrys‑lite ist ein „Experiment“ nichts anderes als eine einfache Datei, die alle wichtigen Einstellungen enthält – ähnlich wie ein vorbereitetes Unterrichtsblatt. Diese Datei einfach erstellt, verändert. Geteilt wird das Arbeitsblatt über einen Link.

  https://edrys-labs.github.io/?/deploy/https://raw.githubusercontent.com/edrys-labs/lab-web-serial/main/laboratory/micropython.yaml

  ```` yaml  MicroPython-Labor.yaml
  id: UFjCXcT4dfSsWcRm
  createdBy: 35banpdWTU7qL
  dateCreated: 1713791372082
  name: Lab - WebSerial
  meta:
    logo: >-
      https://raw.githubusercontent.com/edrys-labs/lab-web-serial/main/media/logo.jpg
    description: >-
      Discover the exciting world of coding with our MicroPython course...

    selfAssign: true
    defaultNumberOfRooms: 0
  members:
    teacher: []
    student: []
  modules:

  - url: >-
      https://raw.githubusercontent.com/edrys-labs/module-markdown-it/2.0.0/index.html
    config: >-
      # Course Summary: Introduction to Python, Arduino, and MicroPython
      ...
    studentConfig: ''
    teacherConfig: >-
      ## Teacher instructions

      ...
    stationConfig: ''
    showInCustom: Lobby
    width: full
    height: tall

  - url: https://edrys-labs.github.io/module-serial/
    config:
      baud: 115200
    studentConfig: ''
    teacherConfig: ''
    stationConfig: ''
    showInCustom: Station
    width: full
    height: medium

  - url: https://edrys-labs.github.io/module-station-stream/index.html
    config: ''
    studentConfig: ''
    teacherConfig: ''
    stationConfig:
      video: true
      audio: false
    showInCustom: Station
    width: half
    height: medium
  
  ...
  ````

      {{2}}
- __Peer to Peer Verbindung mittles WebRTC statt klassischer Server:__

      --{{2}}--
  Anstatt dass alle Daten über einen zentralen Server laufen, kommunizieren die Browser der Teilnehmer direkt miteinander. Das ist, als ob alle im Raum direkt miteinander sprechen würden – das spart Zeit, erzeugt keine Kosten und ist Datenschutskonform.

  ![Screenshot eines Labors mit 4 Nutzern](media/labor.png)

      {{3}}
- __Einfache Integration von Hardware:__

      --{{3}}--
  Hardware kann entweder direkt an den Laptop des Lehrers über eine Browser-Schnittstelle, wie zum Beispiel WebUSB, WebSerial angeschlossen werden oder über ein zusätzliches Programm, dass als "Server" den direkten und lokalen Zugriff auf das Experiment ermöglicht.

  ![Zugriff auf Arduino](media/station.png)

     {{4}}
- __Automatische Synchronisation der Arbeit mittels CRDTs:__

      --{{4}}--
  Wenn mehrere Personen gleichzeitig an einem Arbeitsblatt (Labor/Experiment) arbeiten, sorgt ein intelligentes System dafür, dass alle immer den aktuellen Stand sehen. Es ist, als würde eine Tafel im Klassenzimmer automatisch alle Änderungen anzeigen, egal wer gerade etwas ergänzt oder verändert.

  ![Screenshot vom gemeinsamen Zugriff auf ein Experiment](media/micropython.png)

     {{5}}
- __Ideal für kleine Gruppen:__

      --{{5}}--
  Da alles direkt im Browser läuft, brauchen die Nutzer weder komplizierte Anmeldungen noch teure Server – das macht edrys‑lite besonders attraktiv für kleine Gruppen oder Unterrichtssettings, wo Flexibilität und einfache Handhabung im Vordergrund stehen.

  !?[YouTube: Edrys MicroPython Lab](https://www.youtube.com/watch?v=6ZjGHorc2ds)

## Demo: SUUpoRT Urkraine

![](/media/ukarine.jpeg)

## Demo: Analog-Digital-Wandler

Ein weiterer Vorteil von edrys-Lite ist die Möglichkeit, mehrere Experimente parallel durchzuführen. Das bedeutet, dass die Schülerinnen und Schüler nicht nur an einem Experiment arbeiten können, sondern auch an mehreren gleichzeitig.

Die Studierenden setzen eine Anwendung um, die zwei existierende Klassen für die Verwendung von peripheren Bauteilen - Ultraschallsensor und LCD-Display - um. Im Ergebnis steht eine Applikation die kontinuierlich die Distanz zu einem Hindernis vermisst. Die Daten werden zudem über die Serielle Schnittstelle ausgegeben und analysiert.

https://edrys-labs.github.io/?/classroom/1Sjgqpq8CaIKAsJh

## Andere Anwendungsbeispiele

![](/media/ChemischeAnlage.jpg)


## Wie geht es weiter?

> __Interaktive Projektdokumentation__ https://liascript.github.io/course/?https://raw.githubusercontent.com/edrys-labs/documentation/refs/heads/main/README.md

!?[YouTube: Presentation](https://www.youtube.com/watch?v=Uv79Y8EhBVw)

