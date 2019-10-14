Role Name
=========

Role written to speed up the process of retagging and pushing container images to an internal repository.

Requirements
------------
Will need either images already pulled locally or a tar file with images to import.
Role also assumes docker is installed. Future versions will consider other container runtimes.

Role Variables
--------------


Dependencies
------------


Example Playbook
----------------

Example playbook
    - hosts: servers
      roles:
         - ansible-role-ocp-images-push

License
-------

MIT

Author Information
------------------

Ken Hitchcock
github.com/KenHitchcock
