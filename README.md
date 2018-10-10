# lowdb-google-cloud-storage-adapter
This let you to create and use a lowDB source located on Google cloud storage

## Installation

`npm i --save lowdb-google-cloud-storage-adapter`

## Usage

``` javascript
const GcloudAdapter = require('lowdb-google-cloud-storage-adapter');
const low = require('lowdb');

const adapter = new GcloudAdapter('db.json', {
  projectId:"Project Id",
  keyFilename:"Key file path",
  bucketName:"Bucket name",
});

const db = low(adapter);

```
