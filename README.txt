we have downloaded this conFusion folder from resourses and then

here there is index.html and package.json file already here, so we just need to install the packages
    installed in package.json file by typing
        npm install
create a .gitignore file and add node_modules in there and do a git commit

=====================================================================================================
Fetching bootstrap

(note: the lite server is already setup for this exercise in the downloaded resourses, but we need to 
explicitely configure that if we want to use that)

    to install bootstrap type
        npm install bootstrap --save

    but, to use bootstrap we need to install its peers manually which are jquery and popper.json
        npm install jquery popper.js --save

    now start the lite server by npm start and start working

    (note: in node_modules, there is a folder named bootstrap in there and in there we have css and js 
    folder which contains the files that we needed to use bootstrap in our application, we will also
    require the specific bootstrap files in order to use bootstrap later)

    now we will be creating meta tags and link the bootstrap files in the node_modules folder 
        here, we have copy and pasted the code snipits of these tags from the resourses in the head of 
        index.html file     

                <!-- Required meta tags always come first -->
                    <meta charset="utf-8">
                    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
                    <meta http-equiv="x-ua-compatible" content="ie=edge">

                <!-- Bootstrap CSS -->
                    <link rel="stylesheet" href="node_modules/bootstrap/dist/css/bootstrap.min.css">

    now, we need to add jquery, popper.js and js file to index.html as well, 
        note: we will add all these in the body, just before the </body> closing tag of body
        and the code is in the resourses
            <!-- jQuery first, then Popper.js, then Bootstrap JS. -->
                    <script src="node_modules/jquery/dist/jquery.slim.min.js"></script>
                    <script src="node_modules/popper.js/dist/umd/popper.min.js"></script>
                    <script src="node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
            (note: include them in the same sequence as provided)                
        
    and now as we save the changes, the normal font will be changed to the bootstrap default font
    
=====================================================================================================
Responsive Design And Bootstrap Grid

    added .container to index.html and doing changes in index.html file

    to add custom css just create a folder in the root directory named css and then in that folder
        add a file named style.css 