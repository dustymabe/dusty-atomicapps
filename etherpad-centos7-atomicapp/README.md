This is an atomic application based on the nulecule specification. Kubernetes and native docker are currently the only supported providers. You'll need to run this from a workstation that has the atomic command and kubectl client that can connect to a kubernetes master.

This is a multi container application based on the etherpad and mariadb

### Option 1: Interactive

Run the image. It will automatically use kubernetes as the orchestration provider.  It will prompt for all parameters in the Nulecule file that do not have default values.  These are "db_user", "db_password", and "db_name"

    $ [sudo] atomic run dustymabe/centos-etherpad-mariadb
