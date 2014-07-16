tsung-heat-template
===================

heat template to deploy tsung load testing suite

# Getting started
We will assume that you have a working heat client.

 1. First we will create our machine.
   ```
   heat stack-create -f tsung-single-node.yml tsung-test -P key_name=id_rsa-devx -P server_name=tsung-test
   ```
