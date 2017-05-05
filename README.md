java_deps
=========

## Deeplearning4j build environment

This is a provisioning role to create build machines capable of building the
deeplearning4j projects from scratch: [libnd4j](https://github.com/deeplearning4j/libnd4j), [nd4j](https://github.com/deeplearning4j/nd4j), [datavec](https://github.com/deeplearning4j/datavec), [deeplearning4j](https://github.com/deeplearning4j/deeplearning4j).

The test for these is running the main repo's [build script](https://github.com/deeplearning4j/deeplearning4j/blob/master/build-dl4j-stack.sh).

If you need to run this locally:
```
ansible-galaxy install huitseeker.java_deps
cat << EOF > provision.yml
---
- hosts: all
  roles:
    - huitseeker.java_deps
EOF
ansible-playbook -b -i "localhost," -c local provision.yml
```

Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------


License
-------

BSD
