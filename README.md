To start the app

`./gradlew run --args=https://fhcacc.icure.cloud/ws`

Once the app started you get the keystore id on the stdout.

You can use the keystore id in the command below:

`curl -X GET "https://fhcacc.icure.cloud/sts/token?ssin=74010414733" -H "accept: */*" -H "X-FHC-keystoreId: 0f775280-7795-426d-961a-9a4483b2e787"`

that returns the token:


```{"tokenId":"83716024-568e-45a1-8b43-e094ef5db472","token":"<?xml version=\"1.0\" encoding=\"UTF-8\"?>...","timestamp":1639584028731,"validity":1639670442417,"quality":"doctor"```
