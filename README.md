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

## Available Commands
The available commands are:


| Command            | Description |
|--------------------|--------------|
| confluent acl      | Specify an ACL for a service. 
| confluent config   | View or set connector configuration properties. 
| confluent current  | Print the filesystem path of the data and logs of the services managed by the current Confluent run. If such a path does not exist, it will be created.
| confluent destroy  |  Delete an existing Confluent run.
| confluent help     | Print command information.
| confluent list     | 	List all available services or plugins.
| confluent load     | Load a bundled connector with a predefined name or custom connector.
| confluent log      | View a snapshot or tail the log of a service.
| confluent start    | Start Confluent Platform services.
| confluent stop     | Stop services.
| confluent top      | View service resource usage.
| confluent unload   | Unload a connector.

  
