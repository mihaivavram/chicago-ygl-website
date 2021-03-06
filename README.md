# chicago-ygl-website
Code for the Chicago YGL (Young Government Leaders) Website project is being created in order to empower YGL and provide a sustainable solution for YGL’s needs and capabilities. 

## What is YGL?
Young Government Leaders Chicago is a 501(c)3 organization for young, and young at heart, people involved in government. Whether it is working for federal, state, or local government, part of a public-private partnership, or a non-profit organization in Chicago, YGL is here for all who want to make government better. YGL Chicago strives to make government accessible to everyone.  


## Getting a development environment setup

### Checkout the repo

We make use of the 'open source' fork and pull request style of contribution. To pull a copy of this code in a way that fits within that you'll need to:
1. Fork the repository 
  * This can be done by using the 'fork' button on the top right of this repository page
2. Use git to clone your forked repository to your local machine
  * Example (replace the github url with yours):
    ` git clone https://github.com/Ryan-Koch/chicago-ygl-website `

### Get the containers up and running with wordpress
1. Install the version of Docker that works with your computer's operating system. You can find that [here](https://www.docker.com/products/docker-desktop)
2. Once Docker is installed navigate a terminal session over to you local repository. From there we can use docker-compose to manage the two containers this project uses.
  * To start: ` docker-compose up -d `
  * To stop: ` docker-compose stop `
  * To delete the containers: ` docker-compose rm ` 
3. Navigate to http://localhost:8080 and go through the wordpress setup wizard
4. Choose the understrap theme by going to Appearance > Themes > Understrap > Activate button within Wordpress

### Getting Docker Up on a Windows PC: 
Unless you have Windows Enterprise, or Professional, You'll need to install and Ubuntu Based virtual Environment and Run it from there.
Step 1: Download the Docker Tool Box 
Step 2: Download the latest Version of Ubuntu in an ISO file
Step 3: Install The Tool Box and Oracle VM
Step 4: Open Oracle and Click New
Step 5: Select Type Linux and Ubuntu
Step 6: Add a virtual Hard Disk(The Ubuntu ISO from earlier)
Step 7: Next Until Create
Step 8: From here you can Run Docker Off Your Windows PC

### Get the front end stuff running
1. Install [Node](https://nodejs.org/en/) for access to npm. 
2. Navigate to themes/understrap within your local repository
3. Install gulp cli
  * ` npm install gulp-cli ` or `npm install -g gulp-cli ` for a global install
4. Install Natives
  * `npm install natives@1.1.6`
5. Install the rest of the dependencies
  * `npm install`
6. Start gulp watch
  * `gulp watch`
