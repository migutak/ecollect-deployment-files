# process maker

CHRISPINE’S Profile 0725160399 chrispine.otaalo@gmail.com

To change the expiration date for all the users in PM 3 in the "workflow" workspace, you can do this from the command line of your PM server:
mysql -u root -proot
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

http://127.0.0.1:8089/sysworkflow/en/neoclassic/oauth2/applications
http://172.16.19.151:8089/sysworkflow/en/neoclassic/oauth2/applications
our application "caselister" was registered successfully!

Application Credentials

    * Client ID: YPQEXHKSFJZSZDVQVCTAJUDVFMBZDYHC
  * Client Secret: 5393352015e60c53af17a02027464074

  * Client ID: CEKOGNMZXSJTBXIPCRDVOUFISCTMGAKD
  * Client Secret: 1282642125e4ad5086c9995012845496

Next Steps

  * Make authorize requests
  * Get access tokens


ecollecttst
 * Client ID: YABZMYNJTYWRIFRZOQFZLNINHRQNLNFJ
* Client Secret: 5457597435e577227e1e175003579392

Home
Registration Success


Your application "ecollect" was registered successfully!

Application Credentials

  * Client ID: GMZXWMGXVPXDHSIKADKQVBJNSJMRYNMI
  * Client Secret: 3403119695e68332f07d878068047494

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


jdbc:oracle:thin://@172.16.210.14:1564/ecollect
ecol/L#TTc011@172.16.210.14:1564/ecollect
019E7310690800

ecol/
req -x509 -sha256 -nodes -days 365 -newkey rsa:2048 -keyout privateKey.key -out certificate.crt

docker run -it -d --name elasticsearch -p 9250:9200 -p 9350:9300 -v /app/data/elasticsearch:/usr/share/elasticsearch/data -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.6.0

http://ecollecttst.co-opbank.co.ke:5601/app/kibana#/dashboard/8c716cf0-53d3-11ea-bd82-bbc774644e87?_g=(refreshInterval%3A(pause%3A!f%2Cvalue%3A900000)%2Ctime%3A(from%3Anow%2Fw%2Cto%3Anow%2Fw))

https://ecollecttst.co-opbank.co.ke:4403/goto/c1984e27ec55535256062a2aec357159?_a=(fullScreenMode:!t)
http://ecollecttst.co-opbank.co.ke:5601/goto/1441d2733a6b9d444949e4f03782992e

1) collateral details table in bfub
pm table with sample data 
2) allocation criteria
3) Release Letter

TODO
-----------
- AD integration with Processmaker

Welcome, Kevin Miguta
Deposit 10$ MEMBERSHIP
[Your Account Balance : $0 ]
Estimated BTC to deposit ( 0.00103 )
Bitcoin Deposit Wallet Address
34fgiSmXnivxhvnUzZd8yrUbwn23iBMXae


$ch = curl_init("https://example.com/api/1.0/workflow/cases");
curl_setopt($ch, CURLOPT_HTTPHEADER, array("Authorization: Bearer " . $accessToken));
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
$aCases = json_decode(curl_exec($ch));
$statusCode = curl_getinfo($ch, CURLINFO_HTTP_CODE);
curl_close($ch);

if ($statusCode == 200) { //if successful request
   //loop through array of cases and print when each one is due:
   foreach ($aCases as $oCase) {
      print "<p>Case '{$oCase->app_title}' in task '{$oCase->app_tas_title}' is due {$oCase->del_task_due_date}.</p>\n";
   }
}


$aVars = array(
   'pro_uid'   => '325089587550b34ab5471f8086074839',
   'tas_uid'   => '491406639550b34b27f0b34088369199'
);
$oRet = pmRestRequest('POST', '/api/1.0/workflow/cases', $aVars);
$make_call = callAPI('POST', 'https://api.example.com/post_url/', json_encode($data_array));

if ($oRet->status == 200) {
   print "New Case {$oRet->response->app_number} created.\n";
}


req.open("POST", "http://127.0.0.1:8000/api/notehis",oVars, true);

    req.onreadystatechange = function() {
      if (req.readyState==4) {
        if (req.responseText) {
          console.log(req.response)
        }
      }
    } // end req
    
    req.send(null);




    url = "http://{server}/{workspace}}/oauth2/token";
method = "POST";
clientID = "Your Client ID";
clientSecret = "Your Client Secret";
user = "Your username";
password = "Your username";

$.ajax({
    url: url,
    type: method,
    data: JSON.stringify({
        "grant_type": "password",
                "scope": "",
                "client_id": clientID,
                "client_secret":clientSecret,
                "username": user,
                "password": password
    }),
    async: false, //with false => sync ; true => async
    contentType: "application/json",
    success: function (data, textStatus) {
       console.log(data);
    },
    error: function (xhr, textStatus, errorThrown) {
        console.log(textStatus);
    }
});   


[root@ab79cc1f8c6b images]# mv backgroundpm3.jpg backgroundpm3.jpg.bk
[root@ab79cc1f8c6b images]# mv logopm3login.png logopm3login.png.bk
[root@ab79cc1f8c6b images]# pw
bash: pw: command not found
[root@ab79cc1f8c6b images]# pwd
/opt/processmaker/workflow/public_html/images
[root@ab79cc1f8c6b images]#

[root@ab79cc1f8c6b css]# ls
form.css      loginStyle.css        printstyle.css  sprite.css     style.css
jscolors.css  pmos-xtheme-gray.css  rtl.css         sprite_ie.css  xtheme-gray.css
[root@ab79cc1f8c6b css]#
vi loginStyle.css

@#


52.117.54.217 root/RwUNvns4
159.122.130.146 root/YAGd5RFB

docker run -it -d --name ecollect -v /app/configs/nginx.conf:/etc/nginx/nginx.conf:ro -v /app/nginxlogs:/var/log/nginx:rw -v /app/ecollect:/usr/share/nginx/html:ro -p 80:80
ThisB!gHous#$123


module.exports = {
    oracle: {
        connector: 'oracle',
        hostname: process.env.DB_HOST || '172.16.20.2',
        port: process.env.DB_PORT || 1523,
        user: process.env.DB_USER || 'ecol',
        password: process.env.DB_PASSWORD || 'DsQSnttm_1',
        database: process.env.DB_DATABASE || 'ECOLTST',
    }
}


"oracle": {
    "host": "172.16.210.14",
    "port": 1564,
    "database": "ecollect",
    "password": "L#TTc011",
    "name": "oracle",
    "tns": "",
    "user": "ecol",
    "connector": "oracle"
  }


processmakeroracle | [04-Mar-2020 07:52:44] ERROR: [pool www] failed to read the ACL of the socket '/var/run/php-fpm/www.sock': Operation not supported (95)
processmakeroracle | [04-Mar-2020 07:52:44] ERROR: FPM initialization failed
processmakeroracle | [FAILED]

Starting php-fpm-7.1: [04-Mar-2020 08:34:10] ERROR: [pool www] failed to read the ACL of the socket '/var/run/php-fpm/www.sock': Operation not supported (95)
pmaker          | [04-Mar-2020 08:34:10] ERROR: FPM initialization failed
pmaker          | [FAILED]




