"#CS634Project" 

The CVAT installation instruction that we followed is from the link that is provided in the Project page.

First of all, as we are using windows, we followed the windows 10 installation guide.

The step-by-step process is provided below:
1. Firstly, we have to install the WSL2 to use the Linux distributor. 
For that, we run this code in the command line,
wsl --install -d ubuntu

This installs the WSL2 in the desktop.

2. Then, we have to download and install Docker Desktop for Windows from the link provided in the CVAT page. 

3. Next, we have to install the Git for Windows from the link provided in the CVAT page.

4. Google chrome was already installed for both of us.

5. We started the ubuntu terminal and entered the following command to clone the latest develop branch.

git clone https://github.com/opencv/cvat
cd cvat

Then,

docker-compose up -d

then 

# enter docker image first
docker exec -it cvat_server /bin/bash
# then run
python3 ~/manage.py createsuperuser

after that, we inserted our username and password.

then we open the installed Google Chrome browser and go to localhost:8080

Lastly, if we type our username and password we are able to login.