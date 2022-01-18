# Model-Viewer Starter


The following is a step-by-step run down to how to get started with setting up a local web-sever to host your model-viewer page so you can view it locally on your desktop and within the same local network on your mobile phone.


## Tools

- [VS Code](https://code.visualstudio.com/) one of the most used code editor in the industry for web and cloud application development. VS Code comes with a live preview extension as well which needs to be installed, see next point. 
- After you have installed VS Code, load and enable the Live Server extension which you can search from the Extensions Tab.
- Use VS Code to edit text files (.html, .css, .gltf) to customise your model-viewer website, see _Edit template_ below


## Step-by-step

- __Download__ the VS Code code editor (see Tools), then open VS Code and install the Live Server extension
- __Download__ code template from [github repo](https://github.com/sojamo/model-viewer-starter/archive/refs/heads/main.zip)
- __Open .zip__ file after download and place the model-viewer-starter-main folder where you can remember and find it
- __Drag__ model-viewer-starter-main folder over the VS Code Icon in your Dock, the model-viewer-starter project will open and you can see the file structure on the left side of the window
- __Go Live__, at the bottom of the window you can find a clickable area labeled __Go Live__, do click and activate the Live Server and your browser will open the model-viewer-starter web application. __Go Live__ by now should have changed to __Port:5500__ (number may vary) this tells you that the local web server for this project is accessible at port 5500 and the address that just opened in your web broswer should read like this http://127.0.0.1:5500 here, 127.0.0.1 s your loop back address, let's find out your local network address in the next step. 
- __Find__ your local network address (assuming you are on macos), press Alt and click on the wireless-network icon in your top menu bar. You will now see your available networks and the network you are connected to. Here read and note down the IP Address (which should look similar to this example local IP 192.168.10.23)
- __Test phone__ After you have written down the IP address of your (mac) computer, go to your mobile phone and make sure your wireless connection is connected to the same network as your computer. If this is the case, open a browser and key in the `IP address` of your computer (see previous step) followed by `:` and the `port number` that is used to serve your model-viewer-starter on your local network (for example 192.168.10.23:5500) and then followed by `/public` 
- Now if you have used and keyed in the correct URL, you should see the model-viewer-starter website on your phone

## glTF

The glTF format is a text based 3D format to load and display 3D objects (a glTF file can also come as binary).

- [Khronos glTF tutorials](https://github.com/KhronosGroup/glTF-Tutorials) get to know the glTF format
- [glTF viewer](https://gltf-viewer.donmccurdy.com/) can be useful to preview and text your glTF file 
- [model viewer examples](https://modelviewer.dev/examples/augmentedreality/) AR examples that can be opened with your phone 


## Edit template

You can edit the template you have downloaded earlier with VS Code. The following can be edited:
- __Website__ open `public/index.html`
- __Styles__ open `public/css/styles.css`
- __glTF file__ open `public/assets/2-blobs.gltf` or your glTF file that replaces this sample (make sure you edit index.html to load your glTF file if its name differs from the sample); here you can make changes to the color or material of a 3D object contained in the glTF file.
- __env-1.jpg__ edit file `public/assets/env-1.jpg` with photoshop, this is the texture used for the environment map when viewing the 3D model
- __sky-1.jpg__ edit file `public/assets/sky-1.jpg` with photoshop, this is the texture used for the skybox map when viewing the 3D model which afftects the reflection of a 3D object



