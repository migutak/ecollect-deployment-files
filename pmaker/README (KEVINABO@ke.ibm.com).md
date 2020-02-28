# process maker

CHRISPINE’S Profile 0725160399 chrispine.otaalo@gmail.com

To change the expiration date for all the users in PM 3 in the "workflow" workspace, you can do this from the command line of your PM server:
mysql -u root -p
use wf_workflow;
UPDATE USERS SET USR_DUE_DATE='2025-12-31';
UPDATE RBAC_USERS SET USR_DUE_DATE='2025-12-31';

If you only want to change the expiration date for certain users:
UPDATE USERS SET USR_DUE_DATE='2020-12-31' WHERE USR_USERNAME IN ('mary', 'joe', 'sally');
UPDATE RBAC_USERS SET USR_DUE_DATE='2020-12-31' WHERE USR_USERNAME IN ('mary', 'joe', 'sally');


Your application "caselister" was registered successfully!

Application Credentials

  * Client ID: BKFXXRQJBQHEGBMSPXTONUPUUKBMEBOC
  * Client Secret: 5628087865e3d2c6b652b80018624665

Next Steps

  * Make authorize requests
  * Get access tokens

Kubernetes ALL nodes grafana

http://127.0.0.1:8085/sysworkflow/en/neoclassic/oauth2/applications

our application "caselister" was registered successfully!

Application Credentials

  * Client ID: PPMBHKKHMDRYMJRLXJPCNGYREZLGONEH
  * Client Secret: 2467532265e49abb66b1707010030223

  * Client ID: CEKOGNMZXSJTBXIPCRDVOUFISCTMGAKD
  * Client Secret: 1282642125e4ad5086c9995012845496

Next Steps

  * Make authorize requests
  * Get access tokens


POST http://127.0.0.1:8085/workflow/oauth2/token

{
      "grant_type":"password",
      "scope":"*",   
      "client_id":"PPMBHKKHMDRYMJRLXJPCNGYREZLGONEH",
      "client_secret":"2467532265e49abb66b1707010030223",
      "username":"admin",
      "password":"admin"
}

{
    "access_token": "7a8b202174d0e56486a9919181f347d2c111bd6d",
    "expires_in": 86400,
    "token_type": "bearer",
    "scope": "*",
    "refresh_token": "a083ef4b9bbd6184310bd64b5f955adea27c2bcc"
}


$.post("http://192.168.0.5:80/medres/oauth2/token", {
        dataType: 'json',
        grant_type: 'password',
        scope: '*',
        client_id: 'client_id',
        client_secret: 'client_secret',
        username: 'user',
        password: 'password'
    }, function(data){
        console.log(data);
        var d = new Date();
        d.setTime(d.getTime() + 60*60*1000);
        document.cookie = "access_token="  + data.access_token  + "; expires=" + d.toUTCString();
        document.cookie = "refresh_token=" + data.refresh_token; //refresh token doesn't expire 
    })


    $.post('http://192.168.0.5/api/1.0/medres/cases', {
                        access_token: getCookie('access_token'),
                        pro_uid: '3827944695a42a7990f0655045007841',
                        tas_uid: 'sme-129625a4d1cc557f110087068990',
                        variables: {
                           'data': object
                        }
                    }, function(data){
                        console.log(data)
                    })


docker run -it -d --name nginx -v /app/certs/ecollectweb.co-opbank.co.ke.key:/etc/nginx/ecollectweb.co-opbank.co.ke.key:rw -v /app/configs/nginx.conf:/etc/nginx/nginx.conf:ro -v /app/nginxlogs:/var/log/nginx:rw -v /app/certs/ecollectweb.co-opbank.co.ke.crt:/etc/nginx/ecollectweb.co-opbank.co.ke.crt:rw -v /app/ecollect:/usr/share/nginx/html:ro -p 80:80 -p 443:443 nginx:coop


docker run -it -d --name ecollect -v /app/configs/nginx.conf:/etc/nginx/nginx.conf:ro -v /app/ecollect:/usr/share/nginx/html:ro -p 80:80 nginx:1.17.1-alpine

kubeadm join --token ul75vc.6w5ewgeeaw7ck8mp 172.16.204.72:6443 --discovery-token-ca-cert-hash sha256:<hash>

kubeadm join 172.16.204.72:6443 --token ul75vc.6w5ewgeeaw7ck8mp --discovery-token-ca-cert-hash sha256:b88c224233e7f90cda60646e625979d460d01e16c3c99be1e1c430b7ef9c07a8


Work on configuration section for i.e create menu under configurations for
1) Insurance companies
2) Service providers

Be able to perform add, delete, update


ServiceProviders
	id
	providerName
	physicalAddress
	postalAddress
	emailAddress
	indeminityExpiry
	contactPerson
	dateofEntry
	dateofLastUpdate

Insurances
	id
	insuranceName
	physicalAddress
	postalAddress
	emailAddress
	contactPerson
	dateofEntry
	dateofLastUpdate



