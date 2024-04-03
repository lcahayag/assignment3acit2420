Step 1!
Log into your ssh server!

ssh username@serverip

Step 2!
Update your package lists!

sudo pacman -Syu
sudo pacman -S vim nginx

Step 3!
Create a new directory for the project!!!

sudo mkdir -p /web/html/(name of project)

Step 4!
Edit the Nginx configuration file

sudo vim /etc/nginx/nginx.conf

Step 5!
Add this server block 

server {
    listen 80;
    server_name nginx-2420; # Your domain or IP address

    location / {
        root /web/html/nginx-2420;
        index index.html;
    }
}

Step 6
Save the file and exit vim 
Press esc and type (:wq!)

Step 7!!
Enable Nginx to start 

sudo systemctl enable nginx

Step 8
Start Nginx 

sudo systemctl start nginx

Step 9
Create index.html in the project directory and add the following code

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2420</title>
    <style>
        * {
            color: #db4b4b;
            background: #16161e;
        }
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        h1 {
            text-align: center;
            font-family: sans-serif;
        }
    </style>
</head>
<body>
    <h1>All your base are belong to us</h1>
</body>
</html>

Step 10
Get ip address!!!!!!!

Step 11
Enter ip address and behold at your progress!!!!!!!



