# ec2-createlamp

This is a simple example command line client that creates a lamp server and everything you need to do that in ec2

## Build

Ensure you have maven 3.02 or higher installed, then execute 'mvn install' to build the sample.

## Run

Invoke the jar, passing your aws credentials and the name you wish to create or destroy

ex.
  java -jar target/ec2-createlamp-jar-with-dependencies.jar accesskey secretkey create adrianalmighty
  java -jar target/ec2-createlamp-jar-with-dependencies.jar accesskey secretkey destroy adrianalmighty

## License

Copyright (C) 2010 Cloud Conscious, LLC. <info@cloudconscious.com>

====================================================================
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
====================================================================