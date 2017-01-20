# PHP Type hints convertor

Converts `@param` and `@return` annotations to PHP7+ native type hints.

## Usage

1. [Download](https://github.com/kukulich/php-type-hints-convertor/archive/master.zip) or clone

2. Install dependencies

    ```
    composer install
    ```

3. Edit [ruleset.xml](https://github.com/kukulich/php-type-hints-convertor/blob/master/ruleset.xml)

4. Run convertor

    ```
    vendor/bin/phpcbf --encoding=utf-8 --extensions=php --tab-width=4 --no-patch --standard=ruleset.xml directory_with_your_project
    ```

5. Run checker and add type hints that cannot be added automatically

    ```
    vendor/bin/phpcs --encoding=utf-8 --extensions=php --tab-width=4 --standard=ruleset.xml directory_with_your_project
    ```

6. Run your tests and check if everything is ok
