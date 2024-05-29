# poetry-cached-action

This Action caches poetry dependencies 

## Requirements

Your project must have a `poetry.lock` file already generated.

## Inputs
- **caching**: turn on/off the dependencies cache. Value: `true` or `false` (default: `true`)
- **poetry-version**: specify the poetry version. If not informed, a poetry version will be provided.

## How to use

```yaml
steps:
    - name: Load & cache dependencies
      uses: viniremigio/poetry-cached-action@v1
      with:
        caching: 'true'
        poetry-version: '1.8.3'
```

## Important
This Github Action is provided as an example to be used in personal projects. For more reliable actions serving the same purpose, please refer to other options in the [Github Marketplace](https://github.com/marketplace?query=poetry+cache).
