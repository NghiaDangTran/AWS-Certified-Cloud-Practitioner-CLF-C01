
# IAM Identity and Access Management

 * is a `global service`
 * `root` account `created by default`, `shouldn't` be `used` or share
 * u can set orther as `User`, and Put then in `Group`
 * `Group` only have `User`, `not` orther `group`, but `one` user can have `mutiple group`
# Permission,
 * use a `JSON` file to asign what `service` `user` or `group` can `do`
 * should apply `Least Previlege Principle` dont `give to much permission`
 * `inline` policy is where u write the `custom policy`
# IAM Policies Structure
 - `version`: policy language version
 - `id`: optional
 - `statement`: on or more indicidual statements requred (optional)
 - `sid`: staement id
 - `effect`: `Allow` or `Deny`
 -  `prinipal`: `account/user/role` for the effect
 -  `action`: list of action for effect
 -  `resource` list of resource to which the action applied
 -  `condition`: if else (optional)

# IAM Password Policy
 - set length
 - require special char
 - allow user to change their own password
 - password expiration time
 - prevent passwrod reuse
 


 
 
## but MFA is a must
 - you want to `protect` atleast ur `root account and IAM User`
 - `MFA= Password u have + security device`
 - > is u got hack or password stolen, account is still ok
 - support virtual MFA or U2F or Hardware key, 
 # IAM Roles
 - connect AWS service together
 
 # IAM Security Tools (Audit)
**IAM Credential Report (account level):**

-   Provides status of user's AWS credentials like when iam account reacte  paswweord 
-   Helps audit user activity for security.

**IAM Access Advisor(User-level) :**
-   Shows when and what services an IAM user, group, or role has accessed.
-   Helps remove unnecessary access to follow the principle of least privilege.
- 

# IAM Guidelines & Best Practices 

* Don't use the root account except for AWS account setup 
* One physical user = One AWS user 
* `Assign users to groups` and `assign permissions to groups `
* Create a` strong password policy `
* Use and enforce the use of `Multi Factor Authentication (MFA) `
* Create and use `Roles` for giving permissions to AWS services 
* Use Access Keys for Programmatic Access (CLI / SDK) 
* Audit permissions of your account using IAM Credentials Report & IAM Access Advisor 
* `Never share IAM users and Acess Keys`

# Shared Responsibility Model for Iam
- Aws:
    * infrastruture (global network security)
    * configuration and vulnerability analysis
    * compliance validataion
 - User
    - User, gorup, polices management and monitoring
    - Enable MFA on all account
    - rotate all ur keys offten
    - User IAM tools to apply approriate premissinons
    - Analyze access patterns and review perimison
# Extra infor 
 - If a policy explicitly denies an action, it's denied even if another policy allows it.
 - If there's no policy for an action, it's implicitly denied.
 - Explicit allow overrides the default implicit deny


# How MFA work 
```


# How MFA work 
`
const speakeasy = require('speakeasy');
const QRCode = require('qrcode');

// Generate a secret key for the user.
const secret = speakeasy.generateSecret({length: 20, name: 'MyApp:User123'});
console.log('Secret:', secret.base32);  // You'd typically save this in your database.

// Generate a QR code for the user to scan using their authenticator app.
QRCode.toDataURL(secret.otpauth_url, function(err, data_url) {
  console.log('QR Code:', data_url);  // Show this to the user.
});

// Later, when the user logs in, they provide a token from their authenticator app.
let userToken = '123456';  // You'd typically get this from a login form.

// Verify the token against the secret.
let verified = speakeasy.totp.verify({ 
  secret: secret.base32,
  encoding: 'base32',
  token: userToken
});

if (verified) {
  console.log('User is authenticated.');
} else {
  console.log('User failed to authenticate.');
}

`
```
