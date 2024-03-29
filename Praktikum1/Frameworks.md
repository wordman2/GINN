
# Aufgabe 1a
Welche Methoden wurden in der Vorlesung vorgestellt?

- Foreward Propagation
- Backward Propagation

###### ##################################################################################
# Aufgabe 1b
Recherchiere geeignete Frameworks (auch andere außer Tensorflow und PyTorch)! Überlegen Sie sich Kriterien, anhand deren Sie die Frameworks evaluieren. Finden Sie heraus, wie die bisher in der Vorlesung vorgestellten Methoden (...) umgesetzt werden können in den Frameworks. Stellen Sie die gesamte Auswertung übersichtlich dar (natürlich inklusive Pros & Cons etc).

Wir untersuchen nur Python Libarys.

## ChatGPT ##
Folgenden Output hat mir ChatPT gegeben. Daran könnten wir uns orientieren:  

1. Keras: Keras ist eine High-Level-API, die auf TensorFlow, Theano und Microsoft Cognitive Toolkit aufbaut. Es bietet eine einfache und intuitive Syntax für das Erstellen und Trainieren von neuronalen Netzen.

2. MXNet: MXNet ist ein Framework für Deep Learning, das von Apache entwickelt wird. Es bietet eine skalierbare und effiziente Implementierung von neuronalen Netzen sowie Unterstützung für verschiedene Programmiersprachen, darunter Python.

3. Chainer: Chainer ist ein Deep-Learning-Framework, das eine flexible und intuitive API bietet. Es unterstützt dynamische Berechnungsgraphen und ermöglicht es den Benutzern, ihre Modelle auf eine natürliche Weise zu definieren und zu manipulieren.

4. Caffe: Caffe ist ein Framework für Deep Learning, das für seine Geschwindigkeit und Effizienz bekannt ist. Es wird häufig in der Bildverarbeitung und im Bereich der Computer Vision eingesetzt.

5. Theano: Theano ist ein Python-Framework, das speziell für die effiziente Berechnung mathematischer Ausdrücke entwickelt wurde, insbesondere für das Training von neuronalen Netzen. Obwohl es nicht mehr aktiv weiterentwickelt wird, wird es immer noch von einigen Forschern und Entwicklern genutzt.

6. CNTK (Microsoft Cognitive Toolkit): CNTK ist ein von Microsoft entwickeltes Deep-Learning-Framework, das für seine Skalierbarkeit und Effizienz bekannt ist. Es bietet eine breite Palette von Funktionen für das Training von neuronalen Netzen, einschließlich Deep-Learning-Modellen.

7. Neon: Neon ist ein Deep-Learning-Framework, das von Nervana (später von Intel übernommen) entwickelt wurde. Es ist auf die Effizienz bei der Berechnung von neuronalen Netzen ausgelegt und bietet eine Reihe von Optimierungen für die Verarbeitung großer Datensätze.

8. Lasagne: Lasagne ist ein weiteres Deep-Learning-Framework in Python, das auf Theano aufbaut. Es bietet eine einfach zu verwendende API für das Erstellen und Trainieren von neuronalen Netzen sowie eine Vielzahl von vorgefertigten Schichten und Funktionen.

9. PaddlePaddle: PaddlePaddle (auch bekannt als "Paddle") ist ein von Baidu entwickeltes Deep-Learning-Framework, das für seine Skalierbarkeit und Effizienz bekannt ist. Es bietet eine Vielzahl von Funktionen für das Training von neuronalen Netzen und wird häufig für große Datensätze und verteilte Berechnungen verwendet.

## Auswertung
### Framework1 
Quelle
- Stichwort 1
- Stichwort 2

### scikit-learn
https://scikit-learn.org/stable/modules/neural_networks_supervised.html
- Vorteil: viele bereits mit Scikit-learn Bibliothek vertraut, findet schnell Hilfe im Netz
- Nachteil: Nicht für sehr große Datenmengen geeignet, keine GPU Unterstützung
            im Vergleich zu anderen Frameworks wenig Flexibilität (noch spez. Punkte suchen)

- Implementierung: https://stackabuse.com/introduction-to-neural-networks-with-scikit-learn/


### Keras
Arbeitet auch, aber nicht nur mit Tenserflow und Pytorch als Backend.
https://keras.io/getting_started/intro_to_keras_for_engineers/
Jax als Backend:
- JAX baut auf Numpy auf -> Umstieg ist einfach
- Kombination von Funktionen möglich, da funktionales Programmiermodell
- ist schnell und kann mit GPU/TPU umgehen
- Quelle: https://www.newhorizons.com/resources/blog/jax-vs-pytorch-comparing-two-deep-learning-frameworks
- Durch die hohe Beliebheit gut dokumentiert und aktive Community

### Neon
https://github.com/NervanaSystems/neon/blob/master/README.md
- Vorteil: gut für große Netze
- Nachteil: Wird nicht mehr entwickelt, Tutorials gelöscht, keine aktive Community

### PaddlePaddle
Steht für: PArallel Distributed Deep LEarning
Quelle: https://learnopencv.com/paddlepaddle/
- Vorteil: sehr schnell, Parallelisierung, vortrainierte Modelle vorhanden
- Nachteil: wenig Anleitungen
