# Whatsapp Chat Launcher

## Usage

1. Generate a `base64` encoded Whatsapp shortcode using the below code.
```
whatsapp://send/?phone=<Add the phone number here. NO leading 0s>
```

2. Add the following snippet to the `<head></head>` section of the website. 
```html
<script type="text/javascript">
    var phone_number = "<Add the above Base64 encoded value here>";
</script>
<script type="text/javascript" src="./whatsapp.js"></script>
```