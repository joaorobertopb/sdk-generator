const sdk = require('node-appwrite');

// Init SDK
let client = new Storage.Client();

let storage = new sdk.Storage(client);

client
    .setProject('')
;

let promise = storage.getFileDownload('[FILE_ID]');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});