# Dependencies

- Critical utilities to get the install script to work
- Install OpenFOAM and ThirdParty from sourceforge
- `sudo add-apt-repository ppa:rock-core/qt4`

# Partitioning

Instlallation depends on space being available on /run. Partition accordingly.

```
echo "tmpfs /run tmpfs defaults,size=1G 0 0" >> /etc/fstab
sudo mount -o remount /run
```

# Loading systems

In templated systems, first run the `Allrun` script to create vital files. You will have to recreate this script for your own simulation.

In cmdline, type:
```
dsmcFoam+
```
