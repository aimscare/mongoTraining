# mongoTraining


https://www.pluralsight.com/courses/mongodb-administration

https://www.pluralsight.com/courses/mongodb-introduction

We are very pleased to invite you to a 1 day team workshop “MongoDB Administration" held at

Arts House
1 Old Parliament Lane
Singapore 179429
www.theartshouse.sg

on Wednesday 16th May 09:00 – 19:00.

The workshop will be held as a Pluralsight online video training. The main purpose should be to gain an principle understanding MongoDB and operate a MongoDB as NoSQL database in a productive environment. This is to enable us, to eventually implement and operate a CRAFT Mongo to safely persist documents and get experiences as NoSQL is increasingly used in applications across various industry sectors. 

Although we will form teams, for better experience please bring along your own laptops to the workshop. We aim to have a workshop at which all participants will actively be engaged and have the time to share their thoughts and experiences and learn from each other. In order for this to happen, we kindly ask you to prepare the following:

Prepare your laptop by install the following software prerequisites:

MongoDB will be hosted on a Linux server. In case you don’t have a laptop, that comes with a Unix derivate (MacOS, Ubuntu, RedHat, …) install

•	Oracle VirtualBox 5.2.10 (https://www.virtualbox.org/wiki/Downloads) with Ubuntu 16.04.4 Xenial - 64bit (https://www.osboxes.org/ubuntu/) as guest system
Helpful Link(s): 
https://linus.nci.nih.gov/bdge/installUbuntu.html
https://medium.com/@tushar0618/install-ubuntu-16-04-lts-on-virtual-box-desktop-version-30dc6f1958d0

•	MongoDB Community Server - Stable Release (3.6.4) (https://www.mongodb.com/dr/fastdl.mongodb.org/linux/mongodb-linux-x86_64-ubuntu1604-3.6.4.tgz/download)
Helpful Link(s): 
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-linux/

•	Putty (https://www.putty.org/), Mobaxterm (https://mobaxterm.mobatek.net/download.html) or similar client 

•	FileZilla (https://filezilla-project.org/) or similar

•	Get yourself a GitHub Account (https://github.com/join) as we will share keep our training artefacts in there, so nothing is lost



http://www-conf.slac.stanford.edu/xldb2010/docs/xldb4_wed1615_lightning_8_mongodb.pdf

https://github.com/callicoder/spring-boot-mongodb-angular-todo-app


https://dba.stackexchange.com/questions/82591/sample-yaml-configuration-files-for-mongodb


Read preference:

https://www.alibabacloud.com/help/doc-detail/52344.htm

https://docs.mongodb.com/manual/reference/method/js-connection/

https://sg.simplilearn.com/replication-and-sharding-mongodb-tutorial-video



db

db.createUser({ user: "craftread" , pwd: "craftread", roles: [{role:"read", db:"admin"}]})

db.createUser({ user: "craftrw" , pwd: "craftrw", roles: [{role:"readWrite", db:"admin"}]})



db.stats()

db.auth("admin", "admin")

show users

rs.status()

db.getUser("craftrw")




rs.initiate()

rs.status()



rs.add("ip:2002")

rs.add("ip:2003")

rs.remove("ip:2003")

rs.addArb("ip:2003")


db.printSlaveReplicationInfo()

show dbs


rs.conf()


use craft

db.attachments.save({"fileName":"craft.pdf","tranxId":"1"})   

db.attachments.find().pretty();

db


db.todos.find().pretty();

db.todos.count();









