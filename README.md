# Examining forms

## Tools

This uses the following tools and libraries:

  * express
  * express.static
  * [body-parser](https://github.com/expressjs/body-parser)
  * util

## Install

  * `git clone https://github.com/DWDatITP/sample-forms.git`
  * `cd sample-forms`
  * `npm install`
  * `nodemon server.js`
  * visit <http://localhost:5000>
 
## Adding form handling to your app

If you want to add the ability to handle a form to your existing app you need to:

  * Install the `body-parser` module and save it to your package.json:
  * `npm install body-parser --save`
  * [Require the body-parser module in your server.js](https://github.com/DWDatITP/sample-forms/blob/ced1f4d0fba8467d521feff9dba6fe2510959717/server.js#L5)
  * Tell your app to use the body-parser to read incoming requests:
  * `app.use(bodyParser.urlencoded({extended:true}));`
  * Note: This line MUST come before any `app.get` or `app.post` calls.
