# homer
Homer - Dashboard App - Docker compose

Ver en "localhost:8200"

#######################################
```
EJEMPLO DE CONFIG.YML:

---
# Homepage configuration
# See https://fontawesome.com/icons for icons options

title: "Labarta"
subtitle: ""
#logo: "logo.png"
icon: "fas fa-home" # Optional icon

#header: true
footer: '<p><a>Creado por <a href="https://labarta.es/" style="color:red;">labarta</a></p>' # set false if you want to hide it.

# Optional theme customization
theme: default
colors:
  light:
    highlight-primary: "#3367d6"
    highlight-secondary: "#4285f4"
    highlight-hover: "#5a95f5"
    background: "#f5f5f5"
    card-background: "#ffffff"
    text: "#363636"
    text-header: "#ffffff"
    text-title: "#303030"
    text-subtitle: "#424242"
    card-shadow: rgba(0, 0, 0, 0.1)
    link-hover: "#363636"
    
  dark:
    highlight-primary: "#3367d6"
    highlight-secondary: "#4285f4"
    highlight-hover: "#5a95f5"
    background: "#131313"
    card-background: "#2b2b2b"
    text: "#eaeaea"
    text-header: "#ffffff"
    text-title: "#fafafa"
    text-subtitle: "#f5f5f5"
    card-shadow: rgba(0, 0, 0, 0.4)
    link-hover: "#ffdd57"

# Optional message
#message:
#url: https://b4bz.io
# style: "is-dark" # See https://bulma.io/documentation/components/message/#colors for styling options.
# title: "Demo !"
# icon: "fa fa-grin"
# content: "This is a dummy homepage demo. <br /> Find more information on <a href='https://github.com/bastienwirtz/homer'>github.com/bastienwirtz/homer</a>"

# Optional navbar
# links: [] # Allows for navbar (dark mode, layout, and search) without any links
links:
  - name: "Github"
    icon: "fab fa-github"
    url: "https://github.com/jmlcas/"
    target: "_blank" # optional html a tag target attribute
#  - name: "Wiki"
#    icon: "fas fa-book"
#    url: "https://www.wikipedia.org/"
  # this will link to a second homer page that will load config from additionnal-page.yml and keep default config values as in config.yml file
  # see url field and assets/additionnal-page.yml.dist used in this example:
#  - name: "another page!"
#    icon: "fas fa-file-alt"
#    url: "#additionnal-page" 

# Services
# First level array represent a group.
# Leave only a "items" key if not using group (group name, icon & tagstyle are optional, section separation will not be displayed).
services:
  - name: "Applications"
    icon: "fas fa-cloud"
    items:

      - name: "Cloud"
        subtitle: "NextCloud"
        logo: "assets/icons/nextcloud.png"
        url: "https://nextcloud.com"
        target: "_blank" # optional html a tag target attribute

      - name: "Wekan"
        subtitle: "kanban task manager"
        logo: "assets/icons/wekan.png"
        url: "https://wekan.github.io"
        target: "_blank" # optional html a tag target attribute

      - name: "Home Assistant"
        subtitle: "home automation"
        logo: "assets/icons/home-assistant.png"
        url: "https://home-assistant.io"
        target: "_blank" # optional html a tag target attribute

      - name: "Bitwarden"
        subtitle: "password manager"
        logo: "assets/icons/bitwarden.png"
        url: "https://bitwarden.com"
        target: "_blank" # optional html a tag target attribute


  - name: "Media"
    items: 

      - name: "Radarr"
        subtitle: "movies"
        logo: "assets/icons/radarr.png"
        url: "https://radarr.video"
        target: "_blank" # optional html a tag target attribute        

      - name: "Plex"
        subtitle: "media server"
        logo: "assets/icons/plex.png"
        url: "https://plex.tv/"
        target: "_blank" # optional html a tag target attribute    


  - name: "Admin Apps"
    items:

      - name: "NAS"
        subtitle: "synology"
        logo: "assets/icons/synology.png"
        url: "https://synology.com/es-es"
        target: "_blank" # optional html a tag target attribute        

      - name: "Code"
        subtitle: "server"
        logo: "assets/icons/code.png"
        url: "https://code.visualstudio.com"
        target: "_blank" # optional html a tag target attribute        

    ``` 
