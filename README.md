# coursera-test1
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Assignment</title>
    <link rel="stylesheet" href="css/styles.css">
</head>

<body>
    <h1>Page Heading</h1>
    <div class="container">
        <section class="box">
            <h2>Chicken</h2>
            <p>Dummy text for the Chicken section.</p>
        </section>
        <section class="box">
            <h2>Beef</h2>
            <p>Dummy text for the Beef section.</p>
        </section>
        <section class="box">
            <h2>Sushi</h2>
            <p>Dummy text for the Sushi section.</p>
        </section>
    </div>
</body>

</html>
/* General Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

h1 {
    text-align: center;
}

.container {
    display: flex;
    flex-wrap: wrap;
}

.box {
    box-sizing: border-box;
    border: 1px solid black;
    padding: 20px;
    margin: 10px;
}

h2 {
    font-size: 125%; /* 25% larger */
    text-align: right;
}

/* Responsive Styling */
/* Desktop View */
@media (min-width: 992px) {
    .box {
        width: 30%; /* Equal width for desktop view */
    }
}

/* Tablet View */
@media (max-width: 991px) and (min-width: 768px) {
    .box {
        width: 48%; /* Equal width for the first two sections */
    }

    .box:nth-child(3) {
        width: 100%; /* Full width for the third section */
    }
}

/* Mobile View */
@media (max-width: 767px) {
    .box {
        width: 100%; /* Full width for mobile view */
    }
}

       

       
