

Auto deploy phing script for zend framework2 and doctrine 2 apps 

Structure
=================
- build.xml - main build file
- build.properties - build propertyes 
- db/sample_data.sql - Dump with sample data for import
- templates/doctrine.local.php.template template for doctrine config


Manual deployment
=================

Inside project root 

- $git clone https://github.com/snicksnk/zf-doctrine-deployment-with-phing.git deploy 
- $cd deploy
- $phing 
 


Automatic deployment
====================

```sh
$phing -buildfile path/to/build.xml  -Dnoinput="1" -Ddb.host='localhost'  -Ddb.port='3306' -Ddb.user='user' -Ddb.password='password' -Ddb.name='database'
```
