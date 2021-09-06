# JWT Interactive CLI Tool

This tool is intended to 
- Create JWE/JWS token
- Parsing JWE/JWS token

## Getting Started

This tool provide an interactive cli and can be extend to have more algorithm.

### Prerequisites

Terminal or equivalent tool

### Installing and Running

download the binary file based on your working environment. extract it somewhere and then you can use the CLI file.

examples:

```

sh-3.2# wget https://github.com/OkadocTech/jwtcli-public/raw/1.0/jwtcli_darwin_amd64.tar.gz

sh-3.2# tar xfz jwtcli_darwin_amd64.tar.gz

sh-3.2# ls -lh
total 7640
drwxr-xr-x  3 root  staff    96B Sep  6 15:34 build
-rw-r--r--  1 root  staff   3.7M Sep  6 15:34 jwtcli_darwin_amd64.tar.gz

sh-3.2# pwd
/Applications/XAMPP/xamppfiles/htdocs/okdc/jwtcli-public/download

sh-3.2# cd build/

sh-3.2# ls -lh
total 14944
-rwxr-xr-x  1 akangaziz  staff   7.3M Jul 27 15:36 jwtcli_darwin_amd64

sh-3.2# ./jwtcli_darwin_amd64
This tool providing key generation, parsing, token generator, etc

Usage:
  jwtcli [command]

Available Commands:
  completion  generate the autocompletion script for the specified shell
  create      Token creation
  encrypt     Token encryption
  help        Help about any command
  parse       Token parser

Flags:
  -h, --help   help for jwtcli

Use "jwtcli [command] --help" for more information about a command.
```

### How to
```
% ./jwtcli
This tool providing key generation, parsing, token generator, etc

Usage:
  jwtcli [command]

Available Commands:
  completion  generate the autocompletion script for the specified shell
  create      Token creation
  help        Help about any command
  parse       Token parser

Flags:
  -h, --help   help for jwtcli

Use "jwtcli [command] --help" for more information about a command.
```

##### Token creation\
```
% ./jwtcli create
```
Before creating a token you need to create several json files for your payload in the same directory as the binary i.e. `payload.json`   
Then you will be directed to pick one of the json file as the jwt payload, upon token creation or parsing a token you will be directed to pick any related algorithm to use and also you need to input any signature/encryption key.

##### Token parsing
```
% ./jwtcli parse --token=YOUR_TOKEN_HERE
```
You need to input the token on the `--token=` flag before continue.



## Authors

* **Khalid Adisendjaja** - *jwtcli* - [kh411d](https://github.com/kh411d)
