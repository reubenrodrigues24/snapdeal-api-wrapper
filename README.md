# snapdeal-api-wrapper
A wrapper for the Snapdeal API in PHP.

For the code to work you will have to create an account at the [Snapdeal API page](https://affiliate.snapdeal.com/affiliate/api/product/feeds/) and request for your affiliate ID. 
Initialize the class with the constrauctor and pass your affiliate ID and token.


    $sd = new Snapdeal("<Affiliate-ID>","Affilaite-Token");
    	
To retrieve the home feed of all categories on Snapdeal use :

    $home = $sd->api_home();
      
To retrieve any other product use the <b>call_url(<Product/Feed URL>)</b> function and pass the URL.

TIP: Use print_r() and pass the values returned by api_home() or call_url(<Product/Feed URL>) to print the array.
