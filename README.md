# Housing Selection App Missouri Valley College
![Screenshot1](https://github.com/alrefaeomar/seb_test_2/blob/master/Screenshots/Screenshot%2001.jpg)

## Table of Contents
* [Introduction](#introduction) 
* [Technologies Used](#technologies-used)
* [Instructions](#instructions)
  * [Prequisites](#prequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Technical Documentation](#technical-documentation)
* [Acknowledgements](#acknowledgements)


## Introduction
Since we are facing a pandemic right now, the need of a contactless measurement is a must. Thus, a good measurement for this is to have a Web application where Students can apply their housing. 

## Technologies Used
* HTML
* CSS
* Javascript
* C#
* SQL Server
* Bootstrap


## Instructions

### Installation
The first action needed to use this application is to clone it, by using:
```
$ git clone https://github.com/alrefaeomar/seb_test_2
```

Then, Visual Studio (preferably Visual Studio 2017) will be needed in order to modify or alter the components inside the application, such as the Controllers, Layout, etc.


## Usage
The students will be able to login with their ID numbers and password or PIN in order to login and continue the process of housing selection. It is as easy as the user input his or her ID with the password or PIN and click on the login button to continue the proccess. If the user needs instructions to keep up with the process there is a instructions button that display a modal with all the information, depending on which part of the process the user is.
## Technical Documentation
Most of the Front - End development was created using Bootstrap 4.6.0. All of the pages include the Flex box properties as wee can see:
```
class="d-flex flex-lg-row  flex-md-column  flex-sm-column flex-xs-column m-10 justify-content-center align-content-center"
```
The presented code would create the flex, and the childs inside it would be others components of the website, such as, forms, images, buttons, etc. The childs wil be set to **col** as we can see:
```
class="col justify-content-center align-content-center"
```

Then, the modals used to display instructions in the different pages were also created with Bootstrap, where at first we need create a button with the toggler, so eveytime we click on the button the model will display. 

Also, Font Awesome icons were imported in the **Layout.cshtml** ``<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css" integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />``

Therefore, in the following piece of code we can see the toggler, the target modal and then the **<i><i/>** where a Font Awesome is imported.
```
<button data-toggle="modal" data-target="#Instructions-modal" class="btn btn-primary mr-4 mb-4">Instructions<i class="fas text-center ml-3 fa-angle-up"></i></button>
```
 
Moving on with the Modal Body, we can see that the **id="Instructions-modal"** is the data target that we set on the modal button, so the modal can be triggered after the button is clicked. 

Thus, the rest of the code would be the divs for each of the components of the modal, such as, headers, titles, body, buttons, etc.
```
<div class="modal fade in" id="Instructions-modal" tabindex="-1">
                    <div class="modal-dialog">
                        <div class="modal-content">
                            <div class="modal-header">
                                <h5 class="modal-title">Instructions</h5>
                                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                    <span aria-hidden="true">&times;</span>
                                </button>
                            </div>
                            <div class="modal-body">
                                <p class="text-justify">If you have used this system before, you can log-in with your ID number and the password you have previously created for this portal. If you are a new user, please enter your MVC ID Number check the reCaptcha box/Challenge and click on [New User / Forgot Password]. The system will walk you through the new user/forgot password process afterwards.</p>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-Exit" data-dismiss="modal">Close</button>
                            </div>
                        </div>
                    </div>
                </div>
```


## Acknowledgements

* [Font-Awesome](https://fontawesome.com/)
* [W3Schools](https://www.w3schools.com/)
* [Bootstrap](https://getbootstrap.com/)
* [Missouri Valley College](https://www.moval.edu/)

