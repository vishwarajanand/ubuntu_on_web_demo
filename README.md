# Ubuntu On Web Demo
This repository how we can build an entrypoint to another system powered by React.
Disclaimer, I forked and copied from [https://vivek9patel.github.io/](https://vivek9patel.github.io/).

And upon checking the source and flow, I can foresee following issues while scaling this system:

1. We need a server to maintain the browsing context. Currently, browsing experience is being mimic'ed in UI and the files are actually limited to the github repo. This limits the system to support only few applications provided out of the box.

2. Ideally the system can be linked to a VM with some auth in front and only parts of the OS can be exposed, say terminal or file browser! It can then serve as a handy tool to connect across multiple VMs or PODs.

# To run this on localhost

- Make _.env_ file in root folder

### Get API keys from emailjs

- Get your apis from [emailjs](https://www.emailjs.com/).
  follow this [docs](https://www.emailjs.com/docs)
- inside that file you need to declare your api keys for _emailjs_, below is the sample code
- your api keys will be here: [page](https://dashboard.emailjs.com/admin/integration)
<!-- to get google analytics tracking id -->

### Get Tracking ID from google analytics

- follow this [docs](https://support.google.com/analytics/answer/10269537?ref_topic=1009620) to get your Tracking ID
- add your keys to .env file just like below given template.

```
REACT_APP_TRACKING_ID = "GOOGLE_ANALYTICS_TRACKING_ID"
REACT_APP_USER_ID = 'YOUR_EMAILJS_USER_ID'
REACT_APP_TEMPLATE_ID = 'YOUR_EMAILJS_TEMPLATE_ID'
REACT_APP_SERVICE_ID = 'YOUR_EMAILJS_SERVICE_ID'
```

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributiors who wants to make this website better can make contribution,which will be **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Added some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
