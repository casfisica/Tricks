#Install Kerberos and configurate it, to be used in the lxplus CERN

<par>Install Kerberos client <par>

```bash
sudo apt-get install openafs-krb5 krb5-user kinit

```

<par>Tne configurate it to use cern server</par>

```bash
wget http://linux.web.cern.ch/linux/docs/krb5.conf
sudo cp krb5.conf /etc/

```
<par>Tne configurate it to use cern server</par>

```bash
kinit csalazar@CERN.CH
ssh -v csalazar@lxplus.cern.ch klist -f\; tokens\; touch .sshtest

```
