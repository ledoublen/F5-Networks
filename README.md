# F5-Networks
## Qualification de l'incident
* Première apparition du problème ? (Date et heure)
* Cela a-t-il déjà fonctionné ?
* Avez-vous connaissance d'un changement dans l'infrastructure qui pourrait 
* Tentatives de résolution ?

## Traces
### Capture réseau
Prendre une capture de paquets :\
`tcpdump -nni 0.0:nnn host #ClientIP# -s0 -vvvw /var/tmp/$HOSTNAME.pcap`

### Qkview
Générer un fichier de diagnostique (Qkview) :\
`qkview -s0 -f /var/tmp/$HOSTNAME.qkview --progress-bar`

### Logs
`tar -zxvf /var/log`

## Joindre les traces
Puis nous transmettre les éléments :
* Capture(s) réseau
* Qkview(s)
* Archive .tgz des logs
