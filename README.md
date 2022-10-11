# How to Install Tigergraph Enterprise Edition in Ubuntu Server?

## Prepare To Installation 
1. Download File ISO Ubuntu server 20.04 LTS. Link: https://ubuntu.com/download/server
2. Download Tigergraph Enterprise (.tar) Link: https://dl.tigergraph.com/download.html
3. Install FileZilla

## Instalasi Tigergraph in Ubuntu Server
### 1. Create Virtual Machine in Virtual Box
* Ram Minimum 8GB

* CPU Minimum 4 Cores

* Storage/Hard Disk Minimum 20GB (Install 50GB)

* Network Bridged Adapter

![image](https://user-images.githubusercontent.com/110078907/195172485-676d4220-95c3-4103-a8fd-0cb1dfab6fbe.png)


![image](https://user-images.githubusercontent.com/110078907/195172532-032f13b5-c59c-45f5-8366-7dfebfcbbfc5.png)


![image](https://user-images.githubusercontent.com/110078907/195172633-a35631ca-d9f9-41ce-ae59-9d90a8b4d993.png)


![image](https://user-images.githubusercontent.com/110078907/195172698-0fca2505-55e1-4fdf-9c97-2f75e7388900.png)


![image](https://user-images.githubusercontent.com/110078907/195172724-89b7b2d5-2cc5-47de-b5c5-db528b55f2ef.png)


![image](https://user-images.githubusercontent.com/110078907/195172766-fa9531c4-73a0-4808-b0f7-4118dd9c2d06.png)

### 2. Start Virtual Machine
* Choose auto install openSSH (opsional) [ ]->[x]

* Reboot Now

#### 3. Login with the User and Password that has been created
* Check your Ip

       $ ip a

### 4. Login in your terminal ssh
<img width="481" alt="image" src="https://user-images.githubusercontent.com/110078907/195183879-5b961688-2fce-43f7-99dc-24fee4410132.png">

* Install net-tools

       $ sudo apt install net-tools
       
* install sshpass

       $ sudo apt-get install sshpass
       
### 5. Transfer file tigergraph.tar.gz in server with Filezilla

<img width="477" alt="image" src="https://user-images.githubusercontent.com/110078907/195186194-50f118a7-e205-4470-b0a9-ddb3eb215962.png">

### 6. Extract file tigergraph.tar.gz in server
       $ tar -xzf tigergraph-3.4.0-offline.tar.gz
* open the extracted file

       $ cd tigergraph-3.4.0-offline.tar.gz
       
### 7. Run file install.sh and wait a minutes
       $ sudo ./install.sh -n

If the installation is complete it will look like this:

<img width="512" alt="image" src="https://user-images.githubusercontent.com/110078907/195188556-087d7369-f76b-4072-9a01-f45f130fb873.png">

### 8. If the installation is complete login to the tigergraph user (password default: tigergraph)
        $ su - tigergraph
        
* Check Status

        $ gadmin status
        
<img width="475" alt="image" src="https://user-images.githubusercontent.com/110078907/195190115-d3c26172-4400-4d39-b856-0a8fea6459cb.png">

### 9. Running in your Browser (port :14240)
http://192.168.18.226:14240/ (your ip)

<img width="960" alt="image" src="https://user-images.githubusercontent.com/110078907/195191079-e316cfc2-4948-4f5a-aeee-ef994ec5c28d.png">
