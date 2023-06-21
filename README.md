# flutter_paycards

This is a Flutter plugin for [PayCards SDK](https://github.com/faceterteam/PayCards_Source).

## Usage

`import 'package:flutter_paycards/flutter_paycards.dart';`


`Map<dynamic, dynamic> results = await FlutterPaycards.startRecognizer(cancelLabel: 'Cancel');`

**cancelLabel** sets the label for the cancel button on iOS.

The map returned from startRecognizer() will have below key/values:


| Key                | Type    |
| ------------------ |:-------:|
| cardHolderName     | String  |
| cardNumber         | String  |
| redactedCardNumber | String  |
| expiryMonth        | int     |
| expiryYear         | int     |
| cvv                | String  |
| postalCode         | String  |