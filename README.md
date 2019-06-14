# Generate a Trusted SSL Certificate

This repository contains a script that will generate a trusted ssl certificate which can be used for local software development.

```
git clone https://github.com/daniazar/generate-trusted-ssl-certificate.git
cd <PATH_TO_REPO_FOLDER>/generate-trusted-ssl-certificate
bash generate.sh
```

## Requirements
# OS X
You should be all set. OS X has by default openssl installed.

# Windows 10
Install openssl. I recommend using the Git bash. It has openssl preinstalled. Git Bash is bundled with the Git installer.

https://git-scm.com/

## Configuration

You can adjust the `[dn]` part of the `openssl-custom.cnf` file to whatever you prefer.

```
[dn]
C = <COUNTRY>
ST = <STATE>
L = <LOCALITY / CITY>
O = <ORGANIZATION>
OU = <ORGANIZATION_UNIT>
emailAddress = <EMAIL_ADDRESS>
CN = <HOSTNAME / IP_ADDRESS>
```

## Angular
For using with angular and more information read:

https://medium.com/@rubenvermeulen/running-angular-cli-over-https-with-a-trusted-certificate-4a0d5f92747a