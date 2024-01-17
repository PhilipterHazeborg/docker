[quick-start](https://cloud.philipterhazeborg.de/s/ZSJ5PKEdfza7zSs)

## TODO
- [x] mariaDB
- [x] adminer
- [x] openldap
- [x] phpldapadmin
- [x] redis
- [x] nextcloud
    - [x] ldap-Zugriff
    - [x] redis
- [x] moodle
    - [x] ldap-Zugriff
    - [x] redis

## Domäne
dc=bbs1,dc=local
FQDN: dc.local
|benutzer       |password   |server     |
|---------------|-----------|-----------|
|admin          |admin      |ldap       |
|nxcAdmin       |admin      |nextcloud  |
|root           |root       |mariadb    |
|nextcloud      |nextcloud  |mariadb    |
|moodle         |moodle     |mariadb    |
|redis          |redis      |redis      |
|user           |bitnami    |moodle     |

## Ports
### openldap
|external|internal|
|--------|--------|
|389     |389     |
|636     |636     |

### phpldapadmin
|external|internal|
|--------|--------|
|8080    |80      |

### mariadb
FQDN: mariadb
|external|internal|
|--------|--------|
|3306    |3306    |

### phpmyadmin
FQDN: phpmyadmin
|external|internal|
|--------|--------|
|8081    |80      |

### moodle
FQDN: moodle
|external|internal|
|--------|--------|
|80      |8080    |
|433     |8443    |

### nextcloud
FQDN: nextcloud
|external|internal|
|--------|--------|
|8008    |80      |

### redis
FQDN: redis
|external|internal|
|--------|--------|
|6379    |6379    |
