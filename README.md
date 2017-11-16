symfony3-angular-material
=========================

A Symfony project created on November 14, 2017, 1:56 pm.
"# symfony3-angularjs-material" 

Installation

- Download source code from git repository.
git clone https://github.com/jslegend/symfony3-angularjs-material.git

- Install XAMPP on Windows 10.

- Set Virtual Host

Open file - C:\Windows\System32\drivers\etc\hosts

Add following string to set virtual host

127.0.0.1	mytest.com

Go to your XAMPP folder and open file

C:/XAMPP/apache/conf/extra/httpd-vhosts.conf

And add followings.

<VirtualHost *:80>

        ServerAdmin office@bzabc.tv
        
        DocumentRoot "PROJECT_PATH\web\app_dev.php"
        
        ServerName mytest.com # Please make sure this is same as hosts
        
        ServerAlias mytest.com *.mytest.com # Please make sure this is same as hosts
        
        <Directory "PROJECT_PATH\web\app_dev.php">
        
          Options Indexes FollowSymLinks Includes ExecCGI
          
          AllowOverride All
          
          Order allow,deny
          
          Allow from all
          
        </Directory>
        
</VirtualHost>

Run your Apache service.

Open your browser and input "mytest.com" to open the site.
