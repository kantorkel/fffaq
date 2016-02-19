Lässt sich die original Firmware wieder einspielen?
--------------
Ja! Ein bereits in einen Freifunk-Knoten umgewandeltes Gerät kann jederzeit wieder mit der original Hersteller-Firmware geflasht (bespielt) werden.

Wie schnell ist mein Zugang im Freifunk?
--------------
Innerhalb des Funknetzes hängt die Geschwindigkeit stark von der Qualität der Funk-Verbindung ab und über wie viele Knoten sie geht. Die Geschwindigkeit der Knoten ins kabelgebundene Netz (z.B. Internet) wird jedoch maßgeblich durch die Prozessor-Leistung der Knoten begrenzt. Denn die müssen den VPN-Tunnel ver- & endschlüsseln, was viel Rechenleistung benötigt. Gemessene Richtwerte pro Modell findest Du unter https://projects.universe-factory.net/projects/fastd/wiki/Benchmarks.

Mein Freifunk-Router spannt ein zweites WLAN mit einer MAC-Adresse wie z.B. f8:d1:11:87:52:2e auf. Was bedeutet das?
--------------
Das zweite WLAN mit einer SSID in Form einer MAC-Adresse ist ein Ad-hoc-WLAN und dient der Vernetzung der einzelnen Router untereinander. “Sehen” sich zwei Freifunk-Konten in ihrem Empfangsbereich, so nehmen sie über diese WLAN-SSID miteinander Kontakt auf und leiten den Datenverkehr weiter. Wie sprechen dann davon, dass sie “meshen”, der eigentlichen Funktion des Freifunk-Netzes.

Kann ich den Funkkanal wechseln?
--------------
Freifunk arbeitet auf Kanal 1. Da sich die einzelnen WLAN-Knoten nur miteinander vernetzen können, wenn auch alle auf dem selben Kanal funken, macht eine Änderung keinen Sinn. Eine Veränderung des Kanals würde dazu führen, dass ein Router nicht mehr seine Kernfunktion, das “Meshen”, erfüllen kann, es sei denn, alle anderen Router würde auch umgestellt. Sollte es zu Kollisionen mit benachbarten Netzen kommen, schlagen wir den diplomatischen Weg vor, indem man sich mit seinen Nachbarn über die Kanalbelegung abstimmt.

Kann ich meine Knotendaten (Name, Ort auf der Knotenkarte, etc.) ändern?
--------------
Ja! Du kannst diese Daten selbständig mit dem Token, den du bei der Einrichtung erhalten hast unter https://formular.hamburg.freifunk.net ändern. Solltest du den Token verlegt haben, schreibe uns mit der Adresse, die du bei der Einrichtung hinterlegt hast und wir schicken ihn dir zu.

Wie ist die Belegung der Ports?
--------------
Die Standarbelegung für die LAN-Ports (gelb bei TP-Link) ist client-Netz – also für Endgeräte im Freifunknetz, genauso als wären sie per WLAN verbunden.

Der WAN-Port (blau bei TP-Link) macht standardmässig entweder Mesh-VPN (VPN-uplink zum Gateway) und sollte dementsprechend hinter einem Internet-Anschluss hängen, oder Mesh-on-WAN (also meshen per Kabel), solltest du das im Konfigurationsmodus so eingestellt haben.

Kann ich Uplink über WLAN machen statt über Kabel?
--------------
Prinzipiell ja. Allerdings ist es nicht sehr Effizient, da dann schon Mesh, client-Netz, alle clients sowie der Router zu dem als Uplink verbunden wird auf dem selben Kanal funken. Hinzu kommen evtl. Geräte aus der Nachbarschaft, die vielleicht auch auf diesem Kanal sind.
