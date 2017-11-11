# Inventory Service
GrabNow Inventory Service Backend. Service exposed as REST End-Points.

## Data-Store
GrabNow Inventory uses Mongodb as Data Store. Schemaless nature of Mongo caters to the flexible attribute requirements of merchant and Inventory domain entities. Mongo db will function in Replica-Set mode for high availability. Data partitionioning is obtained by virtue of Sharding feature of this NoSQL.  

## Containerization
GrabNow Inventory Service makes use of Docker to Containerize the service. For Development purpose mongo db is in isolated container local to the service.

## Security
Service will be protected by Secure tokens maintained by OAuth 2.0 Security domain.  

## Collaborator Access
for access first generate a public key using

~~~
$ ssh-keygen
~~~

Once the public key is generated, request access to the GrabNow administrator along with the key. After confirmation that the key has been added to the github account, run the following commands:

~~~
$ ssh-add <key>
~~~
adds RSA identities to the authentication agent

~~~
$ ssh -T git@github.com
~~~
