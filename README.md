# [BitBag](https://bitbag.io/) [Symfony Flex](https://symfony.com/doc/current/quick_tour/flex_recipes.html) Recipes

### We are happy to announce that we provided our own Symfony flex entrypoint :tada:

We would like to thank you Symfony Core-Team members which provided a Symfony Flex Serverless and the ability to create a [custom recipe server](https://symfony.com/blog/symfony-flex-is-going-serverless#custom-recipes)

## How to add entrypoint to project
Its simple! Just run:
```bash
composer config --json extra.symfony.endpoint '["https://raw.githubusercontent.com/piotrkardasz/bitbag-recipes/flex/main/index.json", "flex://defaults"]'
```
<sub>This command provides additional BitBag entrypoint for Symfony Flex.</sub>

## How to use it
#### Now you are ready to use Symfony Flex magic :exploding_head:

You can use our custom [aliases](https://symfony.com/doc/current/quick_tour/flex_recipes.html#flex-recipes-and-aliases) to add and autoconfigure our packages

For example to add `bitbag/wishlist-plugin` to your Sylius project you can run:
```bash
composer req wishlist
```
or to point specific version of the package:
```bash
composer req wishlist:1.7
```
Then Symfony Flex will configure a package for you!
It can also provide additional docker-composer configuration or instructions like, how to create Doctrine Migrations and so on.

![image](https://user-images.githubusercontent.com/40711740/149417990-d42a8f5a-400f-49fe-adad-c46b108092bc.png)

Enjoy! :tada:
