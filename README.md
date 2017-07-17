# AngularSocial

Install
```

  npm i --save ngx-facebook `https://zyra.github.io/ngx-facebook/`
```

include scripts to index page
```

<script type="text/javascript" src="https://connect.facebook.net/en_US/sdk.js"></script>
<script src="https://apis.google.com/js/platform.js" async defer></script>
```


**Settings environment**
```
socialAuth: {
    facebook: {
      appId: string,
      xfbml: boolean,
      version: string
    },
    linkedin: {
      apiKey: string,
      authorize: boolean,
      isServer: boolean
    },
    google: {
      client_id: string,
      cookiepolicy: string,
      scope: string
    }
  }
```

**Facebook:**
<br>
```
loginWithFacebook():

return {
  authResponse: {
    accessToken: string,
    expiresIn: number,
    grantedScopes: string,
    signedRequest: string,
    userID: string
  }
  status: string
}
```
```
getProfile():

return {
  id: string,
  name: string
}
```

**Linkedin:**
```
loginLD():

return {
  emailAddress: string,
  firstName: string,
  lastName: string
  id: string
}
```

**Google:**
create button with id googleBtn
```
attachSignin()

return {
  token: string,
  ID: string,
  Name: string,
  Image URL: string,
  Email: string
}

```
