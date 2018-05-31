You must configure the CLI before using

 1- Set your PATH variable:
 ``` bash 
 $ export PATH=<path-to-confluent>/bin:${PATH};
 ```
 2- Optional: Specify a custom location to store the CLI data and logs. By default the Confluent CLI stores its data and logs in your platform’s temporary directory.
 You can check the current data and log location with the confluent `current` command.
 ``` bash
 $ confluent current # /tmp/confluent.gupKDQKn
 ``` 
  if you wanted to change this location  you should : 
  
  Create a directory:
  ``` bash 
  $ mkdir <path-to-confluent>/var
  ```
  Set the path to your directory:
  ``` bash
  $ export CONFLUENT_CURRENT=<path-to-confluent>/var
  ```
  
   > The `Confluent` CLI is meant for development purposes only and is not suitable for a production environment. The data that are produced are transient and are intended to be temporary. 

asdfsadfsadfasdf

## Available Commands
The available commands are:


| Command  | Description  |
| confluent acl  | Specify an ACL for a service.  |
| confluent config  | View or set connector configuration properties.  |
|   |   |

  
