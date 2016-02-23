Reproduce bug : Role Dependencies and include statement with ansible 2
=======================================================================

  * https://github.com/ansible/ansible/issues/14625

Reproduce :

```
git clone https://github.com/gaelL/_ansible2_bug_include
cd _ansible2_bug_include
ansible-playbook -i hosts site.yml
```

Files : 

```
./hosts
./site.yml
./roles/bar/meta/main.yml
./roles/foo/tasks/include_level2.yml
./roles/foo/tasks/main.yml
./roles/foo/tasks/include_level1.yml
./roles/foo/defaults/main.yml
```
