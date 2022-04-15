# Inventory Management with Angular and Spring boot 

This is an inventory management system that can be used to track item transactions such as adding new items, selling items, inserting items, etc.

### Images & Videos
* Images of the application can be found in the _images_ folder.
* [Click here](https://drive.google.com/drive/folders/1mZjjC_NEZQTcPBP4auC_BIaGpki-6e7j?usp=sharing) to see the Demo.

### Languages & Tools

* Angular 11
* Angular Material
* Spring Boot 2.4.5
* Spring Boot JPA (Java Persistence API)
* HATEOAS (REST APIs with Hypermedia)
* Mysql 8.0
* Docker + Docker Compose

### Features & Behaviours

* Add Items with basic details such as Item ID, Item Name, Cost, Price, Quantity.
* All the CRUD operations for items such as View items, Add items, Edit items, Delete items.
* Item list and filters - Shows items in a list and filtering them by Item ID, Item Name, etc.
* Sell items - By clicking the "Sell" button, it can be sold for a custom price or the item price itself.
* Insert items - By clicking the "Insert" button, items can be inserted. This can also be used when an item is returned that has already been sold.
* View item history - Shows item transaction details for a selected date.

### Installation (on Ubuntu)

1. Install Docker and Docker Compose (Refer https://docs.docker.com/engine/install/ubuntu/ and https://docs.docker.com/compose/install/).
2. Clone this repo (`git clone https://github.com/mihiran-paranamana/inventory-management-angular-spring-boot.git`).
3. Move into the _inventory-management-angular-spring-boot_ root folder (`cd inventory-management-angular-spring-boot`).
4. Run build script (`sudo bash ./build.sh`).
5. Run the installation script (`sudo bash ./install.sh`).
6. Browse http://localhost:4200/

* With the 4th step, It will create builds for the angular client app (inside _inventory-management-angular-spring-boot/client/dist/client/_) as well as the spring boot server app (inside _inventory-management-angular-spring-boot/server/target/_).
Also, it wll create a separate build folder located in the root folder with all the necessary build artifacts and final zip file (_ims-stable-v0.0.1.zip_).
* With the 5th step, It wil run `sudo docker-compose build` and `sudo docker-compose up -d` commands to build and up the containers.
* If you need to install the application with the final build (_ims-stable-v0.0.1.zip_) that has been generated by the "build.sh" script, first you can copy it into anywhere (even in another computer that has docker installed), then extract it, move to the root folder and run the "install.sh" script.

### Installation (on Windows or Mac)

1. Install Docker Desktop (Refer https://docs.docker.com/docker-for-windows/install/ or https://docs.docker.com/docker-for-mac/install/).
2. Follow the above Ubuntu installation process. With docker, you won't have to do any other OS specific installation steps. Use the docker terminal to run the above commands.

### Enable Dev Mode

* Dev Mode is defined in several places in the code with "Dev Mode Start" and "Dev Mode End" tags.
  This can be enabled by un-commenting the code lines inside those tags for development purposes.

### Contact Details

* Email: mihiran.hlrm@gmail.com
* SkypeId: live:mihiran.hlrm
