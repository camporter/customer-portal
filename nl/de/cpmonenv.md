---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Umgebung und Systemereignisse überwachen
{: #customerportal_cpmonenvsysevent}

Durch die Überwachung Ihrer Umgebung haben Sie die Möglichkeit, Geräte jederzeit zu überprüfen, und werden automatisch benachrichtigt, wenn eines Ihrer Geräte ausfällt. Sie können außerdem Systemereignisse überwachen und so für einen reibungslosen Betrieb Ihrer Systeme sorgen.  
{: shortdesc}

## Umgebung überwachen
{: #cpmonenv}

Verwenden Sie mindestens die Basisüberwachung mit Pingsignalen. Sie können jedoch Ihre Überwachungsoptionen so anpassen, dass Ihre Geschäftsanforderungen optimal erfüllt werden.

### Über Netzwartung und ungeplante Ereignisse informiert bleiben
{: #cp_stayinfomaintevent}

Geplante und Notfallnetzwartungen sind von Zeit zu Zeit unvermeidbar. In der {{site.data.keyword.BluSoftlayer_full}}-Infrastruktur werden viele Kanäle (z. B. [Twitter-Konten ![Symbol für externen Link](../icons/launch-glyph.svg)](https://twitter.com/softlayernotify){:new_window}) unterhalten, damit Sie stets über alle geplanten und Notfallwartungsereignisse informiert sind. Darüber hinaus können Sie [E-Mail-Benachrichtigungen abonnieren](/docs/customer-portal/cpsub2not.html){:new_window}, die vom Ereignismanagementsystem ausgegeben werden. Dieser ergänzende Service sendet an Benutzer mit einem entsprechenden Abonnement automatisch E-Mails über ungeplante Ereignisse, die sich auf Services auswirken könnten.

### {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für Mobilgeräte nutzen
{: #cp_bmxinframobile}

Verwenden Sie die [{{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für Mobilgeräte ![Symbol für externen Link](../icons/launch-glyph.svg)](https://knowledgelayer.softlayer.com/topic/mobile-devices){:new_window}, um Ihre Geräte für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur unterwegs über Ihr mobiles iOS- oder Android-Gerät zu verwalten. Die Funktionalität in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für Mobilgeräte beinhaltet Ticketingunterstützung, Basisgerätesteuerung und Bandbreitenüberwachung.

## Systemereignisse überwachen
{: #customerportal_monevent}

Sie können Systemereignisse überwachen, indem Sie Prüfprotokolle und Zugriffsprotokolle einsehen.

### Prüfprotokoll für ein Konto anzeigen
{: #cp_viewacctauditlog}

Jedes Kundenportalkonto wird zusammen mit einem Prüfprotokoll bereitgestellt, in dem die Interaktionen jedes Benutzers im Kundenportal aufgezeichnet werden. Zu den aufgezeichneten Interaktionen gehören Anmeldeversuche (erfolgreich und erfolglos), Aktualisierungen der Portgeschwindigkeit, Systemstarts oder -beendigungen und Warmstarts sowie diejenigen Interaktionen, die von den Mitarbeitern des Support-Teams für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur ausgeführt werden. Führen Sie die folgenden Schritte aus, um ein Prüfprotokoll für ein Benutzerkonto anzuzeigen.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto** > **Verwalten** > **Prüfprotokoll** aus, um auf das Prüfprotokoll zuzugreifen.

Im Prüfprotokoll werden anfangs die letzten 25 Interaktionen von Benutzern mit dem Konto angezeigt. Sie können jederzeit bis zu 200 Interaktionen anzeigen. Die Anzahl der angezeigten Ergebnisse können Sie in der Dropdown-Liste **Anzeigen** aktualisieren. Falls Einstellungen geändert wurden, enthält die Spalte **Aktion** für die Interaktion einen Link. Klicken Sie auf einen dieser Links, um die durch die Aktion beeinflusste Einstellung sowie Details über die Änderung anzuzeigen. Wenn Sie auf den Gerätenamen oder Benutzernamen für eine Interaktion klicken, werden Sie zur Anzeige mit den Gerätedetails bzw. zur Anzeige mit dem Benutzerprofil weitergeleitet.

### Zugriffsprotokoll eines Benutzers anzeigen
{: #cp_viewuserlogs}

Zugriffsprotokolle zeigen Daten für jeden Zugriffsversuch an, der durch einen bestimmten Kundenportalbenutzer unternommen wurde. In den Protokollen sind für jeden Zugriffsversuch eine Datums-und Zeitmarke und eine IP-Adresse angegeben. Führen Sie die folgenden Schritte aus, um das Zugriffsprotokoll eines Benutzers anzuzeigen.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} zu.
2. Wählen Sie in der Menüleiste die Optionen **Konto** > **Benutzer** aus, um auf das Fenster 'Benutzer' zuzugreifen.
3. Wählen Sie in der Dropdown-Liste **Aktionen** den Eintrag **Prüfprotokoll anzeigen** aus, um das Zugriffsprotokoll des Benutzers anzuzeigen.

Im Zugriffsprotokoll werden für jeden Benutzer die von ihm unternommenen Zugriffsversuche nach Datum sortiert zusammen mit der IP-Adresse angezeigt, über die der Zugriffsversuch erfolgte. Die Informationen im Zugriffsprotokoll sind schreibgeschützt, so dass zu keinem Zeitpunkt Änderungen am Inhalt vorgenommen werden können. Sie können das Zugriffsprotokoll jederzeit erneut anzeigen, indem Sie die obigen Schritte wiederholen. Um die Protokolle zu verlassen und zur Anzeige 'Benutzer' zurückzukehren, klicken Sie oben in der Anzeige auf den Link **Alle Benutzer anzeigen**.