const sdk = require('node-appwrite');

// Init SDK
let client = new Avatars.Client();

let avatars = new sdk.Avatars(client);

client
    .setProject('')
;

let promise = avatars.getBrowser('aa');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});