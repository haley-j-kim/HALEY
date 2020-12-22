# HALEY
const axios = require('axios')
const qs = require('querystring')

...

const requestBody = {
  name: 'Akexorcist',
  age: '28',
  position: 'Android Developer',
  description: 'birthdate=25-12-1989&favourite=coding%20coding%20and%20coding&company=Nextzy%20Technologies&website=http://www.akexorcist.com/',
  awesome: true
}

const config = {
  headers: {
    'Content-Type': 'application/x-www-form-urlencoded'
  }
}

axios.post(url, qs.stringify(requestBody), config)
  .then((result) => {
    // Do somthing
  })
  .catch((err) => {
    // Do somthing
  })
