# Paytron-Inline
This is the documentation for using Paytron payment gateway inline.

Add this to your html
```
https://paytron.com.ng/assets/js/iframe.paytron.js
```

Then in your codes
```
  PaytronModal.showModal({
    email: 'akinjiolatoni@gmail.com',
    company: 'Pawa',
    description: 'AEDC Abuja',
    recipientAccountNumber: '1234567890',
    firstname: 'Abiola',
    lastname: 'Funmbi',
    recipientBankCode: '058',
    amount: '300,
    companyLogo: 'https://yourwebsite.com/logo.png'
  }).setCallback(function(e) {
    if (e.code === Paytron.SUCCESS) {
      //perform a success action or redirect to success page
    } else if (e.code === Paytron.FAILURE) {
      //perform a failure action or redirect to failure page
    }
  });
```


