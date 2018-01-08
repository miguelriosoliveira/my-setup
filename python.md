# Write numbers as brazilian currency
> Using lib [num2words](https://pypi.python.org/pypi/num2words)

```python
from num2words import num2words

def num2words_ptbr(num):
    num = float(num)
    int_part, dec_part = str(num).split('.')
    int_part = int(int_part)
    dec_part = int(dec_part if int(dec_part) >= 10 else dec_part + '0')

    int_word = num2words(int_part, lang='pt_BR')
    dec_word = num2words(dec_part, lang='pt_BR')

    int_currency = '{} {}'.format(int_word, 'reais' if int_part > 1 else 'real')
    dec_currency = '{} {}'.format(dec_word, 'centavos' if dec_part > 1 else 'centavo')

    final_word = '{}'.format(int_currency)
    if dec_part:
        final_word += ' e {}'.format(dec_currency)

    return final_word
```
