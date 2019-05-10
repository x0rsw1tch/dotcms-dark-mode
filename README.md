# dotcms-dark-mode

Dark stylesheet for dotCMS back-end


## how to use

Use the Chrome extension "Stylus" to add your stylesheets, and use the following RegEx pattern for host matching, changing the hostname as needed:

```
  HTTP or                                Optional                              Back-end
   HTTPS                Host FQDN          Port                                  URIs
     |                      |               |                                     |
 ---------         -------------------- ---------    --------------------------------------------------------
 |       |         |                  | |       |    |                                                      | 
(http)+s*(\:\/\/)+(WWW\.HOSTNAME\.COM)+(\:8080)*(\/)+(dotAdmin\/|c\/|.*\?leftMenu|html\/portal|.*\?mainFrame)+.*
```

### For styling the log window

Add a separate styleshet entry with the following CSS (feel free to change the colors, font, etc as you sdee fit)

```
html {
    color: #ccc;
    background-color: #090909;
}

.tailerBody {
    font-size: 16px;
}
```

RegEx Pattern: `.*\/dotTailLogServlet\/.*`
