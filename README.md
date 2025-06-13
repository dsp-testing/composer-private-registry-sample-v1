Testing below functionalities

1. Composer
2. Private registry
3. Grouping
4. Multi directory

### Dowload package from public registry
composer create-project phpstan/phpstan:1.12.0 --no-dev phpstan-1.12.0

### Zip content
zip -r phpstan-1.12.0.zip phpstan-1.12.0

### Create json
cd phpstan-1.12.0

cp composer.json ../phpstan-1.12.0.json

cd ..

```
"name": "phpstan/phpstan",
  "version": "1.12.0",
```

### Deploy both to private registry
curl -u thavaahariharangit@github.com:<<token>> -T phpstan-1.12.0.zip https://jfrogghdemo.jfrog.io/artifactory/dependabot-php/phpstan/phpstan/phpstan-1.12.0.zip

curl -u thavaahariharangit@github.com:<<token>> -T phpstan-1.12.0.json https://jfrogghdemo.jfrog.io/artifactory/dependabot-php/phpstan/phpstan/phpstan-1.12.0.json

