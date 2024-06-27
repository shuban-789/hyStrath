# Dependencies

- Critical utilities to get the install script to work
- Install OpenFOAM and ThirdParty from sourceforge
- `sudo add-apt-repository ppa:rock-core/qt4`

# Environment variables

```
WM_PROJECT_Name=(name)
WM_PROJECT_DIR=(openFOAM.tgz)
WM_USER_PROJECT_DIR=(usr dir, hystrath cloned and unzipped inside)
```

# Partitioning

Instlallation depends on space being available on /run. Partition accordingly.

```
echo "tmpfs /run tmpfs defaults,size=1G 0 0" >> /etc/fstab
sudo mount -o remount /run
```
