# Write numbers as brazilian currency
> Using lib [num2words](https://pypi.python.org/pypi/num2words)

```python
from num2words import num2words

def num2words_ptbr(value, to_currency=False):
    params = {'lang': 'pt_BR'}
    if to_currency:
        params['to'] = 'currency'
    return num2words(value, **params)
```

# pytest coverage review
```bash
pytest --cov=<project_path> --cov-report=html --junitxml=htmlcov/results.xml <tests_path>
```
