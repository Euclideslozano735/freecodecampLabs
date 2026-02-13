<!-- You should have a div element with a class of blog-post-card to hold all of your card elements.
Within the .blog-post-card element, you should have an image element with a valid alt attribute and text, and a class of post-img. You can use https://cdn.freecodecamp.org/curriculum/labs/cover-photo.jpg for the src attribute of the image.
You should have a div with a class of post-content within the .blog-post-card element with the following:
An h2 element with a class of post-title and text for the title of your blog post.
A p element with a class of post-excerpt and text to summarize your blog post.
An a element with a class of read-more with the text Read More. -->

You should apply the following styles to the .blog-post-card element:
A white background.
Rounded corners.
A width of your choice.
The text alignment of your choice.
The .post-img element should be styled so that the image fills the card's entire width and has a bottom border.
The .post-content element should be styled so that there is padding inside the card.
The .post-title and .post-excerpt elements should have a text color other than the default and margins on all sides.
The .read-more element should be styled like a button and have:
A text color other than the default.
A background color.
Margins on all sides.
Padding on all sides.
Rounded corners.
A display property set to inline-block.
A hover effect that changes its background color.
Note: Be sure to link your stylesheet in your HTML and apply your CSS.

body{
background-color: rgb(206, 206, 189);
font-family: Arial, sans-serif;
}
.blog-post-card{
background-color: white;
border-radius: 10px;
width: 350px;
margin: 125px auto;
text-align: center;
}
.post-img{
border-radius: 5px;
border-bottom: 4px solid rgba(0, 0, 0, 0.587);
width: 100%;
}
.post-content{
padding: 5px;
width: 80%;
text-align: center;
margin-left: auto;
margin-right: auto;
}
.read-more{
color: white;
background-color: rgba(37, 35, 35, 0.868);
margin-top: 3px;
margin-left: 10px;
margin-right: 10px;
margin-bottom: 30px;
display: inline-block;
border-radius: 4px;
padding: 10px;
text-align: center;
}
.read-more:hover{
background-color: orange;
}
.post-title{
margin: 4px;
color: rgba(0, 0, 0, 0.861);
}

.post-excerpt{
margin-bottom: 20px;
margin-top: 10px;
color: rgba(0, 0, 0, 0.799);
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="styles.css" rel="stylesheet"/>
    <title>Blog Post Card</title>
</head>
<body>
    <div class="container">
    <div class="blog-post-card">
    <img class="post-img" src="https://cdn.freecodecamp.org/curriculum/labs/cover-photo.jpg" alt="image d'un écran d'ordinateur">
    <div class="post-content">
    <h2 class="post-title">Learn Web Development in 2024</h2>
    <p class="post-excerpt">Stay ahead of the curve with the latest trends in web development. Discover what's new and exciting in 2024</p>
    <a class="read-more">Read More</a>
</div>
</body>
</html>
