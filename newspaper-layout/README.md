In this lab, you will design a newspaper layout using CSS Grid, including concepts like grid rows and grid columns.

Objective: Fulfill the user stories below and get all the tests to pass to complete the lab.

User Stories:

    Your page should contain a main element with the class newspaper-layout.
    The .newspaper-layout should include a header with the class title containing an h1 to display the newspaper's name.
    The .newspaper-layout should include an article with the class feature-article for the main news article.
    The .feature-article should include an h2 element for the article title followed by a p element for the article content.
    You should add three more article elements for smaller articles, with classes small-article1, small-article2, and small-article3.
    Each of the smaller articles should include an h3 element for the article title followed by a p element for the article content.
    The .newspaper-layout should include an article element with the class secondary-article for an additional news section.
    The .secondary-article should include an h2 element for the article title followed by a p element for the article content.
    The .newspaper-layout should include a figure with the class cover-image to display an image that represents the newspaper's content.
    The elements with the classes title, feature-article, secondary-article, cover-image, small-article1, small-article2, and small-article3 should have a grid-area property set to the same class name.
    Your .newspaper-layout should use CSS Grid with a grid-template-areas property to define the arrangement of sections:
        The .title should span across the top row.
        The .feature-article should span two columns in the second row, with the .cover-image in the third column.
        The .secondary-article should span two columns in the third row, with the .cover-image in the third column.
        The three small articles should appear in the fourth row.
    The .newspaper-layout should have a grid-template-columns property that divides the space into three equal columns.
    You should set the .newspaper-layout's grid-template-rows property to auto for the first row and divide the remaining space into equal parts for the other rows.
    You should add a gap between grid items.
    Ensure that the image inside .cover-image fits within the designated space by setting its max-width to 100%.

Note: Be sure to link your stylesheet in your HTML and apply your CSS.

Failed: 12. The display property of the .newspaper-layout element should be set to grid.
Failed: 13. Your .newspaper-layout element should have a grid-template-areas property with title spanning all three columns of the first row.
Failed: 14. The second row of the grid template should contain a feature-article spanning two columns and a cover-image.
Failed: 15. The third row of the grid template should contain a secondary-article spanning two columns and a cover-image.
Failed: 16. The fourth row of the grid template should contain small-article1, small-article2, and small-article3.
Failed: 17. Your .newspaper-layout selector should use the grid-template-columns property to divide the space into three equal parts. Remember you can use either the repeat function or manually define each fractional unit.
Failed: 18. Your .newspaper-layout selector should have a grid-template-rows property set to auto 1fr 1fr 1fr.
Failed: 19. You should add a gap between grid items.
Failed: 20. .title should have a grid-area of title.
Failed: 21. .feature-article should have a grid-area of feature-article.
Failed: 22. .cover-image should have a grid-area of cover-image.
Failed: 23. .secondary-article should have a grid-area of secondary-article.
Failed: 24. .small-article1 should have a grid-area of small-article1.
Failed: 25. .small-article2 should have a grid-area of small-article2.
Failed: 26. .small-article3 should have a grid-area of small-article3.
Failed: 27. The img inside .cover-image should have a max-width of 100%.
