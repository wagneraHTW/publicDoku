## laufende Prozesse - ohne Kernalprozesse - beobachten 

```bash 
ps -ax | grep -v " \[.*\]"
```

## Liste der offenen IP4 Verbindungen
```bash 
lsof -i 4 -n  
```
###Zu welchem paket gehört das File  
```bash 
dpkg -S  /usr/lib/postgresql/9.3/bin/psql 
#out: postgresql-client-9.3: /usr/lib/postgresql/9.3/bin/psql
```



## Schleifen 

```bash
for i in {1..5};      do echo " > $i "; done ; 
for((i=5;i>=1;i-=1)); do echo " < $i "; done ;

```




for i in {1..22};   do   ( ping -q -c 1 $comp$i ) ; done

