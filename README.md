# Video Doorbell, Lab 7


## Part A. HelloYou from the Raspberry Pi

**a. Link to a video of your HelloYou sketch running.**

[HelloYou](https://github.com/popeil97/IDD-Fa19-Lab7/blob/master/HelloYou.MOV)

## Part B. Web Camera

**a. Compare `helloYou/server.js` and `IDD-Fa18-Lab7/pictureServer.js`. What elements had to be added or changed to enable the web camera? (Hint: It might be good to know that there is a UNIX command called `diff` that compares files.)**

The general server setup remains similar on both servers, including most socket communication lines and arduino commincation functionality. However, pictureServer.js has a few extra event handlers for handling the takePicture button from the client. There is also an instantiation of the Node web camera module.

**b. Include a video of your working video doorbell**

[VideoDoorbell](https://github.com/popeil97/IDD-Fa19-Lab7/blob/master/VideoDoorbell.MOV)

## Part C. Make it your own

**a. Find, install, and try out a node-based library and try to incorporate into your lab. Document your successes and failures (totally okay!) for your writeup. This will help others in class figure out cool new tools and capabilities.**

I used the nodemailer module that leverages Sendgrid to send emails via javascript server side code. Whenever the user pressed the arduino button(doorbell), the nodemailer accesses the picture through the rasperry pie file system and makes a POST request to send the picture and message to the designated email account.

**b. Upload a video of your working modified project**

[My Video Doorbell](https://youtu.be/sNa52PhXh5Y)
