# Example Gift Card App

Many small businesses have taken a hit due to the COVID-19 outbreak. One way to help support local businesses is purchasing gift cards.

The problem is that many modern POS systems don't either have a straight forward way to sell gift cards online or don't offer such solution at all.

This example application attempts to solve this problem by using Stripe payment solution and GiftUp API to create a easy to use online solution for selling and redeeming gift cards.

## Get Started
1. Sign up on stripe.com and get your company verified to obtain live keys
2. Sign up on giftupapp.com and following the getting started steps e.g. providing stripe keys
3. Obtain site id from https://giftup.app/installation/other
![obtain-site-id](https://user-images.githubusercontent.com/21044999/78466319-1c111700-76bd-11ea-9a3a-ea3c39290a02.png)


## To Run
Download the `gift-card-app` binary and run it like so:
```
 NAME=BUSINESSNAME SITEID=64756a71-b216-4da0-b16a-c8becfcf7a22 APIKEY=your-api-key PORT=3000 ./gift-card-app 
 ```

## Environment Variables
1. Name - Name of your business
2. Site ID - site ID generated by GiftUp
3. Port - port number you wish to run the app on e.g. if you don't provide a PORT number just go to http://localhost:8090
4. API Key - Generate GiftUp API Key from https://giftup.app/integrations/api-keys

## FAQ

### Can this integrate with my POS System
As of now, no. This is designed to be a separate system, and a temporary solution during the COVID-19 crisis.

### Why is this program written in Go?
This application isn't designed to be solution for all businesses, but merely a simple example. Go language was chosen as it outputs a binary executable that is portable and can be run anywhere (no npm, gem, jvm, etc. needed).
