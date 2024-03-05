1. login to GITPOD

2. User this REPO
https://gitpod.io/new#https://github.com/woutersf/workshop-mountain-camp-ch-24

3. Composer install

4. docker-compose start

5. Settings file fiddling

6. install Drupal

7. Configure openai KEY
/admin/config/openai/settings

Organisation
https://platform.openai.com/account/organization


8. Debug openai KEY on 
/admin/config/openai/chatgpt

9. Configure embeddings
/admin/config/openai/openai-embeddings/settings

10. 
sudo vi web/modules/contrib/openai/modules/openai_embeddings/src/Form/SettingsForm.php
Comment out validate handler contents

11. 
Add Block

12. 
