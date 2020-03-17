# Sparta NodeJS sample app
## Description
This is an implementation of a simple web app made by Sparta Global to test
and practice Devops and testing practices. The repo for the app can be found
here: https://github.com/spartaglobal/node-sample-app

This implementation of the app and accompanying database was provisioned using
Ansible, using Vagrant and Virtual Box.

## Setup
Clone this repo, and make sure that both Vagrant and Virtual Box are both installed
on the host machine. It is not necessary to download Ansible if your machine
is able to, since the app and database provisioning uses Ansible Local.

Open the root directory of the app in the command line. Enter the command
`vagrant up`, and the app and database will be provisioned in separate virtual
machines.

Once the machine setup has finished, access the app by the command
`vagrant ssh app`. This will take you into the app machine for further setup.

Find the app root directory by `cd /home/ubuntu/app` and start the app by the
command `node app.js`. If you want the full functionality of the app, run the
command `node seed/seeds.js` before starting the app.

## Usage
Open a web browser and enter http://developmemt.local:3000 to access the app.
For further extensions, follow the app documentation in the repo given above.
