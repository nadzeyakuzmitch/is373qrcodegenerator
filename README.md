# Nadzeya Kuzmitch IS373 QR Code Generator
## Basic description

This code is for generating QR codes with the parameters specified in the docker-compose.yml or from the users input.

## My GitHub Homepage QR Code

My GitHub Homepage QR:

![alt text](https://github.com/nadzeyakuzmitch/is373qrcodegenerator/blob/master/nadzeyakuzm-github.png?raw=true)

Before I have placed QR, there was this example:

![alt text](https://media-cldnry.s-nbcnews.com/image/upload/t_fit-760w,f_auto,q_auto:best/rockcms/2022-08/220805-domestic-cat-mjf-1540-382ba2.jpg)

## Build the image and run

1. docker build -t nadzeyakuzm/is373qrcodegenerator . <- builds image called "nadzeyakuzm/is373qrcodegenerator" which we can later run in container
   
2. docker run -e QR_CODE_DEFAULT_URL=https://github.com/nadzeyakuzmitch/ -e QR_CODE_IMAGE_DIRECTORY=qrcodes -v $(pwd):/home/ nadzeyakuzm/is373qrcodegenerator <- run the image we have created with parameters you specify to generate QR code