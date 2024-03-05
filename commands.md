# I'm a Lazy ass typist
```
alias drc=docker-compose
alias gs='git status'
```

# LOGS
docker-compose logs -t -f --tail 2000


# shell into Drupal container
```
docker exec -it my_drupal9_project_php /bin/bash
sudo mkdir web/sites/default/files
sudo chmod 777 web/sites/default/files
sudo cp web/sites/default/default.settings.php web/sites/default/settings.php

```

# Edit the settings file (in the PHP container)
```
vi web/sites/default/settings.php
```

# Add the gitpod.io trusted host pattern. (in the php container)
```
$settings['trusted_host_patterns'] = array(
  '.*\.gitpod\.io$',  '\.localhost$', '\.local$', '\.loc$'
);
```

# composer require the modules:

composer require drupal/ctools
composer require drupal/devel
composer require drupal/key
composer require drupal/admin_toolbar

composer require 'drupal/openai:^1.0@alpha'
composer require 'drupal/search_api_ai:^1.0@alpha'

#composer require 'drupal/openai:^1.0@alpha'
#composer require 'drupal/chatgpt_plugin:^2.1'
#composer require 'drupal/openai_ckeditor'
#composer require 'drupal/openai_content'
#composer require 'drupal/chatgpt_plugin'
#composer require 'drupal/openai_images:^2.1'
#composer require 'drupal/ai_image:^1.0@beta'

