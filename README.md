# <!DOCTYPE html>
<html>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<head>
    <title>Navbar Dropdown Menu</title>
</head>

<style>
    ul {
        font-family: Arial, Helvetica, sans-serif;
        list-style-type: none;
        margin: 0;
        padding: 0;
        width: 200px;
        background-color: orange; 
        border-radius: 5px;
    }

    li a {
        display: block;
        color: white;
        padding: 8px 16px;
        text-decoration: none;
    }

    
    li a:hover {
        background-color: lightblue;
        color: black;
    }

    .dropbtn {
        min-width: 168px;

    }

    .dropdown {
        position: relative;
        display: inline-block;
        border-bottom: 1 solid gray;
    }

    .dropdown-content {
        display: none;
        position: absolute;
        background-color: rgb(28, 27, 26);
        min-width: 200px;
        box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
        z-index: 1;
        top: 15%;
        left: 101%;
        border-radius: 5px;
    }



    .dropdown-content a {
        color: white;
        padding: 12px 16px;
        text-decoration: none;
        display: block;
    }

    .dropdown-content a:hover {
        background-color: lightblue;
    }

    .dropdown:hover .dropdown-content {
        display: block;
    }

    .dropdown:hover .dropbtn {
        background-color: lightblue;
    }

    .dropdown-content-sub {
        display: none;
        position: absolute;
        top: 0;
        left: 101%;
        min-width: 200px;
        background-color: rgb(28, 26, 26);
        border-radius: 5px;
    }

    .dropdown-content:hover .dropdown-content-sub {
        display: block;
    }

    .dropdown-content a,
    .dropdown-content-sub a {
        color: white;
        padding: 12px 16px;
        text-decoration: none;
        display: block;
    }

    .dropdown-content a:hover,
    .dropdown-content-sub a:hover {
        background-color: lightblue;
    }
</style>

<body>
    <h1>Navbar _Act 3 _Angelo B. Del Carmen_ BSCS 2A</h1>
    <ul>
        <li><a href="default.asp">HOME</a></li>
        <li class="dropdown">
            <a class="dropbtn">PRODUCTS
                <i class="fa fa-caret-right"></i>
            </a>
            <div class="dropdown-content">
                <a class="a1" href="#">PRODUCT 1
                    <i class="fa fa-caret-right"></i>
                </a>
                <div class="dropdown-content-sub">
                    <a href="#">SUB PRODUCT 1</a>
                    <a href="#">SUB PRODUCT 2</a>
                </div>
                <a class="a2" href="#">PRODUCT 2
                    <i class="fa fa-caret-right"></i>
                </a>
            </div>
        </li>
        <li><a href="contact.asp">ABOUT</a></li>
        <li><a href="about.asp">CONTACT</a></li>
    </ul>
</body>

</html>
