iso4217.js
=======

A javascript object used to reference ISO 4217 currency codes. Fair warning, atm this requires Twitter Bootstrap and jQuery.

#### Example Use
    iso4217.all().init( 'EUR', 20 );
This initialized all possible currrency codes, and set the default currency code to 'EUR' with a value of 20.

    iso4217.only(['EUR', 'USD', 'CNY', 'BHD']).init('USD', 12 );
This initialized only 'EUR', 'USD', 'CNY', and 'BHD'. 'USD' is the default with a value of 12.

    iso4217.omit(['AED', 'UGX']).init('CNY', 55, '#dropdownMenu', '#dropdownToggle', '#inputText');
This initialized all currency codes *except* 'AED' and 'UGX'. 'CNY' is the default with a value of 20. The element with id 'dropdownMenu' is the ul element to append the list of currency codes; the element with id 'dropdownToggle' is the button the user will use to select currency codes; the element with id 'inputText' is the text input to display the value of 55.
