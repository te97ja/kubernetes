this will let u deploy pods on to the node u desire
first u need to label the nodes with the following 
# kubectl label nodes <node name> size=large
 size=large is a key value pair an di can be anything=anything

if u mention wrong label name in the yml file other thn the one configured
the pods will be in pending stage ,they wont deploy

