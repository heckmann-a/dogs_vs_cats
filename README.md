# dogs_vs_cats
## Mein Projekt steht auf GitHub zur Verfügung und lässt sich direkt über nbviewer ansehen: 
[Zum Notebook](https://nbviewer.org/github/heckmann-a/dogs_vs_cats/blob/main/Dogs_vs_Cats.ipynb)

&nbsp;
# Einführung:
Hund!...oder Katze?...oder doch Hund?\
Für uns Menschen ist es relativ einfach zu erkennen, ob es sich um einen Hund oder eine Katze handelt.\
Unser Gehirn hat Millionen Jahre Evolution hinter sich – wir sind darauf trainiert, Tiere zu erkennen.\
Bei Computern ist das anders. Sie sehen nur eine Zahlenmatrix mit zu vielen Pixeln und entsprechenden RGB-Werten (Rot, Grün, Blau).

Folglich:\
-> Wir sehen einen flauschigen Hund.\
-> Die Maschine eine gefühlt endlose Zahlenschlange.

Es ist aber wichtig, dass Computer heutzutage Bilder erkennen z.B.:

* In der Medizin um frühzeitig Krankheiten zu erkennen und Diagnosen zu erstellen.
* In der Forschung um mikroskopischen Aufnahmen zu analysieren.
* In der Sicherheit um verdächtige Personen oder Verhalten zu erkennen.
* In der Industrie bei der Fertigung um Fehler in der Produktion zu erkennen.

# Aufgabenstellung:
Damit die Maschinen solche Unterschiede erkennen können, soll hier ein Machine-Learning-Modell erstellt und trainiert werden.\
Hierzu wurde ein Datensatz aus Kaggle genutzt, welches ca. 12.500 Katzen- und 12.500 Hundebilder enthält.

# Datenquellen:
[(Datensätze: Kaggle.com)](https://www.kaggle.com/datasets/karakaggle/kaggle-cat-vs-dog-dataset?select=kagglecatsanddogs_3367a)\
*Der verwendete Datensatz stammt aus Kaggle und unterliegt der Lizenz 'Unknown'.\
Dieses Projekt dient ausschließlich zu Lern- und Demonstrationszwecken und wird nicht für kommerzielle Nutzung eingesetzt.*

# Technologien & Libraries:
* Python in Jupyter Notebook
* libs: matplotlib, pandas, numpy, tensorflow, keras, layers, Image aus PIL

# Beschreibung des Vorgehens:
* Einlesen und Vorverarbeitung der Daten
* Modellierung
* Ablation Study
* Ergebnisse

# Ergebnisse:
Durch den Aufbau eines CNN (Convolutional Neural Networks) mit leichter Datenaugmentierungen und einer Epoche von 20\
konnte eine Performance erreicht werden von:
* Train = 89,38 % [accuracy: 0.8938 - train_loss: 0.2490]
* Validation = 89,86 % [accuracy: 0.8986 - val_loss: 0.2587]
* Test = 87,33 % [accuracy: 0.8733 - test_loss: 0.3081]

|          | Train   |Validation| Test     |
|----------:|:----------:|:----------:|:----------:|
| %        | 89,38    | 89,86    | 87,33    |
| Accuracy | 0.8938   | 0.8986   | 0.8733   |
| Loss     | 0.2490   | 0.2587   | 0.3081   |
