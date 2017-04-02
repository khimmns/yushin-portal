# yushin-portal

## Settings

* node v6.10.1
* Serverless 1.10.1
* aws-cli 1.11.70

1. node
```
$ git clone git://github.com/creationix/nvm.git ~/.nvm
$ source ~/.nvm/nvm.sh
$ nvm install v6.10.1
$ nvm use v6.10.1
```

2. Serverless
```
$ npm install -g serverless
$ npm install aws-sdk
$ npm install --save-dev serverless-offline
$ npm install --save-dev serverless-dynamodb-local
$ sls dynamodb install
```

3. AWS cli
```
$ curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"
$ sudo python get-pip.py
$ sudo pip install awscli
$ aws configure
AWS Access Key ID [None]: <your AWS Access Key>
AWS Secret Access Key [None]: <your AWS Secret Access Key>
Default region name [None]: <your default region>
Default output format [None]: json
``` 

---
## Local Testing

1. Lambda Function Local Testing 
```
$ sls offline
```

2. Dynamodb Local Testing
```
$ sls dynamodb start
```



