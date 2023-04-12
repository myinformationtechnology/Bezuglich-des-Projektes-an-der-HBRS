# Bezuglich-des-Projektes-an-der-HBRS
Kommunikation in verteilten Systemen

Installation unter Ubuntu
Damit das Modul PyAudio läuft wird die C-Bibliothek portaudio benötigt. Unter Ubuntu kann man dafür zunächst die benötigten Abhängigkeiten installieren und anschließend mit pip3 das Python Modul PyAudio

sudo apt update
sudo apt install portaudio19-dev python-pyaudio
pip3 install pyaudio


Record.py
Urpsrüngliches Skript.

Zeichnet 5 Sekunden auf und speichert anschließend die Datei


Recorder.py

Enthält Klasse Recorder als Wrapper um die Funktionen start_recording() und stop_recording().
Nimmt so lange auf, bis man stoppt.
Kann über GUI gesteuert werden: gui.py


Gui.py

Sehr einfache GUI.
Wird im CLI gestart mit 'gui.py <filename.wav>'
Benötigt:

python3-tk (sudo apt install python3-tk, Windows entsprechend Tkinter installieren)
pip3 install pysimplegui (Windows entsprechend PySimpleGUI installieren)




Client Server Anwendung
Es können mit "udpclient.py" für den UDP Client und "udpsrv.py" für den Server Strings mittels UDP übertragen werden.
Beim Ausführen müssen folgene Parameter übergeben werden: Datei.py, Serveradresse (IP Adresse), Port, Nachricht
Es können mit "tcpclient.py" für den TCP Client und "tcpsrv.py" für den Server Strings mittels TCP übertragen werden.
Beim Ausführen müssen folgene Parameter übergeben werden: Datei.py, Serveradresse (IP Adresse), Port, Nachricht
