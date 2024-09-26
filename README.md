# Whatsapp Chat Launcher

## Usage

1. Generate a `base64` encoded Whatsapp shortcode using the below code.
```
whatsapp://send/?phone=<Add the phone number here. NO leading 0s>
```

2. Add the following snippet to the `<head></head>` section of the website. 
```html
    <script type="text/javascript" src="https://cdn.jsdelivr.net/gh/praveenprem/whatsapp-chat-launcher@latest/whatsapp.js"></script>
    <script type="text/javascript">
        var phone_number = "<Add the above Base64 encoded value here>";
        document.addEventListener("DOMContentLoaded", function(event) {
                load_whatsapp_plugin();
        });
    </script>
```

### Example
```html
<!DOCTYPE html>
<html lang="en">

    <head>
        <title>My Store</title>
        <script type="text/javascript"
            src="https://cdn.jsdelivr.net/gh/praveenprem/whatsapp-chat-launcher@latest/whatsapp.js"></script>
        <script type="text/javascript">
            var phone_number = "d2hhdHNhcHA6Ly9zZW5kLz9waG9uZT00NDAwMDAwMDAw";
            document.addEventListener("DOMContentLoaded", function (event) {
                load_whatsapp_plugin();
            });
        </script>
    </head>

    <body>
    </body>
</html>
```