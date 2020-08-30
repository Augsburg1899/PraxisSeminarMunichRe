#---------------------- Data Decision Science ----------------------#
 

#------- Allgemein -------#


Institut:               Unviversität Augsburg, Lehrstuhl Okhrin
Kooperationspartner:    Münchener Rück
Titel:                  Data Analysis of Financial Data and Trading Strategies
Autoren:                Böhm, Lukas; Mayer, Matthias
Bearbeitungszeitraum:   März - Mai 2020 


Im Folgenden wird der Inhalt der jeweiligen Dateien und Ordnern erläutert. 



#-------- Ordner ---------#


 # Data    
Ordner, der die jeweiligen Rohdaten der Märkte enthält. Die Dateien wurden im Rahmen des Skripts "exploratory_data_analysis.py" zusammengeführt.
  
 # Other_Data
Ordner, der zusätzliche Marktdaten enthält. Hierbei fand insbesondere die Datei "Risk_Premium.csv" Verwendung, da die hier aufgeführten Risikoprämien 
für die Berechnung der CAPM-Aplphas benötigt wurden.
  
 # Export
Ordner, in dem die Ausgabedateien der jeweiligen Signal-Skripte abgespeichert wurden. Diese listet im Idealfall je Umsetzung und Markt zwei Dateien: 
Einmal wurden die Ergebnisse ohne Berücksichtigung des Data Snooping Bias abgespeichert. Zum Anderen wurden die Resultate der dazugehörigen Bootstraps ausgelesen.

 # Export_Constant_Mix
Ordner, in dem die Ausgabedateien der jeweiligen Constant-Mix-Skripte abgespeichert wurden. 

 # Results
Ordner, der verschiedene Tabellen enthält, in dem Ergebnisse zusammengefasst werden. Dies schließt beispielsweise ausführliche Hypothesentests mit ein.



#---- Python Skripte -----# 


 # a_exploratory_data_analysis.py
EDA der vorab erhaltenen Marktdaten. Dieses Skript enthält beispielsweise erste Visualisierungen und bringt die Marktdaten in ein sinnvolles Format. 
Dabei wurden auch die Währungen aller Märkte vereinheitlicht und bei Bedarf in USD umgerechnet. 

 # b_main_functions.py
Dieses Modul enthält eine Vielzahl an Funktionen, die für die Datenanalyse von Nutzen sind. Das Modul wird daher auch in anderen Skripten verwendet, zum Beispiel 
in der Datei "c_signal_analysis_class.py". Es ist folglich der "Werkzeugkasten" für die Bearbeitung dieses Projekts.

 # c_signal_analysis_class.py
Modul, das anhand der Funktionen aus dem Python-Skript "b_main_functions.py" ein dementsprechendes Klassen-Objekt erstellt. Auf diese Art und Weise ist es möglich, 
verschiedene Umsetzungsmöglichkeiten, Strategien und Märkte zwar automatisiert, aber dennoch flexibel zu analysieren.
  
 # c_signal_analysis.py
Skript, das die Analyse anhand des Klassenmoduls "c_signal_analysis_class.py" ausführt. Die daraus resultierenden Ergebnisse werden in dem bereits erwähnten Export-Ordner 
gespeichert. Des Weiteren ist es im Rahmen dieses Skripts möglich, bestimmte Einstellungen zu verändern und das Analyseergebnis so dem Untersuchungsgegenstant anzupassen.

 # d_constant_mix_analysis.py
Skript, in dem verschiedene Umsetzungsszenarien anhand einer Constant-Mix Strategie untersucht wurden.

 # e_evaluation_constant_mix.py
Skript, in dem die Ergebnisse, die im Rahmen des Skripts "d_constant_mix_analysis.py" exportiert wurden, aufbereitet wurden.

 # e_evaluation_signals.py
Skript, in dem die Ergebnisse, die im Rahmen des Skripts "c_signal_analysis.py" exportiert wurden, aufbereitet wurden.

 # f_visualisations.py
Skript, in dem verschiedene Inhalte grafisch für die Präsentation aufbereitet wurden. 



