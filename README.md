# kickstart-files
CentOS 7 Kickstart Files


## SSH-Key
Während der Installation können Sie die SSH-Verbindung konfigurieren. Man Verwenden den Befehl sshpw, um temporäre Konten zu erstellen, über die ihr euch anmelden könnt. Diese Konten werden nicht auf das installierte System übertragen.
Syntax: 

```sshpw --username=name password [--iscrypted|--plaintext] [--lock]```


`--username` 		Gibt den Namen des Benutzers an. Diese Option ist erforderlich.

`--iscrypted` 	Wenn diese Option vorhanden ist, wird angenommen, dass das Kennwortargument verschlüsselt ist.

`--plaintext`	  Wenn diese Option vorhanden ist, wird angenommen, dass das Kennwort in Klartext vorliegt.

`--lock`    	  Wenn diese Option vorhanden ist, ist dieses Konto standardmässig gesperrt. Dies bedeutet, dass sich der Benutzer                    								nicht von der Konsole aus anmelden kann.

Standardmässig wird der SSH-Server während der Installation nicht gestartet. Um ssh während der Installation verfügbar zu machen, starten Sie das System mit der Kernel-Boot-Option `inst.sshd`.
