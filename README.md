# F5-Networks
## Qualification de l'incident
### Descritpion
Afin de qualifier l'incident, merci de confirmer ou compléter les informations suivantes :
* Description du problème :
* Première apparition du problème (Date et heure) :
* Autres occurences du problèmes (Date et heure) :
* Cela a-t-il déjà fonctionné ?
* Message d'erreur (copier/coller le message ou joindre une capture d'écran au ticket) : 
* Avez-vous connaissance d'un changement sur le BIG-IP ou dans l'infrastructure avant l'apparition de l'incident ?
* Le problème peut-il être reproduit ?
* Etapes suivies pour tenter de résoudre l'incident :

### Impact
* L'incident concerne un utilisateur ou un groupe d'utilisateurs en particulier ?
* L'incident concerne une application en particulier ? Si oui, indiquer le virtual server concerné

## Traces
### Capture réseau
Prendre une capture de paquets :\
`tcpdump -nni 0.0:nnn host #ClientIP# -s0 -vvvw /var/tmp/$HOSTNAME.pcap`
> Merci d'indiquer à quoi correspondent les adresses IP impliquées (par exemple, l'IP du client, l'IP du virtual server, l'IP des pool members)

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
