
Synopsis

This website is part 2 of assignment 1 for Red Academy's Web Development Program.
This work was completed in 14 days and involved applying concepts learned over the week, such as html
using css to style, and media queries.


Triumphs



2. Felicity slider installed successfully

3. Subscribe button functioning properly

4. slow scroll working





Code Example
 

 window.onload=function() {
     document.getElementById('formId').onsubmit=function() {
         var input = document.getElementById("your-email").value;
         if( input.length==0){
             alert("Please enter your email")
         }else{
             alert("Thanks for subscribing")
         }

    $('.addToCart').click(function(event) {
        event.preventDefault();
        var name = $(this).attr("data-name");
        var price = Number($(this).attr("data-price"));

        addItemToCart(name, price, 1);
        displayCart();
        totalCart();
    });


    function displayCart() {
        var cartArray = listCart();
        output = ""
        total = ""
        for (var i in cartArray) {
            output += "Your cart has " + cartArray[i].count + " unit(s) of " +
                    cartArray[i].name + " @" + cartArray[i].price + " each" + "...and..." + ""

        }
        console.log(output)
    }

This is a mobile first project and as such makes use of media queries:

@media all and (min-width:600px)  {
}

The project made use of font-face:

@font-face {
    font-family: "playfair_displayregular"; /*a name to be used later*/
    url("assets/fonts/playfairdisplay-regular-webfont.otf"); /*URL to font*/
}

The project makes use of combined inages and background grandients:

.hero-banner {

    background: linear-gradient( to bottom, rgba(0,0,0,0.25) 0%, rgba(0,0,0,0.25) 100%),
    url("assets/images/banner-girl.png") no-repeat center,
    url("assets/images/flower-bkgd.jpg");




 

The website is designed to quickly establish our html and css coding skills. Part two
incorporates jquery and javascript.




Installation
 

The site can be viewed at GitHub @ :https://github.com/macbrett?tab=repositories

This was an individual project with plenty of contributions from classmates and teachers.



