# Yii2 Transliterate Behavior
Автоматически выполняет транслитерацию текста

## Установка
Выполнить команду в консоли
```bash
composer require --prefer-dist sergks/yii2-transliterate-behavior "@dev"
```

или добавить в `composer.json`
```php
"require": {
    "sergks/yii2-transliterate-behavior": "@dev"
},
```

## Использование
```php
use sergks\transliterate\TransliterateBehavior;

public function behaviors()
{
    return [
        [
            'class' => TransliterateBehavior::className(),
            'fromAttribute' => 'title',
            'toAttribute' => 'alias',
        ]
    ];
}
```