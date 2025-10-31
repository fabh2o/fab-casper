in the theme folder, on the server (/home/fabh2o/storage/Docker/web/ghost_themes/fab-casper), run
    
    nvim package.json
    nvim assets/css/screen.css

    sudo docker run -it --rm -v .:/home alpine ash

in the docker container, run

    apk add nodejs
    apk add yarn
    cd /home
    yarn install
    yarn zip

on the PC, run

    cd ~/FM/Blog/theme
    scp server:/home/fabh2o/storage/Docker/web/ghost_themes/fab-casper/dist/fab-casper.zip

on the browser, upload the zip as a new theme
