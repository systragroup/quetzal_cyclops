add to:

.git/config


```
[filter "strip-notebook-output"]
	clean = "jupyter nbconvert --ClearOutputPreprocessor.enabled=True --ClearMetadataPreprocessor.enabled=True --to=notebook --stdin --stdout --log-level=ERROR"
```


add:

```
*.ipynb filter=strip-notebook-output
```

to .gitattribute