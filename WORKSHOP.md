# login to GITPOD
https://gitpod.io

# User this REPO
https://gitpod.io/new#https://github.com/woutersf/workshop-mountain-camp-ch-24

# Composer install
Try sudo composer install, only for this demo.

# docker-compose start
or click the Whale and right click compose-start

# Settings file fiddling
```
docker exec -it my_drupal9_project_php /bin/bash
sudo mkdir web/sites/default/files
sudo chmod 777 web/sites/default/files
sudo cp web/sites/default/default.settings.php web/sites/default/settings.php
sudo chmod 777  web/sites/default/settings.php
```

# Install Drupal
You got this.

# Enable modules
- Admin toolbar
- search_api
- Search API AI
- Search API Pinecone
- OpenAI ChatGPT Explorer

# Configure openai KEY
/admin/config/openai/settings

Organisation
https://platform.openai.com/account/organization

# Debug openai KEY config
/admin/config/openai/chatgpt

# Configure embeddings
/admin/config/openai/openai-embeddings/settings

#  Oopsie
sudo vi web/modules/contrib/openai/modules/openai_embeddings/src/Form/SettingsForm.php
Comment out validate handler contents

# Confgure Search API
- Add Server
- Add index
- Add Fields
- field type embeddings

# Add block
Add Block to front page. 

# Add content
Create a few articles with some wikipedia conten

# Try it out
Ask questions to your Drupal!