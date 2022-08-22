
<p align="center"> <img src="Project Elements/Simple_Email_Beacon.png"/> </p>

<hr>
<br/>

```SEB``` is the easiest and most secure way to track outgoing emails.

## Use Case
As cyber security enthusiasts, we have come to understand over 95% of cyber crimes are due to human error and over 90% of these crimes are carried out through email. Our goal was to create a tool that allows you to track your emails with as many data points as possible. With this, you will be able to get data of each time someone opens your email along with the

```
- IP Address
- Date and Time
- Estimated Location Coordinates
```


## Installation

Use the package manager [npm]([https://pip.pypa.io/en/stable/](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)) to install the following packages

```bash
npm install express
npm install express-ip
```

## Usage

```JavaScript
// Initialize express web client on a local host, port 3000
node main.js
```

```curl
// Generate hash to insert into an email
curl --insecure -H "Content-type: application/json" 'http://127.0.0.1:3000/generateHash'
```

```
// Periodically send get requests to the following URL to get the mail status
curl --insecure -H "Content-type: application/json" 'http://127.0.0.1:3000/emailBeaconStatus?hash=<YOUR_GENERATED_HASH>'
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)


Here is the repo to the frontend: https://github.com/cszach/email-beacon-frontend
