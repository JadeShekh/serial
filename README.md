# Here the python server is vulnerable to insecure desrialization and to exploit it  a python script malicious_serialization.py file creates users.json which on being deserialized by the server results in execution of remote code on the server.



Way ahead
in order to avoid the server deserializing the insecure data the hash of the serialized data needs to be passed to the server by the client over any method and then the server before deserializing the data should carry out the hash check and then deserialize the data.
