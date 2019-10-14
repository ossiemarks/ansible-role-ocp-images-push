ansible-role-ocp-images-push
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

You can use the ansible-role-ocp-image-pull to pull images. This needs to be run before using this role.

Example Playbook
----------------

- name: OpenShift Disconnected Prep
  hosts: localhost
  become: true

  tasks:
    - name: "Include the image push role"
      include_role:
        name: ../roles/ansible-role-ocp-image-push

License
-------

MIT

Author Information
------------------

Ken Hitchcock
github.com/KenHitchcock
