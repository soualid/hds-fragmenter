# HDS-Fragmenter

HDS-Fragmenter is a tool for splitting HTTP Dynamic Streaming (HDS) segment files (.f4f), as generated by Adobe's f4fpackager, into individual fragment files. These fragments can be uploaded and played from a regular web server or a cloud service like Amazon S3, removing the need for the apache-origin module.

## Installation

HDS-Fragmenter requires node.js and makes use of the npm package tool for managing the required dependencies. Before getting started, be sure to install the necessary local dependencies:

```
$ npm install
```

After installation of the dependencies, you'll be able to run the software.

## Usage

HDS-Fragmenter should be run from command line using the following command:

```
$ node extract --input <HDS manifest (.f4m) file> --output [directory to store the HDS fragments]
```

## Limitations

HDS-Fragmenter currently <s>only supports DRM-free video segments</s> supports both DRM-free video segments and video segments protected using Adobe Access. Special thanks go to Derek Spencer for testing and confirming this functionality works. If you have any additional inquires or requests about DRM functionality for HDS-Fragmenter do not hesitate to [contact](mailto://contact@opentelly.com) us.

## Bug tracker

Have a bug or a feature request? [Please open a new issue](https://github.com/OpenTelly/hds-fragmenter/issues). Before opening any issue, please search for existing issues and read the [Issue Guidelines](https://github.com/necolas/issue-guidelines), written by [Nicolas Gallagher](https://github.com/necolas/).

## Authors

**Maarten Tielemans**

+ [Github](http://github.com/Tielem)
+ [LinkedIn](http://linkedin.com/in/mtielemans)

**Pieter-Jan Speelmans**

+ [Github](http://github.com/pjsp)
+ [LinkedIn](http://linkedin.com/in/pieterjanspeelmans)

**Steven Tielemans**

+ [LinkedIn](http://be.linkedin.com/in/steventielemans)

**OpenTelly**

+ [Website](http://www.opentelly.com)
+ [Email](mailto://contact@opentelly.com)

**Special thanks to**

+ Derek Spencer ([LinkedIn](http://linkedin.com/in/derekspencer))

## Copyright and license

Copyright 2013 The Virtual Cable Company, BVBA.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

  [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.