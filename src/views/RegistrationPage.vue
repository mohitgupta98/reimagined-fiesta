<template>
  <div class="center">
      <div class="container">
        <h1>Help us know you better!</h1>
        <hr />
        <div>
        <input type="text" placeholder="Business Name*" v-model="businessName" required/>
        <br>
        <input type="text" placeholder="Business Category*" v-model="firstName" required/>
        <br>
        <input type="text" placeholder="Business Description*" v-model="lastName" required/>
        <br>
        <input type="text" placeholder="Email ID*" v-model="mobileNumber" required/>
        <br>
        </div>
        <hr />
        <button class="registerbtn" @click = "registerUser">Register</button>
      </div>
  </div>
</template>

<script>
// import firebase from 'firebase'
// import router from '../router'
// import api from '../config/api'
// import { setCookie } from '../utils/utils'
// import axios from 'axios'

export default {
  name: 'Register'
  // data: () => {
  //   return {
  //     businessName: '',
  //     firstName: '',
  //     lastName: '',
  //     address: '',
  //     mobileNumber: '',
  //     gstNumber: ''
  //   }
  // },
  // methods: {
  //   registerUser () {
  //     const data = {
  //       firebaseMerchantId: this.user.uid,
  //       businessName: this.businessName,
  //       firstName: this.firstName,
  //       lastName: this.lastName,
  //       address: this.address,
  //       mobileNumber: this.mobileNumber,
  //       gstNumber: this.gstNumber
  //     }
  //     if (this.firstName && this.lastName && this.businessName && this.gstNumber && this.address && this.mobileNumber) {
  //       axios.post('http://10.177.68.22:9002' + '/merchants/add', data, {
  //         headers: {
  //           'Content-Type': 'application/json',
  //           Accept: 'application/json'
  //         }
  //       })
  //         .then(data => {
  //           setCookie('merchantId', data.data.merchantId, 100)
  //           router.push('/profile')
  //         })
  //         .catch((error) => {
  //           console.error('Error:', error)
  //         })
  //     }
  //   }
  // },
  // created () {
  //   firebase.auth().onAuthStateChanged(user => {
  //     if (user) {
  //       this.user = user
  //       console.log(user.uid)
  //       fetch(api.BackendBasepath + '/merchants/getMerchantDetailsByFirebaseMerchantId/' + user.uid)
  //         .then(response => response.json())
  //         .then(response => {
  //           console.log(response)
  //           if (response.merchantId) {
  //             setCookie('merchantId', response.merchantId, 100)
  //             router.push('/profile')
  //           }
  //         })
  //     } else {
  //       router.push('/login')
  //     }
  //   })
  // }
}
</script>

<style lang='scss'>
#heading {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 37px;
  color: #000000;
}
.container {
  padding: 16px;
  input[type=text], input[type=password], input[type=number] {
    width: 400px;
    padding: 15px;
    margin: 5px 0 22px 0;
    display: inline-block;
    border: none;
    background: #f1f1f1;
    content: "\A";
    border-radius: 9px;
  }
  input[type=text]:focus, input[type=password]:focus, input[type=number]:focus {
    background-color: #ddd;
    outline: none;
  }
}

/* Overwrite default styles of hr */
hr {
  width: 500px;
  border: 1px solid #f1f1f1;
  margin-bottom: 25px;
}

/* Set a style for the submit/register button */
.registerbtn {
  background-color: #405C58;
  color: white;
  padding: 16px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 350px;
  opacity: 0.9;
  border-radius: 9px;

}

.registerbtn:hover {
  opacity:1;
}

/* Set a grey background color and center the text of the "sign in" section */
.signin {
  background-color: #f1f1f1;
  text-align: center;
}
</style>
