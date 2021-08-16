# MongoDB-ReplicaSet-preparation

First run:

    sh setup.sh

Then initiate the replica sets:

    rs.initiate({_id:"rs0", members: [{_id:0, host:"127.0.0.1:27017", priority:100}, {_id:1, host:"127.0.0.1:27018", priority:50}, {_id:2, host:"127.0.0.1:27019", arbiterOnly:true}]})
