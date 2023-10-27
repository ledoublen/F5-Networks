# F5-Networks

## Capture réseau
`tcpdump -nni 0.0:nnn host #ClientIP# -s0 -vvvw /var/tmp/$HOSTNAME.pcap`

## Qkview
### Classique
``` qkview -f /var/tmp/$HOSTNAME.qkview --progress-bar``` 
> -f pour enregistrer
> --progress-bar comme son nom l'indique
### Unlimited snaplength
`qkview -s0 -f /var/tmp/$HOSTNAME.qkview --progress-bar`

## Logs
`tar -zxvf /var/log`
## Collecte d'informations
* Quand le problème est apparu pour la première fois ?
* Est-ce une nouvelle implémentation ?
* Tentatives de résolution ?
