# ZenCart Coinpal Checkout Installation

## Step 1: Log in to the Coinpal Admin Dashboard to get the Merchant Number and Secret Key.
1. [Register](https://portal.coinpal.io/#/admin/register)/[login](https://portal.coinpal.io/#/admin/login) and go to Coinpal's Admin Dashboard 

![](./img/register.png)

2. Follow the Dashboard guidelines to fill in the relevant information
![](./img/kyb.png)
3. Click the 'Integration' button in the lower left corner to get the corresponding Merchant Id and Secret Key
![](./img/api-key.png)

## Step 2: Installing the Coinpal Plugin on your ZenCart Site.
1. Click on the  [Coinpal plugin](https://github.com/CoinpalGroup/plug_ZenCart/blob/master/coinpal.zip) to download Coinpal ZenCart Payment Plug.
2. Unzip the coinpal.zip file and enter the coinpal folder
![](./img/file1.png)

3.  Copy the coinpal_notify.php file to the root directory of the ZenCart project
![](./img/file2.png)

4. Copy the includes\languages\english\modules\payment\coinpal.php file to the ZenCart project includes\languages\english\modules\payment
![](./img/file3.png)

5. Copy all files in includes\modules\payment to ZenCart project includes\modules\payment
![](./img/file4.png)

3. Activate the Coinpal ZenCart Gateway

    Navigate to your ZenCart admin area and follow this path: Modules -> Payment.
    
    Find the payment method named 'Coinpal' and click 'Install Module'.

![](./img/install.png)


Copy and Paste all of the Settings you generated in your Coinpal Dashboard on Step #1.

Click Update Changes.

![](./img/edit.png)


## Step 3: Testing your Coinpal Magento Integration.

To confirm your Integration is properly working create a test order:

Add a test item to your shopping cart and view the cart.

Proceed to Checkout

Select 'Pay Crypto with Coinpal' as the payment method.

Click Continue button
![](./img/checkout.png)

Click Confirm Order button
![](./img/checkout2.png)

If you like you can now proceed to making a test payment.


## Step 4: Marking a Payment as Received on ZenCart.

Login to your ZenCart Admin Dashboard.

Go to the ZenCart Section and Click Orders.

You will see the test orders marked as “Paid”.

Verify the coins are in your chosen Coinpal Wallet (these are the addresses you input during Step #1).

You may also use a Block Explorer to verify if the transaction was processed.

After the verification of the above steps is completed, it means that the connection with Coinpal is successful.





