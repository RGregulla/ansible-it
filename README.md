# ansible-it

Installiert in ein Virtualbox Image den ServiceManager. Benötigt wird lokal ein installiertes Vagrant sowie Virtualbox.
Unter Windows bzw. einer Proxy-abhängigen Umgebung wird ein konfiguriertes CNTLM automatisch angewendet sobald das notwendige Vagrant Plugin installiert ist.
Installiert wird dieses per
    vagrant plugin install vagrant-proxyconf

Ein lokal instaliertes ansible ist nicht notwendig da das ansible playbook auf der erstellten Maschine ausgeführt wird.

Folgende Dateien sind notwendig

* webtier-9.61.zip -> provisioning/roles/sm-webtier/files
* HPSM_00946-SM-Server-Patch-Linux-961.tar -> provisioning/roles/sm-server/files
* Service_Manager_9.60_English_File_1_SM960-1.zip -> provisioning/roles/sm-server/files

Aufruf WebUI: https://localhost:8443/webtier-9.61/index.do
