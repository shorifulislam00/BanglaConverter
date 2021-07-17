# BanglaConverter
Laravel helper class for convert number to english in word, bangla digit and bangla in word. Put this helper file in `app/BanglaConverter.php` 
In `composer.json` file under `autoload` add this file and run `composer dump-autoload`

    "autoload": {
        "files":[
            "app/BanglaConverter.php"
        ]
       }

### Convert to bangla digit
    
    echo BanglaConverter::bn_number(123456);

> Output: ১২৩৪৫৬
    
### Convert to english in word
    
    echo BanglaConverter::en_word(123456);
    
> Output: One lakh Twenty Three thousand Four hundred Fifty Six
    
### Convert to bangla in word
    
    echo BanglaConverter::bn_word(123456);
    
> Output: এক লক্ষ তেইশ হাজার চার শত ছাপ্পান্ন 

### Convert others like date, mobile no or other string which contain number
    echo BanglaConverter::bn_others('2021-07-17');

> Output: ২০২১-০৭-১৭

    echo BanglaConverter::bn_others(0186322222);

> Output: ০১৮৬৩২২২২২