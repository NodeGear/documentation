Local deploy
============

Dependencies
------------

- Vagrant
- Ansible
- Virtualbox
- Be running Linux/OSX

Reserved addresses
------------------

+-----------+--------------+
| Address   | Purpose      |
+===========+==============+
| 10.0.3.2  | Services     |
+-----------+--------------+
| 10.0.3.4  | Frontend     |
+-----------+--------------+
| 10.0.3.3  | Backend      |
+-----------+--------------+

Local deployment
----------------

::

	├── ng-docker-registry
	├── ng-documentation.git
	├── ng-frontend
	├── ng-fs
	├── ng-git
	├── ng-infrastructure
	├── ng-models

``cd`` into ``ng-frontend`` and run ``vagrant up``

Vagrant will start and provision *Services* and *Frontend* boxes.

  There seem to be a few quirks with ansible and multiple boxes in one vagrantfile so splitting may be necessary.
