# Entity-Relationship-Model
Basics


Integrität - Korrektheit (Unversehrtheit) von Daten.

Datenunabhängigkeit - die Unabhängigkeit von Anwendungsprogrammen und den Daten, 
                        die die Anwendungsprogramme benötigen.
                        
Konsistenz - die Korrektheit der DB-internen Speicherungsstrukturen, 
             Zugriffspfade und sonstigen Verwaltungsinformation.

Entitätstyp - definiert eine Klasse gleichartiger Entitäten. Der Entitätstyp spezifiziert eine Menge von 
              Entitäten (Exemplaren, Instanzen) mit gleichen Attributen.

Entität (Datensatz/Tupel/Zeile) - einzelne konkrette oder abstrakte Dinge (Exemplare, Instanzen) eines Entitätstyps,
                            somit ist eine konkrette Entität immer von einem bestimmten Entitätstyp.
                            
In einer Tabelle stehen viele Entitäten gleichen Entitätstyps (Entitätsmenge).
  
Kardinalitäten - Mengenangaben der Beziehung.
                 1:1 Beziehung (wenn A mit keiner oder genau einer Entität B in Beziehung steht, und umgekehrt)
                 1:n Beziehung (wenn A mit keiner, einer oder mehreren Entitäten von B in Beziehung steht)
                 m:n Beziehung (wenn A mit keiner, einer oder mehreren Entitäten von B in Beziehung steht, und umgekehrt)

Attribut (Spalte) - Merkmal, Eigenschaft einer Entität.

Primärschlüssel - identifizierendes Attribut (eindeutig, einmalig).

Fremdschlüssel -  ist ein Attribut, das auf einen Datensatz in einer anderen Tabelle verweist. 
                  Dadurch werden die Beziehungen zwischen Tabellen realisiert.


Normalisierung -  die Aufteilung von Attributen in mehrere Relationen gemäß den Normalisierungsregeln, 
                  so dass eine Form entsteht, die keine Redundanzen mehr enthält.
                  
Ziel der Normalisierung ist es eine ausreichende Ballance aus: 
                    - geringer Redundanz (Werte eines Attributs sollen genau nur einmal in der Datenbank gespeichert sein),
                    - hoher Perfomance,
                    - hoher Flexibilität
                    zu gewährleisten. Eliminierung der Anomalien.

Datenbank-Anomalien: 
                    - Einfüge-Anomalie:     Daten können nicht in eine Datenbank übernommen werden, 
                                            da z.B. eine unvollständige Eingabe von Daten zu Inkonsistenz führt.
                    - Änderungs-Anomalie:   Die Änderung eines Werts eines Attributs erfolgt nicht an allen Stellen 
                                            der Datenbank, an dem der Wert gespeichert ist. Dies führt zur Dateninkonsistenz.
                    - Lösch-Anomalie:       Beim Löschen von Daten werden unbeabsichtigt andere mit diesen Daten in Zusammenhang 
                                            stehende Informationen ebenfalls gelöscht.
                                     
                                            
 Normalformen:      1.Normalform: Atomisierung der Attributwerte (Attribut = immer nur ein Wert, keine Liste von Werten, 
                                                                  keine zusammengesetzte Werte)                            
                    2.Normalform: wenn 1.Normalform gegeben ist, und jedes Nicht-Schlüsselattribut voll funktional 
                                  vom gesamten Primärschlüssel abhängig ist.
                    3.Normalform: wenn die 2.Normallform gegeben ist, und zwischen den Nicht-Primärschlüsselattributen 
                                  keine Abhängigkeiten bestehen.
                                  

                                            
                                            
                                            
                                            
                                            
                      
