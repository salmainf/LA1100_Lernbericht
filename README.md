# Lernbericht_Numberguesser

Salma Tanner

## Einleitung

Ich habe als Projekt ein Numberguesser programmiert, bei dem man eine Zufallszahl zwischen 1 und 100 erraten soll.

## Was habe ich gelernt?

Ich habe gelernt, wie man die Funktionen "try" und "catch" verwendet und wozu sie dienen.

## Beschreibung



* Eine textliche Beschreibung

![grafik](https://user-images.githubusercontent.com/110892351/189845032-318f0b8e-c77b-4906-b1d8-6101fe5f4366.png)

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

