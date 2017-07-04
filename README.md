# Scrive GO SDK Documentation

## Introduction

The Scrive GO SDK allows authorized web applications to access Scrive
GO. **Should only be used on internal and non public facing web
applications**.

## Example

An example using the Scrive GO Button, sending a document found at url
`/test.pdf` to Scrive GO. Replace `OAUTH_ID` etc with your credentials.

```html
<!DOCTYPE html>
<html>
<head>
<title>Scrive GO SDK Test</title>
<script src="https://go.scrive.com/sdk.v0.js"></script>
<script>
ScriveGO.init({
  oauth_id: "<OAUTH_ID>",
  oauth_secret: "<OAUTH_SECRET>",
  token_id: "<TOKEN_ID>",
  token_secret: "<TOKEN_SECRET>"
});
ScriveGO.parse();
</script>
</head>
<body>
  <h1>Send test.pdf to Scrive GO</h1>
  <button data-url="/test.pdf" class="scrive-go-button">Scrive GO</button>
</body>
</html>
```

## Initialization

Initialize the SDK with your credentials.

```html
<script src="https://go.scrive.com/sdk.v0.js"></script>
<script>
ScriveGO.init({
  oauth_id: "<OAUTH_ID>",
  oauth_secret: "<OAUTH_SECRET>",
  token_id: "<TOKEN_ID>",
  token_secret: "<TOKEN_SECRET>"
});
ScriveGO.parse();
</script>
```

## Scrive GO Button

The Scrive GO button sends the document in `data-url` to Scrive GO. The
document in `data-url` has to be accesiable using AJAX.

```html
<button data-url="<PATH TO DOCUMENT>" class="scrive-go-button">Scrive GO</button>
```

## Scrive GO Upload

Scrive GO upload prompts the user to upload a document to Scrive GO.

```html
<div class="scrive-go-upload"></div>
```
