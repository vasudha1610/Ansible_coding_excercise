# Ansible_coding_excercise

# Ansible_playbook1: copy file from remote to local
1. Write an ansible playbook to copy the files from a remote machine to local machine by meeting the below requirements: 
    a. A source directory inside remote machine and destination directory in local machine are the inputs, and they should be configured through a variable file. 
    b. Search for all the files inside the source directory and its subdirectories which are created in the current month, but ignore the files with .log or .out file extensions. 
    c. Zip/archive all the files selected in the previous 
    step d. Copy the zip file created in the previous step from remote machine to the destination folder inside local machine 
    e. Clean-up or delete the zip file in the remote machine.



# Ansible_playbook2: service_restart in an order
2. Let’s assume a Linux machine has a product installed which includes 3 services namely db_service, app_service and web_service
a. Lets say there is a dependency in the order of service starting. For a proper working of the product, db_service should be started first and then app_service followed by a web_service (db_service > app_service > web_service). 
So if the app_service requires a restart then app_service is restarted first and then web_service be restarted, but not db_service.
b. Using ansible handlers write a program to check the status of each service and if some service is found stopped, restart only the required services in a proper order.


# Ansible_playbook3: archive file
3. Write a playbook to archive/zip all files inside a given directory (and its sub-directories) created by a "test" user, which are older than a month.
