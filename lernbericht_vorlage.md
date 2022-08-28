# Lern-Bericht
Khang Cung

## Einleitung

Wir befinden uns im Modul 133. In diesem Modul arbeiten wir mit JSF.

## Was habe ich gelernt?
Ich habe gelernt, wie man mithilfe von "ManagedBean" Daten von einer xhtml Seite auf ein anderen weiterleiten kann.

## Beschreibung

✍️ Verwenden Sie drei verschiedene Medien, um zu zeigen, was Sie gelernt haben. Zum Beispiel:

* Eine textliche Beschreibung

JSF kann man als MVC framework verstehen. Das Model ist Facelet, das View ist xhtml und der Controller ist ManagedBean. 
Beispiel:
Der Benutzer will sein Namen auf der 2. Seite anzeigen lassen. 
So wird der xhtml Code auf der 1. Seite aussehhen:
```
<h:inputText value="#{helloManagedBean.lastName}"/>
<h:commandButton value="Submit" action="seite2.xhtml"/>
```
So wird der ManagedBean aussehen: 
```java
private String lastName;
public String getLastName() {
return lastName;
}
public void setLastName(String lastName) {
this.lastName = lastName;
}
```
So wird der xhtml Code auf der 2. Seite aussehhen:
```
Ihr Nachname: <h:outputLabel value="#{helloManagedBean.lastName}"/> 
```

Auf der 1. Seite wird der Benutzer seinen Namen in einem Textfeld eingeben müssen. Danach auf die Submit Link klicken, welches ihn auf der Seite 2 weiterleitet.
Dazwischen wird das Programm durch die HelloManagedBean Controller laufen. Im Controller wird die obrigen Code durchlaufen. Der Benutzers Name wird im Variable lastName gespeichert.
Auf der 2. Seite wird die oben gespeicherte Variable wieder mit #{ControllerName.Variable} aufgerufen. 

## Verifikation

Am kurzen Erklärungstext zum ManagedBean, kann man erkennen, dass ich verstanden habe, wie man Eingaben von einer Seite auf der anderen anzeigen kann. 
Der Code beinhaltet, die wichtigsten Stellen, zum dies wiederherzustellen.

# Reflektion zum Arbeitsprozess

Ich bin mit meiner Arbeit bisher in JSF zufrieden. Ich lerne nicht gerne, neue Sprachen, weil ich bisher schon viele gelernt habe. Aber bei JSF war es eine Ausnahme, weil wir immernoch mit HTML und Java programmieren, jedoch wird es nur bei der HTML Seite anders. Dies war mir eine Herausforderung am Anfang, aber nach der Zeit verlief es mir gut.

Ich habe zur Beginn dieses Projektes sehr viel Mühe gehabt, überhaupt die Vorlage Page zu starten. Wir hatten meiner Meinung nach zu wenig Zeit gehabt, die nötigen JDKs und Netbeans etc zu installieren.

**VBV**: Ich werde bei neueren Aufträge einen kurzen Pseudo Code schreiben, damit ich schneller Fehlern beheben kann
