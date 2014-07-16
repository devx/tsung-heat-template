tsung-heat-template
===================

heat template to deploy tsung load testing suite

# Getting started
We will assume that you have a working heat client.

 1. First we will create our machine.
   ```
   heat stack-create -f tsung-single-node.yml tsung-test -P key_name=id_rsa-devx -P server_name=tsung-test
   ```


# Automated single node testing
Not complete yet

```
heat stack-create -f tsung-single-node.yml tsung-test -P key_name=id_rsa-devx -P server_name=tsung-test -P target_ip=my.testing-site.com  -P tung_test_xml="$(< test_script.xml)"
```


# Planned tests
I have planned a multi node automated test that will do the following:

  1. Setup a master node
  2. setup "X" nodes and join them automatically to the master node
  3. exute test from various nodes
