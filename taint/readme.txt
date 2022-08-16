firstly if u need to use taint tolerations ,u need to taint the node with the
following command 

#kubectl taint nodes <node name> colour=red:NoSchedule
 colour=red is a key=value pair ,it can be anything 
 NoSchedule is the effect type


taint and toleartion gives no guarantee that the pods will be deployed on the
tainted node .but if the regular nodes are fulla dn there is no availability ,then 
the pods will be deployed in the tainted nodes.
