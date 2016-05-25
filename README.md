# IBM-Bluemix-data-storage-Cryptography
Prerequisites to install:
 pip install python-swiftclient
 pip install python-keystoneclient
 pip install urllib3 certifi pyopenssl2.	
 IBM Bluemix setup:
Click on dashboard then click on Cloud Foundry App then choose Web app.
Choose the starting point as python on this page.
Click on the overview of the app and then click on Add a service or API 
Under services -> select storage and then click on object storage IBM BETA
On the left side panel select ‘Environment Variables’ . These are credentials associated with your Object Storage Instance, which your bound python application will utilize to connect. 
In the code append auth_url + ‘/V3’
Use Python 2.7 idle or commandline to run the application
update the credentials, userid, projectid in LocaltoIBMBluemix.py
python LocaltoIBMBluemix.py
The localtobluemix.txt should be in the same directory
Follow instructions to
Read the local file, encrypt it & upload it to bluemix object storage
The file can be downloaded & decrypted
Objects in bluemix storage can be listed
Objects can be deleted
