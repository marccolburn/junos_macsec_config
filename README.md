MACSec Configuration
=========

Configure MACSec for Junos.

Requirements
------------


Role Variables
--------------
* macsec_cas: list of dictionaries
** name: str
** cipher: str
** security_mode: str
** mka: dictionary
*** transmit_interval: str
*** key_priority: str
** ckn: str, hexadecimal 64bytes
** cak: str, hexadecimal 32bytes
** interfaces: list of dictionaries
*** name: str

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: junos_macsec_config }

License
-------

BSD

Author Information
------------------

Marc Colburn Juniper
