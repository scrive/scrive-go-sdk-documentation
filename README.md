# Scrive GO SDK Documentation

## Introduction

The Scrive GO SDK allows authorized web applications to access Scrive
GO.

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

The Scrive GO button sends the document in `data-url` to Scrive GO.

```html
<button data-url="<PATH TO DOCUMENT>" class="scrive-go-button">Scrive GO</button>
```

## Scrive GO Upload

Scrive GO upload prompts the user to upload a document to Scrive GO.

```html
<div class="scrive-go-upload"></div>
```
