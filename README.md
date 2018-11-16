# postman_node_vip_pool
#How to create BIGIP node, pool and VIP in bulk using Postman
#Download files and modify environment file to udpate credentials
#Modify csv file to reflect your new config

#Run following CLI command to create new config

newman run Create_Node_Pool_VIP.postman_collection.json  -e tmsh_list.postman_environment.json  -d newbuild.csv -k

Options:
-------
-e - Specify a URL or Path to a Postman Environment.
-d - Specify a data file to use for iterations (either json or csv)
-k - Disables SSL validations 
