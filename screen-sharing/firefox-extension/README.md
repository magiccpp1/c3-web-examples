## Firefox extension how to


#### 1) Signup here:

* https://addons.mozilla.org/en-US/firefox/users/register

#### 2) Fix package.json
 - with the name of the extension you prefer,
 - the version of the extension.
 -  generate a unique id. for example from https://www.guidgenerator.com/online-guid-generator.aspx

#### 3) Fix index.js
 - Add domain names you would like this add-on to be supported on. For more information you can take a look at indext.js in the current directoy.

#### 4) Make XPI file from the current directory by:
    ```
    [sudo] npm install jpm --global

        jpm run -b nightly      # test in Firefox Nightly without making the XPI

        jpm xpi                 # it will create xpi file
    ```

#### 5) Submit the XPI here:
    https://addons.mozilla.org/en-US/developers/addon/submit/1
    This add-on needs to be unlisted, therefore reviewing it by Mozila shouldn't take long.



#### More info

  - More information on add-on distribution and signing:
https://developer.mozilla.org/en-US/Add-ons/Distribution