### Run 

    #make sure you have base image available
    oc create -f https://raw.githubusercontent.com/rarodrigues9/redis-openshift/master/openshift/is-base.yaml -n openshift
    #create all components
    oc create -f https://raw.githubusercontent.com/rarodrigues9/redis-openshift/master/list.yaml
    #start build and watch 
    oc start-build redis-build
