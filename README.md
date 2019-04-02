# Daraja C2B - Customer to business STK push - Windows, Linux and Mac

(this is for the people who want to recreate the product and add their own tweaks)
(Provide the url to the package for those who just need to use it.)

If you are here, it means that you need a working solution right away. Well, I will cut to the chase and jump right in.

### *Customer to Business payment story line.*

a. A customer iis buying a service or a product online.

b. You have provided a convinient channel to pay through m-pesa.

c. When the hit "pay", You might ask for their m-pesa enabled phone number, Or have it in advance - Really up to you.

d. Somewhere in your server, Did I say that I like Ubuntu, Maybe I didn't, You get the request and 
    serve an STK notifications on their cell phone (This must have been made for us with feature phones out here)

e. Assuming the customer is not just initiating reqwuests to your server just to play with you,
  They enter their pin and the payment is successful.

f. You get the monies to your paybill account, you honor their request and deliver that bunch of bananas they have been yearning for.

g. (Not part of the story though) The customer is impressed and comes back to your shop again and again. Invites a friend to check you out too.


## Tools

a. .NET core SDK

        ☝️ at the time of writting this blog, the current stable release is .net core is 2.2

b. Visual Studio Code - the editor

c. ngrok - To expose localhost to the internet. One a payment request is made, we need a way to notify our application the status of the payment, wether t'was successful or not.

## Installation and setup

If you already have all the above requirements setup, Skip to ***-----> THE NEXT SECTION HERE***

a. Install [.net core sdk](https://dotnet.microsoft.com/download)

    make sure to install the SDK and not the Runtime __only__. The SDK comes bundled up with the runtime to enable you to test your applications.

b. Download and install [Visual Studio Code](https://code.visualstudio.com/) 

c. Install [C# language extenstion](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp) for visual studio code. This is to enable syntax highlighting and all the goodness of [static typing](https://en.wikipedia.org/wiki/Type_system)


## Steps
1. Create 2 folders, the library and test

        mkdir daraja.library && mkdir daraja.test
2. 
