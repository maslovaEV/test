Example 1
=======
Only example 1 here

More updates 
------------
to do

Create a new provider
~~~~~~~~~~~~~~~~~~~~~

.. sidebar:: Provider
is a service provider for a stream

Request method: POST

Request format: 

.. http:post:: http://{domain}/v1/providers

.. csv-table::  Response
  :header: "Status code","Description"
  :widths: 25, 60

  "201", "Provider 'kafka-example' has been created."
  "400", "Cannot create provider. Errors: <list-of-errors>."
  "500", "Internal server error"

Request json example::

 {
     "name": "kafka-example",
     "description": "example kafka provider",
     "login": "my_login",
     "password": "my_pass",
     "type": "kafka",
     "hosts": [
       "192.168.1.133:9092",
       "192.168.1.135:9092"
       ]
 }


