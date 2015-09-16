![logo](https://raw.github.com/apiaryio/api-blueprint/master/assets/logo_apiblueprint.png)

# SnowPy
### API Blueprint Parser for Python
Pyton binding for the [Snow Crash](https://github.com/apiaryio/snowcrash) library.

API Blueprint is Web API documentation language. You can find API Blueprint documentation on the [API Blueprint site](http://apiblueprint.org).

** This project is in development. It has not been released yet. **


## Getting started

```python
import snowpy

result = snowpy.parse('# My API', export_source_map=True)
print(result.ast.name)
print(result.sourcemap.name)
```

## Parsing options

Options can be passed to the parser. We support `require_blueprint_name` and `export_source_map` option.

```python
import snowpy

options = {'export_source_map': True}
result = snowpy.parse('# My API', **options)
print(result)
```

## License
MIT License. See the [LICENSE](https://github.com/tomochikahara/snowpy/blob/master/LICENSE) file.
