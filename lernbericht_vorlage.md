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

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
