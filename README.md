# JuFo-KI
## Einleitung
Mein Projekt untersucht die Frage, wie intelligent künstliche Intelligenz ist.Zur Bestimmung der Intelligenz beim Menschen gibt es verschiedene Tests. Die Intelligenz verschiedener Modelle solltedeshalbebenfalls in verschiedenenTestsuntersucht werden. Ich habeverschiedene Modelle trainiertund anschließenduntersucht, wie präzise die trainierten Modelle verschiedene Aufgaben lösen konnten.Trotz des umfangreichen Trainings verschiedener Modelle konnten in meinen Experimenten die Ergebnisse von Menschen nicht erreicht werden. Eine KI braucht sehr viele Beispiele, um einen Sachverhalt zu erlernen. Ein Mensch schafft das meistens schon mit nur einem Beispiel. Ausnahme war die Erkennung von Mustern des Raven-Datensatzes, der die progressiven Matrizen beinhaltet.Während meines Projektes habe ich herausgefunden, dass alle trainierten Modelle die Daten, mit denen sie trainiert wurden, widerspiegeln. Das bedeutet, eine KI ist nur so intelligent, wie die Daten, mit denen sie trainiert wird.
## Code
Die .ipynb Dateien sind Jupyter-Notebooks. Sie Können in einer Jupyter-Umgebung ausgeführt werden.
#### ChatBot_v1.ipynb
ChatBot_v1.ipynb beinhaltet den Code für einen einfachen Chatbot, der auf der Autoencoder -Architektur basiert. Das Modell dient nur zu Demonstrieren der Funktionsweise eines solchen Modells. Für das Trainierten wird der „[chatterbot/english](https://www.kaggle.com/kausr25/chatterbotenglish)“  Datensatz von Kaggle benötigt.
#### dataset_to_tfrecord.ipynb
Dieses Skript bietet eine effiziente Möglichkeit generierte Einträge vom [RAVEN-Datensatz]( https://github.com/WellyZhang/RAVEN) in .tfrecord Dateien zu konvertieren. .tfrecord Dateien sind speziell für TensorFlow und ermöglichen effizienteres und schnelleres Laden von daten saus GCS- bucket. Wie viele Einträge in eine .tfrecord Datei passen hängt vom Arbeitsspeicher ab und der unkomprimierten Größe der Einträge. 
#### Visualise-RAVEN.ipynb
Visualise-RAVEN.ipynb bietet eine einfache Möglichkeit Einträge zu visualisieren. Es werden zuerst 8 Bilder gegeben, welche Gemeinsamkeiten haben. Als zweites werden die 8 Auswahlmöglichkeiten, die in das Muster passen gezeigt. Als letztes wird die Lösung ausgegeben. 
### SciKit
In SciKit befindet sich die verwendete virtuelle Python- Umgebung, welche für das Trainieren von Modellen des Maschinellen Lernen. Sie kann mithilfe des „activate“ Skripts aktiviert und benutzt werden. Visual Studio ist auch in der Lage virtuelle Umgebungen zu verwenden. Der Vorteil besteht darin, dass alle Benötigten Erweiterungen bereits in der passenden Version installiert sind
### Python-KI
Hier befinden sich der gesamte Python-Code, der Maschinelles Lernen verwendet und lokal auf dem Computer ausgeführt werden kann.
### Csharp_machieneLearning
In diesem Ordner ist die Projektmappe mit der C#-Version des Maschinellen Lernens. ML.NET ist bereits in der Version 1.14 installiert.
## Ergebnisse 
### Modelle_SK-learn
Hier sind die trainierten SciKit-Modelle gespeichert. Sie können problemlos mit der library „Joblib“ geladen und verwendet werden.
### Results
Hier befinden sich Dateien, welche die Genauigkeiten und auch zum Teil mehr Information über die einzelnen Modelle und deren Durchläufe beinhalten. Die Benennung der Dateien ist auf das verwendete Framework zurückzuführen. Die Dateien „Result“ und „ModelResult…“ stammen von Scikit-learn. 
### TensorBoard
Im Ordner TensorBoard sind Informationen zu den entsprechenden Modellen gespeichert. Da die Informationen von TensorBoard aufgezeichnet wurden und TensorBoard nur eingeschränkt auf der TPU ausgeführt werden kann, wurden die Modelle auf meinem Computer ausgeführt. Wegen dem mangelnden VRam konnte kein Training durchgeführt werden, aber Informationen wie: Modellgraph und genauer Aufbau des Modells konnten analysiert und aufgezeichnet werden.   
