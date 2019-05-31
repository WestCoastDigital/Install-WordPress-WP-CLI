#Install WordPress - WP-CLI and Valet

```
cd sites
```

```
mkdir wordpress && cd wordpress
```

```
valet secure
```

```
valet db create wp_database
```

```
wp core download --skip-content --locale=en_AU
```

```
wp core config --dbhost=localhost --dbname=wp_database --dbuser=root --dbpass=root
```

```
chmod 644 wp-config.php
```

```
wp core install --url=https://wordpress.test --title="WordPress" --admin_name=admin --admin_password=admin --admin_email=name@domain.com
```

```
wp plugin install simply-show-hooks --activate
```

```
wp plugin install disable-gutenberg --activate
```

```
wp plugin install show-current-template --activate
```

```
wp plugin install imsanity --activate
```

```
wp theme install generatepress
```

```
cd wp-content/themes
```

```
git clone https://github.com/WestCoastDigital/WCD-Generatepress
```

```
wp theme activate WCD-Generatepress
```
