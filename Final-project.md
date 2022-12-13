# Setting up PERN on Fedora

PERN stands for PostgreSQL, Express, React and Node.js. This tutorial will show you how to setup the entire PERN stack on Fedora.

## PERN Installation

PostgreSQL is available to install through dnf:

```
sudo dnf install postgresql postgresql-server
```
![image](https://user-images.githubusercontent.com/49813952/205966825-cf683762-7042-4ff0-b65f-52a17f611f41.png)


## Node.js Installation

Node.js can be insalled like this:

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash
source $HOME/.bashrc
nvm install lts/gallium
nvm alias default lts/gallium
nvm use default
```
![image](https://user-images.githubusercontent.com/49813952/206504033-16f30960-9aea-438a-a18b-24f3046c496c.png)


## Configuration

To start up Node.js and PostgreSQL on system startup, you must do the following:

```
npm install pm2 -g
```
![image](https://user-images.githubusercontent.com/49813952/207390456-a66a6e7c-2caf-44e3-bd47-ae37eaf163bb.png)

```
pm2 start app.js
```
![image](https://user-images.githubusercontent.com/49813952/207397788-c80fdf01-933a-482d-817a-2e4c3c2ecb2a.png)

```
pm2 save
```
![image](https://user-images.githubusercontent.com/49813952/207397897-606d5e39-ed3a-4e55-be82-7ebcc03feca2.png)


## Express

```
$ mkdir myapp
$ cd myapp
$ npm init
```
![image](https://user-images.githubusercontent.com/49813952/207394416-cb19b4f9-f7b4-4d9d-9f03-4a2d94f8cd36.png)

```
npm install express
```
![image](https://user-images.githubusercontent.com/49813952/207394713-c082e614-de87-468b-bba2-dcfbdc911af3.png)

## Video link for this porject
https://youtu.be/QZWt641XGo4

