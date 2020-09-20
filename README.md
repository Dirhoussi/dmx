<h2>Bodyo Lighting</h2>
<h3>Light architecture within the pod</h1>
<a href="http://www.inbca.com/en/in-c01">Face recognition system with infrared thermometer </a>
<p>This device is like a mobile its operating system is android,it contains an application that can detect body temperature using infrared thermal camera, body temperature alarm, mask recognition, stranger/visitor recognition, face recognition, personnel identity information procurement, attendance and visitor.In this project i am just focusing on getting temperature from the device using requests in typescript.</p> 
<h2><strong>Repository Contents and Documentation</strong></h2>
<br>
<ul>
<li> <strong> ./ThermalCamera_IN-CO1-D : </strong>Example code of testing the api of the thermal camera using typescript.you find in the ./src
   3 files.ts and a folder including  examples of device`s response for debugging </li><br>
<li><strong>./src/DeviceRestart.ts : </strong> it contains a function that return a promise informs you that the device is restarting successfully.you can see the example of answer of the device about this request in this path ./src/device_response/DeviceRestart.txt.for more details about the request look the page 20 of the documentation</li>
<li><strong>./src/GetDeviceMac.ts : </strong> it contains a function that return a promise with the address Mac of the thermal camera.you can see the example of answer of the device to this request in this path ./src/device_response/GetDeviceMac.txt.for more details about the request look the page 15 of the documentation</li>
<li><strong>./src/Recordacquisition.ts : </strong> it contains a function return a promise with data temperature of the user.you can see the example of answer of the device to this request in this path ./src/device_response/Recordacquisition.txt. <strong>the logic of this function must be respected to get the right measurement of the user.</strong>this logic let time to the user to take the right position with the camera.for more details about the request look the page 13 of the documentation</li>
<li><strong>.env</strong> you find here the address of the device.when we connect the camera in a new network we have to change the address in .env .The thermal camera takes a static address in a new network</li>
</ul>
<br>
  
<a href="https://drive.google.com/file/d/1t-7U21KBLVW9WG8iMd1zpm2RnKM7H2_w/view?usp=sharing" target="_blank"><strong>Documentation<strong></a>
<h2><strong>Developing</strong></h2>
<br>
   
<ol>
<li>Install Node.js on this link <a href="https://nodejs.org/en/" target="_blank" >Node.js</a></li> 
<li>Clone this repo</li>
  <code>git clone https://github.com/Matrix-SAS/ThermalCamera_IN-CO1-D.git</code>
<li>install dependencies</li>
   <code>npm install</code>
<li>check the code with tslint</li>
  <code>npm run lint</code>
<li>Run the code in watch mode </li>
  <code>npm run start</code>
</ol>

<h2><strong>Execution</strong></h2>
<br>
<p>when you run the code you will get the parsing  data in your console and the original response of the device  in device_response folder</p>
