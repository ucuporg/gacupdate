# update
# INSTALL UPDATER GENIEACS OTOMATIS

```
apt install git curl -y
```
```
git clone https://github.com/alijayanet/update
```
BACKUP SETINGAN GENIEACS YANG SUDAH ADA 
```
sudo mongodump --db=genieacs --out genieacs-backup >/dev/null 2>&1
```
RESTORE/UPLOAD PRESET PROVISION VIRTUAL PARAMETER UPDATEA 
```
sudo mongorestore --db=genieacs --drop update >/dev/null 2>&1
```
Jika IP URL ACS anda bukan http://192.168.8.89:7547 harap segera di ganti <br>
Untuk menghindari ONU yang kerubah IP URL ACSnya di ADMIN PROVISION INFORM <br>


Jika dirasa kurang pas di hati njenengan silahkan RESTORE setingan sampean
```
sudo mongorestore --db=genieacs --drop genieacs-backup >/dev/null 2>&1
```
