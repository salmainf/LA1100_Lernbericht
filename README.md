# Lernbericht_Numberguesser

Salma Tanner

## Einleitung

Ich habe als Projekt ein Numberguesser programmiert, bei dem man eine Zufallszahl zwischen 1 und 100 erraten soll.

## Was habe ich gelernt?

Ich habe gelernt, wie man die Funktionen "try" und "catch" verwendet und wozu sie dienen.

## Beschreibung

Die Funktion "try" und "catch" ist Abfangmethode für Fehler. Es überprüft das Programm auf korrekte Eingaben. Wenn die Eingabe nicht korrekt ist, sorgt es dafür das es nicht abbricht und dem Spieler die Möglichkeit gibt, es nochmals zu versuchen. Als erstes kommt immer "try", das ist die oben erwähnte Überprüfung der Eingabe, wenn es korrekt ist geht das Programm wie vorgesehen weiter. Wenn es aber nicht korrekt ist, geht das Programm weiter zu "catch", das ist die Umgehung des Abbruchs und Weiterleitung zu der Fehlermeldung. Die Fehlermeldung soll den Spieler eine Nachricht ausgeben, dass die Eingabe falsch war. Ebenfalls soll es ihm die Möglichkeit geben, nochmals spielen zu können, also noch einen Versuch. Diese Abfangmethode war ein guter Ausbau des Spiels und hat es verbessert.

![grafik](https://user-images.githubusercontent.com/110892351/189845032-318f0b8e-c77b-4906-b1d8-6101fe5f4366.png)
(Demonstrierung einer ungültigen Eingabe und der dazu programmierten Fehlermeldung)

```
 try
                {
                    int Zahl = new Random().Next(1, 100);
                    Console.Write("Erraten Sie die random Zahl zwischen 1-100:");
                    double eingabe = Convert.ToDouble(Console.ReadLine());





                    while (eingabe != Zahl)
                    {



                        if (eingabe < Zahl)
                        {
                            Console.WriteLine("Die Zahl ist grösser!");

                        }
                        else
                        {
                            Console.WriteLine("Die Zahl ist kleiner!");
                            Versuche++;
                        }
                        Console.WriteLine("geben Sie nochmals eine Zahl ein");
                        eingabe = Convert.ToDouble(Console.ReadLine());
                    }
                    if (eingabe == Zahl)

                    {
                        Console.WriteLine("Sie haben gewonnen!");
                        Console.WriteLine("Versuche:" + Versuche);
                    }
                    Console.WriteLine("Willst du nochmals spielen? [true/false]");


                    string erneut = Console.ReadLine();
                    if (erneut == "true")
                    {
                        spielen = Convert.ToInt32(1);
                    }
                    if (erneut == "false")
                    {
                        spielen = Convert.ToInt32(0);
                    }
                }
                catch
                {
                    Console.Write("Deine Eingabe ist ungültig!");
                    Console.WriteLine("Willst du nochmals spielen? [true/false]");


                    string erneut = Console.ReadLine();
                    if (erneut == "true")
                    {
                        spielen = Convert.ToInt32(1);
                    }
                    if (erneut == "false")
                    {
                        spielen = Convert.ToInt32(0);
                    }
                }

```
Der Begriff "try" und die Klammern {} überpfüfen, ob es eine gültige Eingabe ( Zahl von 1-100) ist. Wenn dies nicht so ist, geht es weiter zu "catch" und den Klammern {}, dort folgt eine Fehlerausgabe. Das sorgt dafür, dass das Programm nicht einfach abbricht sondern eine Meldung gibt. Bei mir wäre das "Deine Eingabe ist ungültig!", danach wird man gefragt, ob man erneut spielen will. Somit bekommt man nochmals eine Chance anstatt von einem Abbruch.


## Verifikation

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.

